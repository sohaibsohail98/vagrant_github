# Inside our VM ubuntu 16.04

## Day 1:

Commands:

We run the following command to make sure the vagrant environment is up to date and accepts all the disclaimers as yes:

```sudo apt-get update -y``` 

Where am I:

```pwd```

This command is to find our current path/directory


Who am I:

```who```

This command will print out who is using the BASH.


What do I have in my current directory:

```ls```

What do I have in my current directory: (Hidden files)

```ls -a```

Find out the name of the system I am using (Operating System):

```uname```

Clearing the current screen:

```clear```

How do we create a file within the directory:

```touch nameofthefile.extension```

How do we create a directory:

```mkdir nameofthedirectory```

How do I go inside the dir:

```cd nameofthedirectory```


Exercise:

- create two folders dir1, dir2
- in each folder create 2 files test1.txt and test2.txt
- check the current dir location and document the command to access the dir and exitO

Navigating through Gitbash:

- To navigate into the root directory, use "cd /"
- To navigate to your home directory, use "cd" or "cd ~"
- To navigate up one directory level, use "cd .."
- To navigate to the previous directory (or back), use "cd -"

Commands:

How to delete the file:

```sudo rm nameofthefile```

Root user (admin):

```sudo su``` or ```sudo -i```

How to check who is using the machine:

```id```

Echo is used to print on command line:

```echo "Hello"```

How can we go back to normal user:

```exit```

How can we install packages:

```sudo apt-get install nginx``` - This will install the nginx package

How can we check the status of program:

```systemctl status nameofthepackage```



## Day 2:

To access a directory within Mac's Terminal:

```cd ~/Documents/Sparta/starter-code```


For Mac Users running a new Vagrant file, and error can occur with VM saying the user created doesn't match with 
current user running Vagrant. To resolve this error, these are steps to resolve it:

Sometimes, it causes a conflict and it uses the one of the old .vagrant file to start up the machine. To avoid this
conflict and start from a completely new vagrant machine. 

```rm -r .vagrant```

This should remove the .vagrant file which deletes the conflict from a previous vagrant machine. In other words, 
resolving the error.  


In order to understand it fully we can ask following questions:

``` Communication is the key to succesful projects communications between Dev-Ops-Tester-QA and DevOps
What language is used to build this app?
What framework has been used?
Are they any dependencies to be installed together?
What will the app look like?
``` 

1. App folder synced vm with os
2. Node app requires nodes to be installed.
3. Ruby to be installed to run the tests


In order to run BASH as administrator on Mac, it is essential to run this command:

```sudo -i```

We installed a package called bundler, this command installs bundler. NOTE: Please run BASH as admin, otherwise
you have a permissions issue:


```gem install bundler```

After this installation, exit admin mode on Mac. Windows users do not need to do anything. Run the following command:


```bundle```

This will install two dependencies, and run the bundle within the directory.

We run a command to test our VM's dependencies:


```rake spec``` - NOTE: This command is running in the directory of Spec-tests (Outside of the VM machine)

We run a command to install python properties within our VM machine:


```sudo apt-get install python-software-properties```

These are the steps we took to install Node:


```
curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -

sudo apt-get install -y nodejs
```


Running an update to make sure all the dependencies and packages are up to date:


```sudo apt-get update```

Running PM2 package through NPM:


```sudo npm install pm2 -g```


Running an update again:


```sudo apt-get update```


Once we got this working, loading the app directory within the VM and then running another command:

```npm install```


Running an update again:


```sudo apt-get update```


Testing to make sure the app is running:


```node app.js```



Creating a new shell script file to make sure its executable:


```touch nginx_installation_script.sh```

```chmod +x nginx_installation_script.sh```


After this we edited the script file and added these commands to make it executable for commands:


```
#!/bin/bash

sudo apt-get update
sudo apt-get install nginx
sudo apt-get upgrade
```


To run the shell script file, this is the command to be needing to run:

``` 
./nginx_installation_script.sh
```


