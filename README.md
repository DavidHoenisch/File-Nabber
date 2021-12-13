# File Nabber

This is a utility used to retrieve files from remote systems.  This was originally developed as a tool for working with malware.  After CVE-2021-44228 popped up, I made some improvements that would allow me to retrieve log files form remote systems for investigative/forensic purposes.  

### FUTURE OBJECTIVES

#### 1. SSH Key support (Completed on commit 8349bf7072f87024d7243856b94a7ce9b56cf9a4)
#### 2. Better error handling
#### 3. Progress tracker to show download progress 
#### 4. Hashing Functionality to establish basic forensics baseline
#### 5. Integration with Cuckoo Sandbox.  