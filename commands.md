# Useful Linux Commands:

## grep:
- Stands for: **Global Regular Expression Print**.
- It's used to search for a specific string in a specific file (**return the lines that contain that word!**).

### 1. Basic example:
```shell
    // This searchs for any line that have word characters in the file "file.txt"
    grep word file.txt
```

### 2. Search for a word in multiple files:
```shell
    // This searchs for any line that have word characters "file1.txt" "file2.txt"
    grep word file1.txt file2.txt
```

### 3. Search for a word in the entire directory:
```shell
    // This searchs for any line that have word characters in the directory
    grep word *

```

### 4. Search for a specific word only

```shell
    // This searchs for a "word"
    grep -w word file1.txt 
```