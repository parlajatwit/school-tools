# workspace

This tool opens the user's workspace for a specific class.  

# Usage
For every class in the school subdirectory, create a ``.workspace`` file.  
The contents of the ``.workspace`` file are a shell script that sets up the workspace as you see fit.  
For example: I would like to open the brightspace contents page and a terminal emulator in the notes working directory for my Operating Systems class.
```
#!/bin/sh

xdotool exec firefox -new-window $(brighturlgen -c os)
xdotool exec st -d $SCHOOL_DIR/os/notes
```

# TODO
- [ ] more workspace options? 
