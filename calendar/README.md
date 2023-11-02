# calendar
This tool manages your calendar.  
The primary use is to update an ical file located in ``SCHOOL_DIR/.calendar.ics`` from the link in the ``SCHOOL_DIR/.calendar_link`` file.  

To open the calendar, make the shell script ``SCHOOL_DIR/.calendar`` to launch whatever calendar program you use.  
For example:
```
#!/bin/sh

cal_location="/home/jeff/.local/share/calcurse"

calcurse -i "$SCHOOL_DIR"".calendar.ics" ; 
uniq "$cal_location/apts" > "$cal_location/test"
mv -f "$cal_location/test" "$cal_location/apts"
xdotool exec st calcurse
```

# TODO and ideas
- [ ] cron job to update every day?
- [ ] redownload on outlook calendar update hook?
