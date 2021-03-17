## Read 01: 

Text editors or IDE's is a third party software used by web developers to write their code, While you can use the default software like notepad.
IDE's is more preferable choice cause of many reasons but in brief: using notepad sometimes can be frustrating and confusing when writing code because it doesn't have auto code completion, Error checking, Syntax highlighting, etc. There is a lot of famous text editors like Atom, Sublime text and VSCode, And when it comes to choosing the right IDE it will be a pure personal preference.
***
A command line, or terminal, is a text based interface that can be used to enter some commands or instructions that most of them won't display any information unless there was an error present. and the outcome will show on screen as a text. for instance if we type ls it will list  directories and files inside the current directory. 

in terminal there is something come along with it called shell and this is where the OS decide how the terminal will work and the expected outcome of running certain commands. In order to know what is the used shell you can use the command (echo $Shell) where echo can be used to print anything to terminal.
***
Linux treats everything like files even directories and the hardware itself like keyboard and monitor is treated so and when it comes to extensions, Linux is extension less unlike windows where you have to specify a type or extension for any file. 

Linux is case sensitive, For instance the command (ls) differs from command (lS) and each one do different things and that is a common mistakes that new comers face sometimes after seeing unexpected result.

Spaces in file and directory names are  allowed in Linux however it's may be tricky to do so because spaces is used to sperate items in the command line 

and from there you know what is the program name and can specify each command line argument. For instance if we tried to go to a directory called Holiday Photos using the command cd (cd Holiday Photos) it would give an error because (cd) command moves into the directory that is specified by the first argument only. And in order to fix this we use the quotes like so (cd 'Holiday Photos') or we can do it by escape character which is a backslash (cd Holiday\ Photos) that will treat the white space as it's not there (null) and these are the valid methods to use spaces in file names.

When it comes to hidden files Linux has a really unique way of representing them by simply putting a full stop sign (.) before the file name. To make a file or directory hidden we  make the file or directory with it's name beginning with a full stop sign like so (.file) and it gonna work the same with already existed files

if you want to hide a file simply rename it to begin with a full stop sign and to unhide just rename it removing the full stop sign. The command ls that show the files and directories won't show hidden file unless you have specified -a argument after it like so (ls -a).

 

**basic Linux commands that we learned was:**

1- `ls` : that would show the list of directories and files. and when u give -a after it it will include hidden files.

2- `file` : will get information about what type of file a file or directory is.

3- `cd` : it will take us to another directory.

4- `pwd` : will show the current working directory that we are inside. 

5- `echo` : which will print any given variable or text (echo hello world) for instance.