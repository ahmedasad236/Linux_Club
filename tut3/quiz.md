# Redirecting Output to a File or Program

> ## 1. Which answer displays output to a terminal and ignores all errors? 

* a) &>file
* b) 2> &>file
* c) 2>/dev/null
* d) 1>/dev/null

> ## 2. Which answer sends output to a file and sends errors to a different file?

* a) >file 2>file2
* b) >file 1>file2
* c) >file &2>file2
* d) | tee file

> ## 3. Which answer sends both output and errors to a file, creating it or overwriting its contents?
* a) | tee file
* b) 2 &>file
* c) 1 &>file
* d) &>file

> ## 4. Which answer sends output and errors to the same file ensuring existing file content is preserved?

* a) >file 2>file2
* b) &>file
* c) >>file 2>&1
* d) >>file 1>&1

> ## 5. Which answer discards all messages normally sent to the terminal?

* a) >file 2>file2
* b) &>/dev/null
* c) &>/dev/null 2>file
* d) &>file

> ## 6. Which answer sends output to both the screen and a file at the same time?

* a) &>/dev/null
* b) >file 2>file2
* c) | tee file
* d) | < file

> ## 7. Which answer saves output to a file and discards error messages?

* a) &>file
* b) | tee file 2> /dev/null
* c) > file 1> /dev/null
* d) > file 2> /dev/null