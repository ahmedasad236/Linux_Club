# Coposite commands

## I/O streams
|Function|Stream Name|Stream Descriptor|Default Device|
|----|----|----|-----|
Input|stdin|0| keyboard|
Output| stdout| 1| screen
Error| stderr|2|screen
---

Composite Commands can be built through:
* Sequential Commands
* Conditional Commands
* Command loops
* Input/Output Redirection
* Pipes
* Command Argument Exception
* Command Argument Quoting
---

## 1- Sequential Commands

We can have multiple commands in the same line as follows,
`<first command>; <Second command>; ...; ...; etc`
#### Examples:
```bash
echo "one"; sleep 5; echo "Two"
```

> Using Sequential commands is useful when the first command takes long time to execute and we don't want to wait until it is complete.
```bash
g++ -g file.cpp; ./a.out
```

## <span style="background-color: Red">Note: </span>
```
The seq commands just run after each other, they have independent input & output
```

---
## Sequential Commands
* ### Oring ( || ): 
    * The second command will only execute only  if the first command returns false. 

    *   ```bash
        cat <file name> || echo "File Not Found"
        ```

    * It is used for error handling


* ### Anding ( && ):
    * Second command will only execute only if the first command returns true

    * ```bash
        mkdir dir1 && cd dir1
      ```
---

## Loop Commands

> We can build a loop to execute a specific command for several times

```bash
for file in *.txt
    > do
    > mv $file $file.old
    > done
```
---

## I/O Redirection


- ### Output Redirection

    - [`<command> > file`] (Redirect output to file and overwrite it)

    - [`<command> >> file`] (Redirect output to file and append it)

    - #### Example:
    ```bash
        echo "Linux community"

        echo "Linux community" > file.txt

        echo ls -a tut4 >> file.txt

        cat file1 file2 > mergedFiles.txt
    ```

    - ## <span style="background-color: Red">Note: </span>
        1.  **Error messages still go to screen**


        1. **">" Stands for "1>" which means redirect output streams.**
---
* ### Standard Error Redirection
    - [`<command> 2> file`]  (Redirect Error to file and overwrite it)

    - [`<command> 2>> file`] (Redirect Error to file and append it)

    - Examples: 
    (Output to screen & Error to the file)
    ```bash
        make 2> log 
        make 2>> log
    ```
---

*  ### Both Error & Output Redirection
    * Output and Error go to different files.
        * `<command> >file1 2>file2`
        * `<command> >>file1 2>>file2`

    * Output and Error go to the same file.
        * `<command> >file1 2>&1`
        * `<command> >> file1 2>>&1`
    
    * Short version of the previous command
        * `<command> &>file`
        * `<command> &>>file`

---
* ## Standard Input redirection
    * `<Command> < file`

    * Examples:
        ```bash
            wc -l file.txt
            
            sort < log-file > sorted-log-file

            spell < report.txt >> errors.txt
        ```
    
