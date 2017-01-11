There are two basic libraries for concurrency in python:
* Multiprocessing
    As clear from the name, uses different processes and makes use of multiple
    CPUs and cores. There is separate memory space for each process. Useful, for
    CPU bound processes but with a catch that IPC is slower than between two threads.
* Threading
    Uses different threads. Won't make use of different CPU/cores. IPC is better.
    Helpful in case of I/O bound processes.

** More detailed discussion here: http://stackoverflow.com/questions/3044580/multiprocessing-vs-threading-python
