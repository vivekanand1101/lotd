[Python Watchdog](https://github.com/gorakhargosh/watchdog) can be used to moniter filesystem events.
- Comes with ```watchdemo``` script for checking on terminal
- Can be used inside a script/app and also be run as daemon to automate tasks. [Workflow](https://github.com/mdipierro/workflow/blob/master/workflow.py), [Example script](http://brunorocha.org/python/watching-a-directory-for-file-changes-with-python.html)
- Some events: on_created, on_modified etc.
- If any file in the "watched" dir/location is modified/changed(based on definition), it will be caught.
