# Screen sharing fundamentals

## Tracking

When people refer to trackings, they are usually talking about following a series of filters within a dump of any process using System Informer.

There are different ways to write trackings, but within this server, you will generally see them written like this:

`:\ -> .exe`

I've also seen them written in the following formats:
- `:\ > .exe`
- `csrss -> :\ -> .exe`
- `[csrss] :\ > .exe`
Ultimately, they all mean the same thing and refer to the same filtering process in System Informer. In this particular case, you should follow these steps:
1. Dump the CSRSS process.
2. Use Filter Contains (Case-Insensitive) and enter the first specified string. In this case, filter for `:\`.
3. Apply another filter using the next specified string. In this case, filter for .exe.
Now, you may also encounter situations where you need to filter using Regex. In these cases, trackings are usually not very complex, since you will generally only need to use one regex and shouldn't encounter many difficulties.

However, you may occasionally need to combine multiple filters. For example:

`^(?:\\\\\?\\)?[a-z]:\\.+$ -> .exe`

This is uncommon, since the regex is usually modified to match the required filter, but it is something you may encounter.

In this case, follow these steps:
1. Dump the process in System Informer (in this example, the regex is intended for CSRSS).
2. Apply a Regex (Case-Insensitive) filter using:
   `^(?:\\\\\?\\)?[a-z]:\\.+$`
3. After applying the first filter, apply another Contains (Case-Insensitive) filter using: .exe