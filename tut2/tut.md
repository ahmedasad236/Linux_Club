# Wild Cards

<!-- *__What and Why?__* -->

> patterns that work as placeholders in file and directory names

_**if you forget the actual name of a file or you want to use a command on a group of files**_

# \*

    used to replace one char or more (including zero)

### Example

```bash
    touch file{1..1000}.cpp
    // try to remove all files that has numbers between 400 and 500
```

# ?

    replace a single char

### Example

    in the above example delete all files between 30 and 40

#### _what if you need a condition on this char?_

    use [] and put the condition inside

| example     | explain                                       |
| ----------- | --------------------------------------------- |
| [abc]       | a or b or c                                   |
| [!abc]      | each char except (a,b,c)                      |
| [2-5]       | from 2 to 5                                   |
| [!2-5]      | each char except (2,3,4,5)                    |
| [a-z]       | all lowercase english letters                 |
| [a-z2-91-5] | all lowerCase english letters and from 1 to 9 |

### Example

    delete all files between 35 and 40

### useful class names

| class name  | usage                 | other method |
| ----------- | --------------------- | ------------ |
| [[:alpha:]] | Alphabets             | [a-zA-Z]     |
| [[:alnum:]] | Alphabets and numbers | [a-zA-Z0-9]  |
| [[:digit:]] | numbers               | [0-9]        |
| [[:lower:]] | lower case            | [a-z]        |
| [[:upper:]] | upper case            | [A-Z]        |

# {}

    very powerful wild card
    used to group selections

### Example

    touch {name1,name2}.{h,cpp}
    touch file{1..100}.cpp

### Note

_what is the difference between rm file[0-9].cpp , file{0..9}.cpp_

# \

    escape any special letter or space
