* ```mount``` command shows how the physical or virtual drives are mounted on the system.  
* The drive that is mounted on ```/``` is the root one.  
* For virtual drives, they start with ```dev/vd*```  
* For physical drives, they start with ```dev/sd*```  
* The number in the end shows the partition number  
* For ```vfat``` partition based USB drive, they are mounted directly on ```/run/media/username```  
* For ```NTFS``` based external drive, a driver needs to be installed: ``` sudo dnf install ntfs-3g ```  
* We can use ```mount``` command to mount any file system to any directory of choice. Ex: ```sudo mount /dev/sda1 /mnt```  
* We can use ```unmount``` command on any directory to unmount the file system.  
* We can use ```sync``` to make sure that we avoid data loss upon unmounting the file system.  
