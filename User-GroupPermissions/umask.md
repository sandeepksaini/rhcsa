#### Umask application<p>
Umask is normally applied using two files in /etc directory i.e. are **profile** & **bashrc**.
* profile - This file is used when you login to host and new shell is spawned by the host. Normally using ```ssh``` or GUI.
* bashrc - This file is used when you start a new child shell. Normally using ```su``` .

You can make changes to these file as below to understand the login behaviour of shell and how umask is applied using these files.
Changes made in **profile** file and similarlly you can insert changes to **bashrc** file too.

```
if [ $UID -gt 199 ] && [ "`/usr/bin/id -gn`" = "`/usr/bin/id -un`" ]; then
    umask 002
    echo "Applying umask to Normal USER. File Name : `echo $0`"
else
    umask 022
    echo "Applying umask to ROOT. File Name : `echo $0`"
fi
```

If you want to apply specific umask to the users, you may choose to apply inside users **bashrc** file present in their home directory.
