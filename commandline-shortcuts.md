# Bash command line Shortcuts
Picked these from [here](http://www.skorks.com/2009/09/bash-shortcuts-for-maximum-productivity/)

### Command Editing Shortcuts

|**Command**|**Note**|
|:--------------------------------|:----------------------------------------------------------|
| <kbd>Ctrl</kbd> + <kbd>a</kbd> | go to the start of the command line |
| <kbd>Ctrl</kbd> + <kbd>e</kbd> | go to the end of the command line |
| <kbd>Ctrl</kbd> + <kbd>k</kbd> | delete from cursor to the end of the command line |
| <kbd>Ctrl</kbd> + <kbd>u</kbd> | delete from cursor to the start of the command line |
| <kbd>Ctrl</kbd> + <kbd>w</kbd> | delete from cursor to start of word (i.e. delete backwards one word) |
| <kbd>Ctrl</kbd> + <kbd>y</kbd> | paste word or text that was cut using one of the deletion shortcuts (such as the one above) after  |the cursor
| <kbd>Ctrl</kbd> + <kbd>xx</kbd> | move between start of command line and current cursor position (and back again) |
| <kbd>Alt</kbd> + <kbd>b</kbd> | move backward one word (or go to start of word the cursor is currently on) |
| <kbd>Alt</kbd> + <kbd>f</kbd> | move forward one word (or go to end of word the cursor is currently on) |
| <kbd>Alt</kbd> + <kbd>d</kbd> | delete to end of word starting at cursor (whole word if cursor is at the beginning of word) |
| <kbd>Alt</kbd> + <kbd>c</kbd> | capitalize to end of word starting at cursor (whole word if cursor is at the beginning of word) |
| <kbd>Alt</kbd> + <kbd>u</kbd> | make uppercase from cursor to end of word |
| <kbd>Alt</kbd> + <kbd>l</kbd> | make lowercase from cursor to end of word |
| <kbd>Alt</kbd> + <kbd>t</kbd> | swap current word with previous |
| <kbd>Ctrl</kbd> + <kbd>f</kbd> | move forward one character |
| <kbd>Ctrl</kbd> + <kbd>b</kbd> | move backward one character |
| <kbd>Ctrl</kbd> + <kbd>d</kbd> | delete character under the cursor |
| <kbd>Ctrl</kbd> + <kbd>h</kbd> | delete character before the cursor |
| <kbd>Ctrl</kbd> + <kbd>t</kbd> | swap character under cursor with the previous one |

### Command Recall Shortcuts

|**Command**|**Note**|
|:--------------------------------|:----------------------------------------------------------|
| <kbd>Ctrl</kbd> + <kbd>r</kbd> | search the history backwards |
| <kbd>Ctrl</kbd> + <kbd>g</kbd> | escape from history searching mode |
| <kbd>Ctrl</kbd> + <kbd>p</kbd> | previous command in history (i.e. walk back through the command history) |
| <kbd>Ctrl</kbd> + <kbd>n</kbd> | next command in history (i.e. walk forward through the command history) |
| <kbd>Alt</kbd> + <kbd>.</kbd> | use the last word of the previous command |


### Command Control Shortcuts

|**Command**|**Note**|
|:--------------------------------|:----------------------------------------------------------|
| <kbd>Ctrl</kbd> + <kbd>l</kbd> | clear the screen |
| <kbd>Ctrl</kbd> + <kbd>s</kbd> | stops the output to the screen (for long running verbose command) |
| <kbd>Ctrl</kbd> + <kbd>q</kbd> | allow output to the screen (if previously stopped using command above) |
| <kbd>Ctrl</kbd> + <kbd>c</kbd> | terminate the command |
| <kbd>Ctrl</kbd> + <kbd>z</kbd> | suspend/stop the command |


### Bash Bang (!) Commands

Bash also has some handy features that use the <kbd>!</kbd> (bang) to allow you to do some funky stuff with bash commands.

|**Command**|**Note**|
|:--------------------------------|:----------------------------------------------------------|
| <kbd>!!</kbd> | run last command |
| <kbd>!blah</kbd> | run the most recent command that starts with ‘blah’ (e.g. <kbd>!ls</kbd>) |
| <kbd>!blah:p</kbd> | print out the command that !blah would run (also adds it as the latest command in the command history) |
| <kbd>!$</kbd> | the last word of the previous command (same as <kbd>Alt</kbd> + <kbd>.</kbd>) |
| <kbd>!$:p</kbd> | print out the word that <kbd>!$</kbd> would substitute |
| <kbd>!\*</kbd> | the previous command except for the last word (e.g. if you type ‘find some_file.txt /‘, then <kbd>!\|</kbd> would give you ‘find some_file.txt‘) |
| <kbd>!\*:p</kbd> | print out what <kbd>!\|</kbd> would substitute |
