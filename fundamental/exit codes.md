# Screen sharing fundamentals

## Exit codes

An Exit Code is a number that indicates how a program's execution ended. If an error occurs while a file is running, the Exit Code will be greater than 0. If the Exit Code is 0, it generally means the program finished executing successfully, without errors.

In some cases, you may come across Exit Codes in places such as PcaGeneralDb, SgrmBroker, or JavaLauncher.log.

In these situations, it may be useful to know that some cheats terminate with specific Exit Codes when executed. Therefore, you may encounter cheats with unusually high Exit Code values.

In general, you can inspect Exit Codes through SgrmBroker. Simply dump the SgrmBroker process and use the following tracking:

exitcode -> .exe

A well-known Exit Code is 3221225786 in Notepad. If you come across this, it may indicate that the user injected a cheat DLL into Notepad.