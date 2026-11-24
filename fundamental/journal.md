# Screen sharing fundamentals

## Journal

The USN Journal is a feature available in all NTFS file systems. It records changes made to files within a disk or partition. During a screenshare (SS), this can be extremely useful, as it allows you to see, for example, whether a file has been deleted or renamed.

To read the journal, you can use tools such as [JournalTrace](https://github.com/spokwn/JournalTrace).

Below is a list of the changes that may be useful to us during a screenshare and what each one means.

- `Data Extend`: This change is recorded when data is added to a file, increasing its size.

- `Data Truncation`: This change is recorded when part of a file's data is truncated. This can happen when content is deleted from a file or when existing data is replaced with new data.

- `Overwrite`: This change is recorded when a file's data is replaced with other data.

- `Close`: This event is recorded when a file is closed after any modifications to it have been completed.

- `Rename`: This change is recorded when a file is renamed.

- `Delete`: This change is recorded when a file is deleted from the system.

- `Create`: This change is recorded when a new file is created.

- `Basic Info Change`: This change is recorded when a file's attributes are modified.