* ```parted``` tool can be used to view and change the filesystem in the OS.  
* ```sudo parted /dev/sda/``` will run parted on ```/dev/sda```.  
* Inside the "parted" shell, we can use ```print``` to see the current scheme of partition.  
* We can create partitions using ```mkpart``` command, set flags etc in the "parted" shell itself.  
