# Screen sharing fundamentals

## File systems

### NTFS & FAT32

Basically, every disk or partition has a file system. The main drive (usually C:) typically uses the NTFS file system, whereas FAT file systems are more commonly found on USB flash drives or storage devices with less capacity.

The main difference between NTFS and FAT32 is that NTFS has a Journal, whereas FAT32 does not. Therefore, you won't be able to use the Journal to determine whether a file on a FAT32-formatted drive was renamed or deleted.

To check which format or file system a partition or disk uses, open Windows File Explorer, go to "This PC", and open the properties of the disk or partition you want to check. You will then see which file system it uses.