# Tools and Terminal


  ### 1- what is a command line

A command line, or terminal:- is a text based interface to the system. You are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text. 

 **Shell** :-This is a part of the operating system that defines how the terminal will behave and looks after running (or executing) commands for you. There are various shells available but the most common one is called bash which stands for Borne again shell.
 **Here is an example**:-  we can run with commend -(ls ./documents) and with out a commend  - (ls  -l)

**CD** :-which stands for change directory. usually will be run with a single command line argument which is the location we would like to change into. The location is specified as a path and as such may be specified as either an absolute or relative path.
*example:- cd documents    run    OR cd / run 



### 2-what is Linux:-Linux is an extension less system.

under **Linux** the system actually ignores the extension and looks inside the file to determine what type of file it is. 

- file extension is normally a set of 2 - 4 characters after a full stop at the end of a file, which denotes what type of file it is. The following are common extensions:

* file.exe - an executable file, or program.
* file.txt - a plain text file.
* file.png, file.gif, file.jpg - an image.
**examples**:- if we want to know  the file type we can use file commend on terminal

   * file[path]

**quotes**:-The first approach involves using quotes around the entire item. You may use either single or double quotes.Anything inside quotes is considered a single item.
**example**:-  cd 'holiday photos'

Another method is to use what is called an **escape character**, which is a backslash ( \ ). What the backslash does is escape (or nullify) the special meaning of the next character

**example** :- cd holiday\photos

hidden files and directors:-If the file or directory's name begins with a . (full stop) then it is considered to be hidden.
