# Screen sharing fundamentals

## Strings

A string is essentially a sequence of text characters. In screenshares (SS), when referring to strings, we usually mean strings that have been recorded in the memory of certain processes. For example, strings from pcaclient, which are recorded in explorer.exe, or SIGN.MEDIA, which is generated in the registry.

During a screenshare, using tools such as System Informer, you can dump processes and access their memory to filter for various useful strings.

In some cases, certain strings can help you confirm whether files have been executed. In other cases, they can provide information about files that were executed from a USB drive or, by using DPS, reveal strings containing the compilation dates of certain files.