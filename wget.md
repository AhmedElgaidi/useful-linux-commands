## wget:
1) It's a command line for downloading files from the internet/ remote server (WWW).
2) It could be used to take a copy/ mirror of a website for offline surfing for example.

### 1. Basic example:
```shell
    // Download a single file/ folder in the current directory and show the download progress, size, time and date.
    $ wget <link>
```

### 2. Download file with different name:
```shell
    // the flag is uppercase!!
    $ wget -O new_name <link>
```

### 3. Download Multiple files:
```shell
    // Here we are downloading as much number of files/folder we want in one shot.
    // It doesn't matter if the links have different protocols (http, https, ftp, ftps).
    $ wget <link1> <link2> <link3>
```

### 4. Download mutiple files from a file containg the target links:
```shell
    // The file.txt contains multple links, i want to download.
    // It download the target links in the current directory.
    $ wget -i file.txt
```

### 5. Follow a pattern in downloaing:
```shell
    // Let's say that you have a link 'https://www.example.com/products?productId=1' and you want to download (take copy) of all the products within a range
    // The following line should make a copy of the 25 products in the website in the current directory
    $ wget 'https://www.example.com/products?productId={1..25}
```