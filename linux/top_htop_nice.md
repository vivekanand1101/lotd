* top - will show the info about running/sleeping processes, how much
    memory they are consuming, %CPU utilization etc.```-u vivek``` switch
    will show all those processes run by user 'vivek'. ```-d 5``` will delay
    the refresh time of top. These can be sorted by some column value. ```-o colname```
* htop - A better top: both presentation and features.
* nice - You can run a script and set the priority which will be used during
  process scheduling (for CPU). -20 is the highest priority and 19 is the lowest priority. 
  ```sudo nice -n -20 python abc.py ``` You need to be superuser access to set
  a priority higher than 0
