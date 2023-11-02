# school-tools

The purpose of this repository is to hold tools I am writing to make my school workflow better. Many tools are subject to change, but I would like the overarching idea to be a unix-style set of tools, where every tool does one thing well and they interoperate with ease. We'll see how well this is accomplished with time :)  
  
## Usage
This suite of tools assumes a common "school" directory exists, with "classes" as subdirectories.  
The directory structure should be as follows:
```
school
├── datasci
├── ethics
├── os
├── security
└── sysadmin
```  
The environment variable ``SCHOOL_DIR`` should be the absolute path to this school directory.  
```
export SCHOOL_DIR="/home/jeff/school/fall_2023/"
```
I group my classes into semesters, so your path may be different.

## Included tools
- **brighturlgen** - generate urls to various brightspace content pages given a class id
- **workspace** - open multiple user-defined programs given a class name

