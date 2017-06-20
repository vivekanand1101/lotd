```os._exit```
 - terminate the process immediately
 - Does not clean up handlers or flushes stdio buffers
 - Should be only used in child process


```sys.exit```
 - is equivalent to: raise SystemExit()
 - Can be caught at higher level
