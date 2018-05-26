#### Umask application<p>
Umask is normally applied using two files**(SHELL STARTUP FILES)** in /etc directory i.e. are **profile** & **bashrc**.
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

If you want to apply specific umask to the users, you may choose to apply inside users **.bash_profile or .bashrc** file present in their home directory.


#### SUID, SGID & STICKYBIT

| Permission | Octal Value | Behaviour - File | Behaviour - Folder |
-------------|-------------|------------------|--------------------|
| SUID | 4 | Run as owner | N/A |
| SGID | 2 | Run as Group Owner | Inherit group owner |
| Sticky Bit | 1 | N/A | Delete file inside dir only if owner or owner of dir |


