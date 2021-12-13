# File Nabber

This is a utility used to retrieve files from remote systems.  This was originally developed as a tool for working with malware.  After CVE-2021-44228 popped up, I made some improvements that would allow me to retrieve log files form remote systems for investigative/forensic purposes.  


## Usage

```
Options:
  -h, --help            show this help message and exit
  -f FILE, --file=FILE  Specify CSV file to read from
  -d DESTINATION, --destination=DESTINATION
                        Specify destiniation host
  -o OUT, --output=OUT  Specify where to save files that are downloaded
  -k KEY, --key=KEY     Define ssh key to be use for authenitcation
  -u USER, --user=USER  Define user to authenticate as
  -p PASS, --password=PASS
                        Define password to use in place of SSH key

```

You will need a csv file with the list of documents to grab.  
CSV REQUIREMENTS:

    1. Column header named `PATH`
   
    2. Absolute path to file in column `PATH`




### FUTURE OBJECTIVES

#### 1. SSH Key support (Completed on commit 8349bf7072f87024d7243856b94a7ce9b56cf9a4)
#### 2. Better error handling
#### 3. Progress tracker to show download progress 
#### 4. Hashing Functionality to establish basic forensics baseline
#### 5. Integration with Cuckoo Sandbox.  