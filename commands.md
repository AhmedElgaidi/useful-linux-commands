# Useful Linux Commands:

## 1) grep:
- Stands for: **Global Regular Expression Print**.
- It's used to search for a specific regular expression in a specific file (**return the lines that contain that word!**).

### 1. Basic example:
```shell
    // This searchs for any line that have word characters in the file "file.txt"
    $ grep word file.txt
    // such as words, wordlist etc.... not "word"!!
```

### 2. Search for a word in multiple files:
```shell
    // This searchs for any line that have word characters "file1.txt" "file2.txt"
    $ grep word file1.txt file2.txt
```

### 3. Search for a word in the entire directory:
```shell
    // This searchs for any line that have word characters in the directory
    $ grep word *

```

### 4. Search for a specific word only

```shell
    // This searchs for a "word".
    $ grep -w word file1.txt 
    // Only returns lines with "word" word.
```

### 5. To ignore case in search:

```shell
    // Search for any line that contains word characters (small or capital).
    $ grep -i word *
    // returns: WoRD, WORD, etc...
```

### 6. Search in sub-directorires also:

```shell
    // search for the "word" word in current directory files and it's sub-directorires files (**r means recrusive**).
    $ grep -wr word *
```

### 7. Inverse/ Negate the command:
```shell
    // search for all lines that don't contain those characters "word"
    $ grep -v word *
```

### 8. Search for exact line content:
```shell
    $ grep -x "hello my friend"
    // only returns lines that are exactly "hello my friend"
```

### 9. List names of files (Don't return lines):
```shell
    $ grep -l word *
```

### 10. Count the lines in the files  that contain the given regular expression:
```shell
    $ grep -c word *
```