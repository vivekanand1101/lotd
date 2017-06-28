* Hard links point to same inode. They have to be on the same inode. They can only point to directories.  
* The inode is only deleted when the number of hard links to it is 0. The original file is also a link to the same inode.  
* Soft links are links to that file and not the inode itself. If the original file is moved, it won't get updated.  
* Soft links can be across filesystems since it's just a file pointing to other file.  
* Soft links can be pointing to a directory.  
* ```ln -s <new file> <original file or dir>``` will create a soft link.  
* ```ln <new file> <original file>``` will create the hard link.  
