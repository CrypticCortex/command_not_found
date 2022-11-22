#### Note : Did the following only for Offline Installer.

* Mount the .iso file .
* Copy the contents of the iso file to your home direction.
* cd into your destination directory for me it is 
``` cd /home/kalyan/R2022A/ ```<br />
* Make a Temp directory inside 
``` /bin/glnxa64/```<br />

``` $ mkdir /home/kalyan/R2022A/bin/glnxa64/libcrypt ```

* cd back to base directory of Matlab folder

```export LD_PRELOAD=/lib64/libfreetype.so```

* Now do ``` ./install```
