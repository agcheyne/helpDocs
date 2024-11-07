## Creating Soft Links
You can create a soft link using the ln command with the -s option. ln by default is a hard klink

The syntax is:
ln -s /path/to/original/file.txt /path/to/shortcut/link_name

The l at the beginning of the permissions (lrwxrwxrwx) indicates it's a symbolic link.

## Removing Soft Links
To remove a soft link, you can use the rm command:
rm /path/to/shortcut/link_name

### note on hard vs soft links
Use Hard Links When:
- You Need Redundancy: Hard links are ideal when you want multiple filenames pointing to the same data so that even if the original file is deleted, the data remains accessible. Each hard link is essentially a full entry to the same data on disk.
- You Don’t Need to Cross Filesystems: Hard links only work within the same filesystem, so they’re best used when both files are on the same drive or partition.
- You Want to Save Disk Space: Hard links use minimal extra space because they don't duplicate data; they just add a new reference to the same data on the disk.
- The Link and Original File Should Be Treated Equally: With hard links, both the original file and the link are fully interchangeable because they share the same inode. Changes to one reflect on the other.
e.g. backups, same file in multiple locations


Use Soft Links (Symbolic Links) When:
- You Need to Cross Filesystems: Symbolic links can link files or directories across different filesystems or partitions, which is useful if you’re working with multiple drives.
- You Need to Link Directories: Only soft links can link to directories, so use a soft link if you want a shortcut to a folder.
- You Want Clear Visual Cues of the Link: Soft links are often used to make it clear that a file is just a shortcut. For example, /etc often has symbolic links to configuration files located elsewhere on the system.
- You Want to Link to Files that Might Move or Be Replaced: Symbolic links can point to filenames rather than specific data blocks, allowing you to replace the file without affecting the link. However, this can result in "broken links" if the target is moved or deleted.
e.g. config files, convience,
