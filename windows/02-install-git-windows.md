# Install git for Windows

## Install git

* In a browser, navigate to [here](https://git-scm.com/downloads). Select "Windows" in the Downloads section, or click the "Download for Windows" button.

* Double-click on the downloaded file to run the installer.
* Select all default settings except on the page named "Adjusting the name of the initial branch in new repositories", select option "Override the default branch name for new repositories" and verify that the name is set to "main" not "master".

## First-time setup
* Open a cmd window.
* Type this, then press Enter: 

```
git config --global user.name "John Smith" 
```

(Replace John Smith with your name. You must include the double quotes.)

* Type this, then press Enter: 

```
git config --global user.email john.smith@gmail.com 
```

(Replace john.smith@gmail.com with your own email address.)

## Set up SSH key

You can set up an SSH key to use between GitHub and the Git client so that you will not have to type in your password when pushing to GitHub. To create your SSH public and private key, follow the instructions [here](https://git-scm.com/book/en/v2/Git-on-the-Server-Generating-Your-SSH-Public-Key). I recommend that you create the key pair with no password or you will have to type your password every time you access the public key. You will quickly tire of this!

Next, you need to register your public key with GitHub. Follow these instructions:

1. In a browser, navigate to your GitHub main page. Click your profile icon in the upper right corner and select "Settings".
1. On the leftmost navigation pane, click "SSH and GPG keys".
1. Click the green "New SSH key" button.
1. Enter a name for the key (i.e., your name).
1. Navigate to your home/.ssh directory. Open the public key file (with the .pub extension). Copy the entire key to the clipboard.
1. Paste the key into the "Key" field. Click "Add SSH key".

Now, when you clone a repository, select "SSH" as the clone type. It should be automatically selected once you enter a public key.

**Warning**: make sure you copy your public key and not your private key! They are both generated in the home/.ssh directory. The default name of the the private key is **id_rsa**. The default name of the public key is **id_rsa.pub**. Windows users - make sure you can see the file extensions when you browse for files. To turn on this feature, open File Explorer, click the View menu, then select "Show". Make sure "File name extensions" is checked.