# mysy
my sync with iCloud

## description
mysy (my sync) is a tool that synchronizes your local directory to a directory in your iCloud drive.

### mysy
```
$mysy
```
synchronizes all the files listed in the config file.

### init
```
$mysy init
```
initialize mysy configuration at your current local directory `my/local/`. 
The target directory in your iCloud drive is `iCloud/mysy/local`. This can be customized with `-d` optional argument:

```
$mysy init -d mytarget
```
creates `iCloud/mysy/mytarget` as the target directory.

The initialization fails if the current local directory already has configuration files 
or the target directory in iCloud drive already exists. In the case, you can force the initialization using `-f` option

```
$mysy init -f 
```
this overwrites existing configuration files or shares the existing target directory

### add
```
$mysy add filename
```
adds `filename` (can contain path to subdirectory) to the mysy config file.

### list
```
$mysy list
```
show all paths in the config file. (the files that will be synchronized)

### remove
```
$mysy remove filename
```
remove filename from the config file

### change
```
$mysy change dir
```
change the target directory to `iCloud/mysy/dir` from the current one

### doctor
```
$mysy doctor
```
fix problems!







