# String Usage Guidelines

All strings in the Plasma Engine are Utf8 encoded. As such they are accessible as simple `const char*` arrays.
However, one has to be very careful to distinguish between the "Element Count" (the number of bytes in the string) and the "Character Count".
Utf8 is a variable length encoding, which means that all ASCII characters (the first 127 characters in the ANSI set) are encoded with one byte.
Everything else can take between two and four bytes per character.
Therefore it is very dangerous to apply an algorithm to every byte in a string, as it might actually need to be aware of the individual characters.

Therefore all the string classes provide lots of high-level functionality for modifying the strings, which take care of these things internally.
On the other hand, direct access to the char array is not granted, to ensure the encoding does not get corrupted.

The following classes provide functionality to work on `char*` arrays:

* `plUnicodeUtils`
* `plStringUtils`
* `plPathUtils`

These generally implement 'read-only' functionality. The actual string classes provide the same functions, but with more comfortable interfaces.
Note that many of these functions take an 'end' pointer. This can generally be ignored, if you are working on zero terminated strings.
It can however also be used to work on non zero-terminated sub-strings.

## How to access C strings

Working on Utf8 strings is difficult, as you usually want to work on a per-character basis, which does not have a 1:1 mapping to bytes, when the data is Utf8 encoded.
To make this possible, use `plStringIterator`.

`plStringIterator` provides an interface on top of a char array, that allows to iterate forwards and backwards through a string on a per-character basis.
You can access the current character and get it in Utf32 encoding. This can easily be compared with standard C++ char-constants like 'a', 'b', '\\', '\\n', '\0' etc.

If you want to work on a per-character basis on a char that might be Utf8 encoded, you should always wrap it inside an `plStringIterator` and then use the iterator instead of accessing the array directly. Note that it only provides read-access though, as you cannot modify a Utf8 string in place in all circumstances.

Additionally there is `plStringView`, which allows to only work on sub-strings of other strings, which can be used to implement parsing functions very efficiently.

## How to create and modify strings

When you need to modify or build strings, use `plStringBuilder`.

`plStringBuilder` provides a large set of functions to easily modify strings. It includes a set of dedicated 'path functions' for working with paths (to prevent duplicate slashes, extract certain information etc.).

`plStringBuilder` uses an internal cache of 128 bytes, which is allocated on the stack. That means working with local `plStringBuilders` is very efficient, as usually no memory allocations are required, unless you build very long strings.

That in turn means, that you should never use `plStringBuilders` for storage, as they will waste a lot of memory. `plStringBuilders` should nearly always be local variables with a short life span.

## How to store strings

For storing strings, use `plString`.
`plString` is a typedef for `plHybridString<32>`. That means it has an internal cache for storing up to 32 bytes without the need for memory allocations. That usually covers more than 90% of all strings, which means that memory allocations are rare, but the amount of wasted memory is also relatively low.

`plString` does not provide functions to modify the string (other than completely replacing it), use `plStringBuilder` in such cases.

If you know that you are storing strings of certain lengths, e.g. filename extensions, you can use other predefined `plString`s, such as `plString8` or `plString48` to tune the internal cache size to be more fitting.

## How to convert strings between Utf8, Utf16, Utf32 and wchar_t

Plasma Engine provides a few classes to enable converting to and from all the Utf encodings and `wchar_t` encoding (which is simply Utf16 one some platforms and Utf32 on others).

The following classes take strings encoded in any encoding and convert them into their target encoding:

* `plStringWChar`
* `plStringUtf8`
* `plStringUtf16`
* `plStringUtf32`

Ie. an instance of `plStringWChar` will always encode a string to (the platform specific) `wchar_t` encoding and instances of `plStringUtf8` will convert strings to Utf8 encoding, etc.

Use it like this:

```cpp
plStringUtf8 MyUtf8 = L"My wchar_t string"; // The 'L' makes it a 'wide-string', ie. a wchar_t array
printf("Output Utf8: %s", MyUtf8.GetData());
```
  
or for interacting with win32 functions:
  
```cpp
plStringWChar FileNameW = MyUtf8FileName.GetData();
DeleteFileW(FileNameW.GetData());
```

This allows to quickly and easily convert back and forth between the different encodings.
Just make sure that you convert your data to Utf8 when you store something inside the Engine, and to the platform-specific encoding (typically `wchar_t`) when interacting with OS functions (unless they support Utf8 as well).

## See Also

* [Container Usage Guidelines](container-usage.md)
* [String Formatting](string-formatting.md)
