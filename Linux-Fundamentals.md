# Room Name: Linux Fundamentals Part 1 
Date: 06/01/2026
Path: Concepts 
Difficulty: Easy


# Objective
What was the goal of this room/lab?
Go over the first part and learning about linux
A brief introduction to the history fo linux 





# Key Concepts Learned

## Concept 1

Linux is a computer language.
Ubuntu and Debian are some of the common places for distributions of Linux because its so extensible 

The Linux kernel was first released on September 17, 1991





















# Commands Learned

## Command
Echo Command
Output any text that i provide the machine 

-> TryHackMe Version

-> My Version



## Command
Whoami command
Finds out what user that i currently logged in as


-> TryHackMe Version

->My Version

## Command
Ls command
Listing files show us important files, documents,notes, and pictures



->Tryhack me version

-> My version


You can list out the contents of a directory by using ls and the name of the directory.
As seen in the image above


## Command
Cd command
It is short for change directory
Lets say i wanted to open up folder4 i would do “cd folder4”
I can also just put “cd” to go back to the home directory 


-> No TryHackMe Version
And ->My Version

## Command
Cat command
Simply seeing the contents of a text file 
Cat is short for concatenating and it output the contents and not just text files

Sometimes things like usernames, passwords (yes - really...), flags or configuration settings are stored within files where "cat" can be used to retrieve these. 


->TryHackMe Version


-> My Version


## Command
Pwd command
(Print Working Directory)
It can show that we are in a part of the computer but what about finding out where is this exactly on the linux machine’s filesystem
Using the pwd command to find the full file path to the specific folder.



-> TryHackMe Version

->My Version

## Command
Find Command
“find -name”
Okay lets say that we know the name of the text file or specific file we want to find but we dont know which directory or even folder its in the Find command will allow us to find it and also show the pathway to get to it 

-> TryHackMe Version

-> My version

Lets say that we dont know the name of the file or want to search every file that has an extension such as .txt so the find command allows us to do that aswell
“find -name *.txt”

 We will construct a command such as find -name *.txt . Where "Find" has been able to find every .txt file and has then given us the location of each one: 


->TryHackMe Version
Find has managed to find
Passwords.txt located within folder1
Todo.txt located within documents 


-> My Version

—-------












## Command
Grep Command
The Grep common allows us to search the contents of files for specific values we are looking for 



->TryHackMe Version





-> my Version




-> my Version

## Command
& Command
This allows us to execute commands in the background. Like lets say we were gonna copy a large file, usually it would take a long time but with this command e would be able to run it in the background while then we are able to do this.
The Number in the brackets like [1] or [2] is the Job ID
The 1354 is is the PID(process ID), which is the system’s unique identification number for that task

-> My Version


## Command
&& Command
SO this one allows us to do Command1 && command2 like if i wanted to do pwd and ls 
IT is noteworthy t say that command2 will only run if command 1 was successful

















## Command
> Command 
This is known as the output redirector it rakes the output we run from a command and sends that output somewhere else
im gonna do my best do explain what happened here so i did echo hi it printed back hi i did echo hello it printed back hello but now i did echo hi > hello so i put the echo hi inside of a new file named hello and then i used the cat command to open up the file Hello and it printed Hi 
ANOTHER NOTE it completely overwrites everything inside the file if it already exists. 

->TryHackMe Version

->My Version

## Command
>> Command
This command appends is also another output redirctor but what this does is instead of overwriting any contents within the said file, it just puts the output at the end it appends/attaches it the output.
The file would usually be at the end and the stuff your adding or rewriting is at the front


->TryHackMe Version

My Version




I  have achieved my first badge 

