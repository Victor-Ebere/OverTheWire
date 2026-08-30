# Level0 - Level1

**Level Goal**
The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH(on port 2220) to log into that level and continue the game.

**Objective**
 In the course of this walkthrough, you'll learn two new commands,  'ls' and 'cat'. You'd also learn the necessary things you'd need to know about them. An extra would be the pwd command.
Keywords: Directory = Folder 

**To know**
1. ls: This is a command used to list the files or folders contained in your current directory. 

syntax: ls <flag> <directory_name>
FLAGS

* ls -l(long listing): It displays file permissions, owner name, group name, file size in bytes and the latest modification date/time
* ls -1(one per line): Forces the terminal to display exactly one file or directory on each line.
* ls -a(all files): It lists every single item in the folder, including hidden files.
* ls -R(recursive): Searches and displays everything inside the current folder, plus every subfolder and all files nested inside those subfolders.
 
example: You are in your home directory and it contains a directory named school which contains folders of each subject you are offering and files of your daily school activities
i. how do you list the content of school directory?
ans: ls school 
        or 
    1: cd school
    2: ls
ii. list the content of school directory with a detailed information of each file or directory.
ans: ls -l school
iii. list all the content and a full tree-like snapshot of the school directory structure.
ans: ls -aR school

2. cat: The cat command (short for concatenate) is a terminal utility used to read, combine, and display the text contents of files directly on your screen without opening a text editor.
syntax: Giving this to you as a challange exercise 
   run: man cat (To read about the syntax)
3. pwd: From the command p(present) w(working) d(directory). Present working directory, this is used to print out your current working directory. 

# SOLVING LEVEL 1
Instruction says the password is stored in a file called readme located in the home directory. I'd assume you've successfully ssh'ed into level0. 
**STEPS**
1. If you are not in the home directory, run 'cd' to get there. 
2. In the home directory we need to see its contents. So run ls
output: readme
3. We've found the file housing our password, now concatenate the readme file to see our password. 
cat readme
output: the password to move to level2

! [Graphical solution to OTW bandit mode level1](./images/lv0-lv1.png)

