This is about ```/proc/``` 

* The files/folders in /proc/ are virtual since data is not stored in hard disk.
* Data is created dynamically in memory from raw kernel data at that point of time.
* ```cat /proc/cpuinfo``` gives info about the cpu in the system.  
* ```cat /proc/meminfo``` gives memory info in the system
* ```cat /proc/cmdline``` gives all the parameters passed to the kernel at boot time.  
* ```cat /proc/uptime``` uptime of the system. There is a command for that as well ```uptime```.  
* ```/proc/sys``` contains info about kernel. What features are enabled or not.  
* One can use ```sysctl``` command to change those values.  
