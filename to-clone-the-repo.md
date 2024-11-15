# Steps to be followed in order to clone the [Repository][3]
***
### *Step 1*
Create a [GitHub][1] Account and Login using that account.

### *Step 2*
Download and Install [Git ][2] in your computer.


### *Step 3*
After installing git open terminal and 

set the git config global information by running the following commands.

> `git config --global user.name "Your Name"`

> `git config --global user.email "your.email@example.com"`

Change replace the placeholder data with your own.

### *Step 4*
Open `Git bash` terminal and create a public-private key pair, using the command:
> `ssh-keygen -t rsa -b 4096 -f ~/.ssh/vkmkey`

### *Step 5*
go to `~/.ssh` folder and open the file `vkmkey.pub`, then copy the content of that file.

### *Step 6*
Go to GitHub and go to your `settings` and select `SSH and GPG keys`. 

Add a new `SSH key` by pasting the recently copied contents of the `vkmkey.pub`

to the relevant field. Remember to give a title to the key in the given and field,

Also keep the type of the key as `Authentication Key`

### *Step 7*
Now go to the `Git Bash` terminal and `cd` into the directory where you would like to

clone the GitHub repository.

### *Step 8*
Use the following commands to tell the terminal which Private key

to use to authenticate with, when using the git command.

> `eval "$(ssh-agent -s)"`

> `ssh-add ~/.ssh/vkmkey`

### *Step 9*
Use the following command to clone the repository to your local maching.
> `git clone git@github.com:tnuocca-wen/vkm-openemr.git`


[1]: <https://github.com> "GitHub Home Page"
[2]: <https://git-scm.com/downloads> "Git Download Page"
[3]: <https://github.com/tnuocca-wen/vkm-openemr> "VKM OpenEMR Repository"
