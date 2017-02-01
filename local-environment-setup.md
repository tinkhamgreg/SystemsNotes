GIT (Already have an account)
go to https://git-scm.com/download/win
click on download button
run Git-2.11.0.3-64-bit.exe
follow through install instructions with default settings
To Run: open up command prompt
type "git", press enter

Bash install (Windows 10)
Go to settings
Go to update & security
Click "Developer Mode"
Click yes on the messagebox
Now search for "turn windows features on or off". Open the program.
Scroll down and check "Windows Subsystem for Linux(Beta)
After windows installs necessary files, click restart now.
To run, search for bash and run bash.exe
Upon opening , type y to continue installation.
After extracting filesystem, create a username and password.

To install git, type "sudo apt-get install git"
enter y to allow increase in disk space.

To install Docker
type "sudo apt-get install docker"

If you receive the error message that docker is not installed
even though you have installed it, try this command
"sudo curl -ssl https://get.docker.com/ | sh"
put in your root password if prompted

*Docker will not run on Windows 10 bash*



Install Git on Ubuntu
got to https://git-scm.com/download/linux
copy the command under Debian/Ubuntu
Open up the terminal
enter "sudo apt-get install git
To Run, type "git"


Install Docker on Ubuntu
Open the terminal
Enter "sudo apt-get update
Enter sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80 --recv-keys 58118E89F3A912897C070ADBF76221572C52609D 
Enter sudo apt-add-repository 'deb https://apt.dockerproject.org/repo ubuntu-xenial main'
Enter sudo apt-get update
Enter apt-cache policy docker-engine
Enter https://github.com/unh-comp-698-systems-software/notes.git to install Docker
To check the status of docker, enter sudo systemctl status docker

Enter docker run -it ubuntu:xenial /bin/bash
The program should return a "root@32432a23:/#" 

Setup Repository on Ubuntu
Go to your account page on Github
In the top right click the "+" symbol and click "new repository"
Name the repository whatever you like, leave the options unchecked and click "Done"



Local Repository on Ubuntu
GO to https://github.com/unh-comp-698-systems-software/notes
Click on "clone repository"
Copy the url
Open Terminal
go to the directory you wish to place the repository
Enter git clone https://github.com/unh-comp-698-systems-software/notes
Open up the "localenvironmentsetup.md file from Files and paste in the changes
Save the file

Now to Submit to Git
Open the terminal
Now you must navigate to the directory in which you want your repository to sit
if it is a folder within documents, you can enter "cd documents" and then "cd yourfile".
Now Enter "git init" to initialize this folder as a git repository
Now Configure your git account by entering "git config --global user.email "your email address"
And then enter git config --global user.name "A username"
Now you can add the files to your local repository by entering in git add .
Now you can commit those changes by entering in git commit -a -m "enter a message in this format"
-a means add everything in the commit and -m means add a message with the commit.
Enter git remote origin
Enter git remote add 'Your Folder Name Not in Parenthesis' 'The git repository url'
An Example of this can be seen here: greg@greg-VirtualBox:~/Documents/notes$ git remote add Systemnotes https://github.com/tinkhamgreg/SystemsNotes.git

Now we can push the repository to our repository on git
Enter git push 'Your filename not in parenthesis' master
Heres an example: greg@greg-VirtualBox:~/Documents/notes$ git push Systemnotes master
Enter your username in the prompt that you created above
enter the password for your github account
You should see output that describes transfering objects.
Here's an example:
Username for 'https://github.com': Tinkhamgreg
Password for 'https://Tinkhamgreg@github.com': 
Counting objects: 9, done.
Compressing objects: 100% (6/6), done.
Writing objects: 100% (9/9), 1.84 KiB | 0 bytes/s, done.
Total 9 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/tinkhamgreg/SystemsNotes.git
 * [new branch]      master -> master

You have successfully added your local changes to your git repository, you can check them online.






