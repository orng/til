# Write backup files to separate folder
By default, vim will write temporary backup files to the same file as your original file. Using this they will be put inside a .backup folder if you create one in your working dir, otherwise they will be put in /tmp. This prevents your directory from being cluttered by those unseemly files.

```
set backupdir=./.backup,.,/tmp
set directory=.,./.backup,/tmp
```
