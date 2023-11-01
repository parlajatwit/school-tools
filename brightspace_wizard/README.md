# brightspace_wizard

This tool helps speed up some common brightspace actions.  
It mainly generates URLs to class pages, saving time spent loading unneccessary resources and clicking through slow pages to get where you need to go.  

# Usage
For every class in the school subdirectory, create a ``.bright`` file with the contents as the brightspace class ID.  
For example: The link to a System Administration class is ``https://wentworth.brightspace.com/d2l/home/40273``, so the class ID is ``40273``.
```
$ echo 40273 > $SCHOOL_DIR/sysadmin/.bright
```

# To-do
- [ ] grade checker
- [ ] open brightspace pages
    - [ ] move help file to config folder?
- [ ] assignments due
- [ ] calendar module
