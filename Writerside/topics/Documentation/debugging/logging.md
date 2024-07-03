# Logging

Log messages are often very helpful in finding problems.

## Logging Information

The log is accessible through the `plLog` class. There are multiple functions to log information of different severity:

* `plLog::Debug` - for verbose output, will be compiled out in non-debug builds
* `plLog::Dev` - for output during development, will typically be silenced (but not compiled out) in non-development builds
* `plLog::Info` - for regular information
* `plLog::Warning` - for important information that may point at problems
* `plLog::SeriousWarning` - for problems that should be fixed but won't crash the system just now
* `plLog::Error` - for errors

Log messages can be *grouped* using the `PL_LOG_BLOCK` macro.

### TypeScript

Information can also be logged through the [TypeScript API](../custom-code/typescript/ts-api.md#pllog).

## Inspecting the Log

There are multiple ways to see the content of the log:

* In the [Plasma Editor](../../getting-started/editor-overview.md) you can open *Panels > Log* to see two logs, the one for the editor and the one from the engine process.
* [plInspector](../tools/inspector.md) shows the log of the connected process.
* The in-game [console](console.md) outputs the log messages.
* By default all Plasma [applications (TODO)](../runtime/application/application.md) also write the log output to a `Log.htm` file in the application's *appdata* folder.

## Thread-local logging

The logging system uses a thread-local variable to store the *active* logging system, through which to route all messages that originate on that thread. This can be used to easily replace the entire logging backend on a thread and capture all log messages in a custom backend. See `plLogSystemScope` and `plLogInterface`, if you want to write a custom backend. This can be used to, for example, capture all output from some subsystem and prevent the messages from reaching the regular outputs.

## Custom Log Writers

`plLog` is the central class for all messages to be logged. By default, it routes all messages through an instance of `plGlobalLog`, though you can redirect this on the calling side if you want. On `plGlobalLog` you can register multiple handlers that take the messages and either write them to some output or forward them to another system. This method is used to, for instance, forward log messages from one process to another. The [plInspector](../tools/inspector.md) integration, for example, registers a custom log writer to gather all log messages, and send them over the network, for display in the external tool. [Plasma Editor](../../getting-started/editor-overview.md) does something similar for the messages from the engine process.

For an in-depth explanation of how you can configure the system, see `plLog` and `plGlobalLog`.

## See Also


* [plInspector](../tools/inspector.md)
* [Console](console.md)