#### Note : Did the following only for Offline Installer.

* Mount the .iso file .
* Copy the contents of the iso file to your home direction.
* cd into your destination directory for me it is 
```$ cd /home/kalyan/R2022A/ ```<br />
* Make a Temp directory inside 
``` /bin/glnxa64/```<br />

``` $ mkdir /home/kalyan/R2022A/bin/glnxa64/libcrypt ```

* cd back to base directory of Matlab folder ```$ cd /home/kalyan/R2022A/``` and do

```$ export LD_PRELOAD=/lib64/libfreetype.so```

* Now do ```$  ./install```

* After Installing the packages needed , cd into ``` /usr/local/bin ```

* And do ``` $ sudo  ln -s $MATLAB/bin/matlab matlab ```
* But you will get an error ```ln: failed to create symbolic link 'matlab': Permission denied ```
* To overcome this you can add a flag ```--force``` after ```-s``` like <br />```$ ln -s --force /home/kalyan/bin/matlab matlab ```.
* If no matlab file exists in this directory (almost most of the time it will exisit but if you didn't chcek on create symlink during installation you can execute this <br />``` $ sudo ln -s $MATLAB/bin/matlab matlab ```
* libcrypt.so.1 error :
```error while loading shared libraries: libcrypt.so.1: cannot open shared object file: No such file or directory```
    Do this :
        ```sudo pamac -S libxcrypt-compat``` 
                or
        ```yay -S libxcrypt-compat```
