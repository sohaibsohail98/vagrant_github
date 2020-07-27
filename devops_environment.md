#Inside our VM ubuntu 16.04

# sudo apt-get update -y

- where am I - pwd is the command to find our current location 
- who am I - who is the command 
- what do I have available in current dir - ls is to check what's available inside the current directory, ls -a - this
will print out all files
- how can I find out the name of the system I am using - uname will print out the operating system
- clear command will clear the current screen

- how can we create a file - touch nameofthefile.extension - is the command to create a new file
- how do we create a directory - mkdir nameofthedirectory
- how do I go inside the dir - cd nameofthedirectory

-Exercise: create two folders dir1, dir2
- in each folder create 2 files test1.txt and test2.txt
-check the current dir location and document the command to access the dir and exitO

To navigate into the root directory, use "cd /"
To navigate to your home directory, use "cd" or "cd ~"
To navigate up one directory level, use "cd .."
To navigate to the previous directory (or back), use "cd -"

- how to delete the file - use - rm nameofthefile - use sudo rm nameofthefile

-root user (admin) - sudo su - command for root

-How to check who is using the machine - id

-echo is used to print on command line - echo "Hello"

- How can we go back to normal user - exit


- How can we install packages - sudo apt-get install nginx - ths will install the nginx package

- How can we check the status of program - systemctl status nameofthepackage
