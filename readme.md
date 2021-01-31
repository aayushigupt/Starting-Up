# Starting up with Ubuntu!!

Ubuntu Command Line is the Text Interface of our Computer. It can be also stated as a Terminal, Shell, Prompt, Console and many other names.

The Core part of linux is based upon Unix. 

The Code Program is said to be called **Shell Scripts**. Previously in the Unix the Shell Program is stated as sh but now it is extended in Linux it is stated as _bash_. 

Terminal and shell can be related to a coconut as Terminal is the outer part and shell is considered to be as a inner part of coconut. 
Terminal is the GUI interface where we write all the commands and shell is a software which is used to interpret all the commands and executes them.

### The following basic commands which are used :
---

1. _cd_ : It is used to change the directories.
2. _ls_ : It is used to list all the folders and files in that directory.
3. _mv_ : It is used to move the file in a particular location.
4. _cp_ : It is used to copy the content of the files.

Shortcut key of Terminal : `Ctrl-Alt-T`

After opening the terminal you will see some text it is said to be as odd text it is a way of computer to prompt you so that you can write the command after it.

To know the directory you are presently working can be known by:

```Ubuntu
pwd
```

pwd stands for **print working directory**

It will print **/home/$username**

To come back from the folder you have to use the command 

```Ubuntu 
cd ..
```

_Check there is a space between cd and .._

And to go to any folder you have to print command `cd`

By this command you will go to the root

```Ubuntu
cd /
```

Root is the base of the directory all the futhur directories and subdirectories starts from there.

Shortcut to go to **/home/$username** is **`~`**

And to go to Desktop you can directly use the shortcut  

``` Ubuntu
cd ~/Desktop
```

**Note : Linux is case sensitive so you have to take care of that so in Desktop D will always in caps**

### To create files and folders

To create a particular directory use the command mkdir which stands for make directory.

```Ubuntu
mkdir tmp
cd tmp
```
If you want you can also form multiple directories 

```Ubuntu
mkdir dir1 dir2
```

Here two directories will be formed **dir1** and **dir2**.
And if you want you can form as many as directories you want by following the same command.

`ls` is used to list all the items in a directory.

Also can create a file using redirection for eg:

```Ubuntu
ls > text_file.txt
```
Here it will create a file in working directory.

To write some content in the file you can use echo
```Ubuntu 
echo ""This is the text file"""
```
And to look at the content or output the content you can use cat for eg:
```Ubuntu 
cat text_file.txt
```
we can also form the files and put the content directly
```Ubuntu
echo "This is an another file" > text_2.txt
```
cat came from concatenate means linking together if we do

```Ubuntu
cat text_1.txt text_2.txt
```
Then it will print the content of both the files.

Two things which come first is `?` and second is `*`

if we do :

```Ubuntu
cat text_?.txt
```
Then it will print the same which it was printed in above command and also can do 

```Ubuntu
cat text*
```
it will again print the same we can also do `cat t*` it will print the output of the files which start with t and this is how the work becomes shorter and faster.
And ? this is used for only "single characters"

If we have to combined the text of both the files into an another file we can do like:

```Ubuntu
cat t* > combined_file.txt
cat combined.txt
```
So it will form an another file named as combined.txt which will contain the content of both the file text_1.txt and text_2.txt.


To see the whole file you can use new program **pager**

During previous time `more name_of_file` is used but now less is used. To see the file
```Ubuntu
less combined.txt
```
Here a pager will be opened and to exist type `q` you will go back to the shell.

Note : a.txt and A.txt will be considered as two different files

