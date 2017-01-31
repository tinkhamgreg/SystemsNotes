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



