
The video tutorial I am learning from 
https://youtu.be/8JJ101D3knE?si=rnR1-TTMUeeFHC9_


## Configuring git
System - all users
Global - All repositories of the current user
Local - the current repository 

Configuring git
- Name
- Email
- Default editor
- Line ending

To configure git 
git config -- {level} {variable} {value}

level = system, global, local
variable = user.name, user.email, core.editor
value = name, email, or text editor command

on text editor command you can use the "--wait" flag to wait for the text editor to close

## The configuration is stored in a file so u can edit it directly

git config --global -e 
The -e will open the default editor edit all of the global settings 

git init - to initiate a repository in the current directory
git add {file name} - adds the file into the staging area 
git commit - commits the files in the staging area to a commit log
 - -m == flag to include message in the commit.

Windows have both a carriage return and line feed character at the end of every line. I don't know why


git config --global core.autocrlf input [[What is core.autocrlf]] , [[What is core.autocrlf.2]]


## To learn more about git commands

You can search online for the documentation of the command or

To learn more about git commands you can use the --help flag or -h(Shorter manual page) to open the command documentation in the terminal. 
- I'm struggling to understand the documentation right now. But I think I'll learn how to understand it in the future.
- I actually am starting to understand it more now. I understood the --get flag for the git config command on my own and I as pretty happy exploring it on my own.

I played around with the git config --get command and I found out that if I don't specify what level I want like "git config --global --get user.name" and instead use "git config --get user.name" it will first try to access the system properties and if it can't then it will use the global properties if you're not in an initialized folder with its own local configuration. 

So if I am inside a git initialized repository and did "git config --get user.name" it will show the local user name.

If I am in the home directory for example, it will show the global user name, and if I run the command with sudo, it will gain root access which will allow it to access the system configuration and show the system user name. I think that's pretty cool.



