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
