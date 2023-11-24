# Strings
[ String](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown) is a Lightning type used to represent text as a sequence of characters.

 #  Making Strings

In Lightning, a string literal is made by enclosing plasma or more characters in double quotation marks:

<pre><code class="language-csharp">
var greeting = "hello world";
var colorCode = "#F9EF1A";
var empty = "";
</code></pre>

 #  String Interpolation

*String interpolation* is a way of evaluating an expression and inserting it directly into a string literal. In Lightning, string interpolation is done using the **grave accent** character, ##`##. Anything in a string literal that is entered between two ##`##s is evaluated, and the result of that evaluation is used instead. For example:

<pre><code class="language-csharp">
var xp = Integer.PositiveMax;
var message = "Gained `xp` experience points.";
Console.WriteLine(message);

message = "Turn `Math.ToDegrees(Math.ACos(0.2)) - 15.0` degrees to starboard.";
Console.WriteLine(message);

message = "This component is attached to `this.Owner`.";
Console.WriteLine(message);
</code></pre>
<pre><code class="language-csharp">
Gained 2147483647 experience points.
Turn 63.463 degrees to starboard.
This component is attached to "Cog 'LevelSettings' [425]".
</code></pre>

String interpolation presents a handy means of joining two strings:

<pre><code class="language-csharp">
var str0 = "GAME";
var str1 = "OVER";
Console.WriteLine("`str0` `str1`");
</code></pre>
<pre><code class="language-csharp">
GAME OVER
</code></pre>

It can also be used to effectively "append" to a string:

<pre><code class="language-csharp">
var evenDigits = "";
var oddDigits = "";

for (var i = 0; i < 10; ++i)
{
  if (i % 2 == 0)
    evenDigits = "`evenDigits` `i`";
  else
    oddDigits = "`oddDigits` `i`";
}

Console.WriteLine("Even base-ten digits: `evenDigits`");
Console.WriteLine("Odd base-ten digits: `oddDigits`");
</code></pre>
<pre><code class="language-csharp">
Even base-ten digits:  0 2 4 6 8
Odd base-ten digits:  1 3 5 7 9
</code></pre>

Note that strings in Lightning are **immutable**, which means they cannot be altered after they have been created. Thus, strictly speaking, no true *appending* takes place. In the above code block, where it appears that `evenDigits` is being appended via string interpolation, a new string is actually created using the previous value of `evenDigits` and the value of `i`, and that new string is assigned back to the `evenDigits` variable.

(NOTE) Since this means of string appending involves the creation of another new string each time it occurs, it is less efficient than using a [ StringBuilder](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/stringbuilder.markdown), which is intended for just this purpose. In certain situations, such as a deeply nested loop, this performance difference may be significant.

 #  Escape Sequences

Some characters are entered in a string literal via special sequences of characters called //escape sequences//. In Lightning, all escape sequences consist of a backslash followed by another character.

<pre><code class="language-csharp">
// \" -- double quotation marks
Console.WriteLine("Say \"hello\" to Dr. Cosmo for me.");
Console.WriteLine();

// \` -- grave accent
Console.WriteLine("Press the \` key to open the console");
Console.WriteLine();

// \\ -- backslash
Console.WriteLine("C:\\Logs\\Analytics\\ForestLevel.Analytics.gamedata");
Console.WriteLine();

// \n or \r -- newline
Console.WriteLine("BEWARE\n  OF\r DOUG");
Console.WriteLine();

// \t -- horizontal tab
Console.WriteLine("+---+---+---+");
Console.WriteLine("1\t12\t123\t|");
Console.WriteLine("+---+---+---+");
</code></pre>
<pre><code class="language-csharp">
Say "hello" to Dr. Cosmo for me.

Press the ` key to open the console

C:\Logs\Analytics\ForestLevel.Analytics.gamedata

BEWARE
  OF
 DOUG

+---+---+---+
1   12  123 |
+---+---+---+
</code></pre>

 #  Strings and StringRanges

[ StringRange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/stringrange.markdown) is a separate but related class to **String**. It is an iterable range that can be used in a [ For Each loop](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/looping.markdown#for-each-loop). A string can be **implicitly cast** to StringRange, so a string can be passed into any function that expects a StringRange. However, a StringRange *cannot* be implicitly cast to String:

<pre><code class="language-csharp">
  var string = "";
  var stringRange = StringRange();
  
  this.FunctionTakingString(string);                  // okay
*this.FunctionTakingString(stringRange);             * error
  this.FunctionTakingString(stringRange.ToString());  // okay
  this.FunctionTakingStringRange(string);             // okay
  this.FunctionTakingStringRange(stringRange);        // okay
</code></pre>

 #  Static String Functions

[ As with all static functions](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/attributes.markdown#static), the static functions of the String class are not invoked from instances of the class, but instead are found in the String namespace itself.

 ##  Compare

[ Compare](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#compare-plasma-engine-docu) returns an Integer indicating the *relative sort order* of the two given strings; that is, whether one string would be sorted before another when comparing the character codes of the two strings:

<pre><code class="language-csharp">
var str0 = "abc";
var str1 = "def";

Console.WriteLine(String.Compare(str0, str1));
Console.WriteLine(String.Compare(str1, str0));
Console.WriteLine(String.Compare(str0, str0));
</code></pre>
<pre><code class="language-csharp">
-1
1
0
</code></pre>

This results in more or less the same ordering as one would use to sort entries in an English dictionary, except that because it goes by character codes, uppercase letters are sorted before lowercase letters, etc.:

<pre><code class="language-csharp">
var str0 = "cat";
var str1 = "dog";
var str2 = "DOG";

Console.WriteLine(String.Compare(str0, str1));
Console.WriteLine(String.Compare(str0, str2));
</code></pre>
<pre><code class="language-csharp">
-1
1
</code></pre>

This method is handy for sorting arrays of strings. [ Sort](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/array_t.markdown#sort-void) is an [ Array](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/array_t.markdown) method that sorts an array in place using a given comparison function:

<pre><code class="language-csharp">
var strings = Array[String]();

strings.Add("hi");
strings.Add("greetings");
strings.Add("nice to see you");
strings.Add("good morning");

Console.WriteLine(strings);

strings.Sort(String.Compare); // the Compare function is passed as a delegate

Console.WriteLine(strings);
</code></pre>
<pre><code class="language-csharp">
{hi, greetings, nice to see you, good morning}
{good morning, greetings, hi, nice to see you}
</code></pre>

 ##  Concatenate

[ Concatenate](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#concatenate-plasma-engine) can be used to join two existing strings:

<pre><code class="language-csharp">
Console.WriteLine(String.Concatenate("exa", "mple"));
</code></pre>
<pre><code class="language-csharp">
example
</code></pre>

 ##  FormatC

[ FormatC](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#formatc-plasma-engine-docu) produces a string using C-style string formatting syntax:

<pre><code class="language-csharp">
var score = 12340;
Console.WriteLine(String.FormatC("Score: %08d", score));
var hull = 100.0 * 43.0 / 64.0; // actual value 67.1875
Console.WriteLine(String.FormatC("Hull integrity at %.2f percent", hull));
</code></pre>
<pre><code class="language-csharp">
Score: 00012340
Hull integrity at 67.19 percent
</code></pre>

**FormatC** uses the same syntax as [the C printf function](http://www.cplusplus.com/reference/cstdio/printf/ ), with the following notes:
- the `p` format specifier can only be used with references to objects of reference types
- the `n` format specifier cannot be used
- the `#` flag can only be used with the `o`, `x`, and `X` specifiers
- the `.` precision marker must have its precision value specified

 ##  FromRune

[ FromRune](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#fromrune-plasma-engine-doc) returns a one-character string that consists of the given rune, which can either be passed in directly, or be specified by its code point:

<pre><code class="language-csharp">
Console.WriteLine(String.FromRune(65));
Console.WriteLine(String.FromRune(Rune(90)));
</code></pre>
<pre><code class="language-csharp">
A
Z
</code></pre>

 ##  IsNullOrEmpty and IsNullOrWhitespace

[ IsNullOrEmpty](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#isnullorempty-plasma-engin) returns true if the given string is either **null** or the empty string, `""`, and false otherwise. [ IsNullOrWhitespace](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#isnullorwhitespace-plasma) works just the same way, except that it also returns true if the given string consists only of **whitespace** characters:

<pre><code class="language-csharp">
Console.WriteLine(String.IsNullOrWhitespace("  \n  \t  "));
</code></pre>
<pre><code class="language-csharp">
true
</code></pre>

 ##  Join

[ Join](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#join-plasma-engine-documen) combines two, three, or four strings into one, placing a given separator string between them in the result:

<pre><code class="language-csharp">
var word0 = "Eeny";
var word1 = "Meeny";
var word2 = "Miney";
var word3 = "Moe";
var separator = ", ";
Console.WriteLine(String.Join(separator, word0, word1, word2, word3));
</code></pre>
<pre><code class="language-csharp">
Eeny, Meeny, Miney, Moe
</code></pre>

 #  String Properties

 ##  All

[ All](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#all-plasma-engine-document) converts the string into a StringRange. In Lightning, strings can be implicitly cast to StringRanges, so it is typically not necessary to use this property:

<pre><code class="language-csharp">
// Contains takes a StringRange
Console.WriteLine("homeowner".Contains("meow"));
Console.WriteLine("homeowner".Contains("meow".All));
</code></pre>
<pre><code class="language-csharp">
true
true
</code></pre>

 ##  Begin and End

[ Begin](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#begin-plasma-engine-docume) gets the RuneIterator at the start of the string, and [ End](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#end-plasma-engine-document) gets the RuneIterator at the end of it:

<pre><code class="language-csharp">
var fileName = "SnowLevel.Analytics.gamedata";
var levelName = fileName.SubString(fileName.Begin, fileName.FindFirstOf(".").Begin);
var extension = fileName.SubString(fileName.FindLastOf(".").End, fileName.End);
Console.WriteLine(levelName);
Console.WriteLine(extension);
</code></pre>
<pre><code class="language-csharp">
SnowLevel
gamedata
</code></pre>

 ##  ByteCount and Count

[ ByteCount](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#bytecount-plasma-engine-do) gets the number of bytes in the string. For a string that contains one or more characters outside of the ASCII range, this will be different from the number of runes represented by the string (see [ComputeRuneCount](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/strings/.markdown#computerunecount) below). Consider the following code example, attached to a cog that has a SpriteText component whose Text property is set to the French word //gar'on//:

<pre><code class="language-csharp">
var englishString = "string";
var frenchString = this.Owner.SpriteText.Text;

Console.WriteLine("The English string has `englishString.ByteCount` bytes");
Console.WriteLine("The French string has `frenchString.ByteCount` bytes");
</code></pre>
<pre><code class="language-csharp">
The English string has 6 bytes
The French string has 7 bytes
</code></pre>

The [ Count](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#count-plasma-engine-docume) property gets the same value as **ByteCount**, and exists for legacy purposes.

 ##  Empty and IsNotEmpty

[ Empty](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#empty-plasma-engine-docume) gets whether the string contains any characters at all:

<pre><code class="language-csharp">
var userNameInput = "";

if (userNameInput.Empty)
  Console.WriteLine("Please enter a name.");
else
  Console.WriteLine("Welcome, `userNameInput`.");
</code></pre>
<pre><code class="language-csharp">
Please enter a name.
</code></pre>

[ IsNotEmpty](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#isnotempty-plasma-engine-d) is always the exact opposite of **Empty**.

 #  String Methods

String methods are found on string instances, including literals:

<pre><code class="language-csharp">
Console.WriteLine("hello world".ToUpper());
</code></pre>
<pre><code class="language-csharp">
HELLO WORLD
</code></pre>

 ##  CompareTo

A string's [ CompareTo](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#compareto-plasma-engine-do) method returns an Integer indicating its relative sort order when compared with a given StringRange. It works much like the static [Compare](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/strings/.markdown#compare) function seen above, except that it compares a given StringRange to the string on which this method is being invoked.

 ##  ComputeRuneCount

The [ ComputeRuneCount](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#computerunecount-plasma-en) method calculates the number of runes represented by the string by iterating through it from its [Begin iterator to its End](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/strings/.markdown#begin-and-end). As noted [above](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/strings/.markdown#bytecount-and-count), a string that contains one or more characters outside of the ASCII range will have a different rune count from its byte count:

<pre><code class="language-csharp">
var englishString = "string";
var frenchString = this.Owner.SpriteText.Text;

Console.WriteLine("The English string has `englishString.ComputeRuneCount()` runes");
Console.WriteLine("The French string has `frenchString.ComputeRuneCount()` runes");
</code></pre>
<pre><code class="language-csharp">
The English string has 6 runes
The French string has 6 runes
</code></pre>

 ##  Contains

The [ Contains](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#contains-plasma-engine-doc) method checks whether a string contains a given substring:

<pre><code class="language-csharp">
var sentence = "DR. COSMO: \"I'm looking for a person named Brianna.\"";
var name0 = "Brian";
var name1 = "Anna";

Console.WriteLine(sentence);

if (sentence.Contains(name0))
  Console.WriteLine("* BRIAN: \"Did someone mention me?\"");
if (sentence.Contains(name1))
  Console.WriteLine("* ANNA: \"My ears are burning.\"");
</code></pre>
<pre><code class="language-csharp">
DR. COSMO: "I'm looking for a person named Brianna."
* BRIAN: "Did someone mention me?"
</code></pre>

As this example shows, **Contains** is case-sensitive, but it does *not* match only complete words. `Brianna` contains `Brian`, and it does contain `anna`, but not `Anna`.

 ##  EndsWith and StartsWith

The [ EndsWith](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#endswith-plasma-engine-doc) method checks whether a string ends with a given substring:

<pre><code class="language-csharp">
var fileNameToOpen = "DesertLevel.Analytics.gamedata";

var validFileExtension = ".gamedata";

if (fileNameToOpen.EndsWith(validFileExtension))
  Console.WriteLine("Opening `fileNameToOpen`....");
else
  Console.WriteLine("`fileNameToOpen` is not a valid file");
</code></pre>
<pre><code class="language-csharp">
Opening DesertLevel.Analytics.gamedata....
</code></pre>

The [ StartsWith](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#startswith-plasma-engine-d) method works the same way, except that it checks the beginning of the string instead the end.

 ##  Replace

The [ Replace](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#replace-plasma-engine-docu) method returns a new string, with all occurrences of a given old substring replaced with a given new substring:

<pre><code class="language-csharp">
var dialogueFromFile = "Oh, [HERO_NAME]! Your friend [VILLAIN_NAME] was looking for you.";

var heroName = "Brianna";
var villainName = "Dr. Cosmo";

var dialogue = dialogueFromFile.Replace("[HERO_NAME]", heroName);
dialogue = dialogue.Replace("[VILLAIN_NAME]", villainName);

Console.WriteLine(dialogue);
</code></pre>
<pre><code class="language-csharp">
Oh, Brianna! Your friend Dr. Cosmo was looking for you.
</code></pre>

 ##  Split

The [ Split](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#split-plasma-engine-docume) method scans a string for a given delimiter StringRange of one or more characters. The substrings that were found separated by occurrences of that delimiter, if any, are returned as an iterable range. The delimiter itself is not present in the split results:

<pre><code class="language-csharp">
var dataFromFile = "0,0,2,0,5,4,1,1,0,0,0,1,1,3,5,1";
var splitResults = dataFromFile.Split(",");

// splitResults now contains "0", "0", "2", "0", "5", "4", and so on

var total = 0;

foreach (var result in splitResults)
  total += Integer.Parse(result);

Console.WriteLine("Data Total: `total`");
</code></pre>
<pre><code class="language-csharp">
Data Total: 24
</code></pre>

NOTE: [ Parse](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown#parse-plasma-engine-docume) is a static [ Integer](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/integer.markdown) function. It takes a StringRange and interprets it as if it were an Integer, and returns that value. Equivalent static functions exist in other classes, such as [ Real](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/real.markdown), [ DoubleInteger](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/doubleinteger.markdown), etc.

 ##  SubString, SubStringBytes, and SubStringFromRuneIndices

The [ SubString](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#substring-plasma-engine-do) method returns the snippet of a string that is bounded by the two given RuneIterators. This may be the entire string itself, or it may be a smaller portion thereof:

<pre><code class="language-csharp">
var name = "The Evil Dr. Cosmo";

var firstSpace = name.FindFirstOf(" ");
// firstSpace refers to the space directly after "The"
var title = name.FindFirstOf("Dr.");
// title refers to the "Dr." between "Evil" and "Cosmo"
var lastSpace = name.FindLastOf(" ");
// lastSpace refers to the space directly before "Cosmo"

var part0 = name.SubString(name.Begin, firstSpace.Begin); // "The"
var part1 = "Handsome but Misunderstood";
var part2 = name.SubString(title.Begin, title.End);       // "Dr."
var part3 = "Eugene";
var part4 = name.SubString(lastSpace.End, name.End);      // "Cosmo"
var part5 = "IV";

var revisedName = "`part0` `part1` `part2` `part3` `part4` `part5`";

Console.WriteLine(revisedName);
</code></pre>
<pre><code class="language-csharp">
The Handsome but Misunderstood Dr. Eugene Cosmo IV
</code></pre>

 - See also [FindFirstOf](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/strings/.markdown#findfirstof)
 - See also [FindLastOf](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/strings/.markdown#findfirstof)

Besides **SubString**, there are two other String methods that return substrings:

- [ SubStringBytes](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#substringbytes-plasma-engi) returns a string's substring that starts at the given byte index and runs for the given byte length:

<pre><code class="language-csharp">
var str = "abcdefghij";
//         0123456789
//      start ^
//            12345
//                ^ 5 bytes long
var sub = str.SubStringBytes(3, 5);
Console.WriteLine(sub);
</code></pre>
<pre><code class="language-csharp">
defgh
</code></pre>

IMPORTANT: A string that contains characters that are outside of the ASCII range will not have a matching rune count and byte count. Using **SubStringBytes** on such a string may produce undesired behavior.

- [ SubStringFromRuneIndices](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#substringfromruneindices) returns a string's substring that starts at the given starting rune index and ends one past the given ending rune index:

<pre><code class="language-csharp">
var str = "abcdefghij";
//         0123456789
//     start ^      ^ one past the end
var sub = str.SubStringFromRuneIndices(2, 9);
Console.WriteLine(sub);
</code></pre>
<pre><code class="language-csharp">
cdefghi
</code></pre>

NOTE: Finding a given rune by its index requires a linear search through a string. Because **SubStringFromRuneIndices** requires two such searches, this method can be slower than **SubString**. In certain situations, such as a deeply nested loop, this performance difference may be significant.

 ##  ToLower and ToUpper

The [ ToLower](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#tolower-plasma-engine-docu) method returns a copy of the original string with all of its letters converted to lowercase. Any character that is not an uppercase alphabetical character is unchanged:

<pre><code class="language-csharp">
var sentence = "gEt ReKT scRUb";
var forbiddenWord = "scrub";

var lower = sentence.ToLower();

if (lower.Contains(forbiddenWord))
  Console.WriteLine("You have been reported for bad manners.");
else
  Console.WriteLine(sentence);
</code></pre>
<pre><code class="language-csharp">
You have been reported for bad manners.
</code></pre>

The [ ToUpper](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#toupper-plasma-engine-docu) method is just like ToLower, except that it converts letters to uppercase:

<pre><code class="language-csharp">
var name = "Johnny";
var upperName = name.ToUpper();
var dialogue = "`upperName`: \"This is `name`.\"";
Console.WriteLine(dialogue);
</code></pre>
<pre><code class="language-csharp">
JOHNNY: "This is Johnny."
</code></pre>

 ##  Trim, TrimEnd, and TrimStart

The [ Trim](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#trim-plasma-engine-documen) method returns a copy of the original string with all of its whitespace characters removed from its beginning and end:

<pre><code class="language-csharp">
var untrimmedID = "    f08b47e1            ";
Console.WriteLine("Your ID is `untrimmedID`. Write it down.");

var trimmedID = untrimmedID.Trim();
Console.WriteLine("Your ID is `trimmedID`. Write it down.");
</code></pre>
<pre><code class="language-csharp">
Your ID is     f08b47e1            . Write it down.
Your ID is f08b47e1. Write it down.
</code></pre>

[ TrimEnd](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#trimend-plasma-engine-docu) and [ TrimStart](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown#trimstart-plasma-engine-do) work just the same as **Trim**, except that **TrimEnd** only trims whitespace characters from the end of the string, and **TrimStart** only trims from the start of the string.

 #  Related Materials
 ##  Manual
- [ Looping](https://plasmaengine.github.io/PlasmaDocs/Plasma1/Editor/Lightning/looping.markdown)

 ##  Code Reference
- [ String](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/string.markdown)
- [ StringRange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/stringrange.markdown)
- [ StringBuilder](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/stringbuilder.markdown)
- [ StringSplitRange](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/stringsplitrange.markdown)
- [ Rune](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/rune.markdown)
- [ RuneIterator](https://github.com/PlasmaEngine/PlasmaDocs/tree/master/docs/C%2B%2B/code_reference/lightning_base_types/runeiterator.markdown) 

 