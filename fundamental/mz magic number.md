# Screen sharing fundamentals

## MZ magic number

MZ is the magic number (file signature) used by Windows executable files.

Some tools, such as Paths Parser or UserAssistView, include an analysis of this signature and can show us when it is no longer in the same state as it was at the time of execution.

You may encounter the "Not MZ" flag. This indicates that the original executable file may have been modified or replaced. However, we must confirm this through the USN Journal, as explained in the Replaces (not here yet).

It is also important to clarify that, although this is a good indication for suspicion, it does not necessarily mean that the program has been modified.