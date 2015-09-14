#Drawer Node.js v1.0.0 Documentation
This module is simple http-server framework which contains utilities for handling and organizing files by file extensions.
Using drawer, files can be saved and load by file-name and list files up very simply.

## List of Contents
* drawer.init(dir)
* drawer.writefile(filename, data)
* drawer.readfile(filename)
* drawer.readfile(filename)
* drawer.removeFile(dirname)
* drawer.fileList(dirname)


## drawer.init(dir)
Initialized drawer in local directory. 
It will be created photo/musin/documentation/javascript/html/etc as sub-folder in drawer automatically.

###Example
```
var Drawer = require('drawer');
var drawer = new Drawer();
drawer.init(__dirname);
```
It will be created drawer folder which has sub-folders(photo/documentation/javascript/html/ect) in __dirname.


## drawer.writefile(filename, data)
Write file data and it will be automatically stored into the folder where sorted by extension. 

###Example
```
var Drawer = require('drawer');
var drawer = new Drawer();
drawer.writefile(filename, data);
```

##drawer.readfile(filename);
Read file with only filename. The location will be searched by file extension and load the file.
```
var Drawer = require('drawer');
var drawer = new Drawer();
drawer.readfile(filename);
```

##drawer.filelist(file-type);
Show the list of files which has been sorted by extenstions. 
```
var Drawer = require('drawer');
var drawer = new Drawer();
drawer.filelist('photo');
```
It will be shown the list of photos you have in drawer.








