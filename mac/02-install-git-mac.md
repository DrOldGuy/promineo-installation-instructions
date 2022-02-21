# Install Git for Mac OS

## Before you start
Check to see if git is installed. Type:

```
git --version
```

If you get a version number back, skip to the Setup section.

## Install Homebrew
* Open a Terminal window.
* Type all on one line, then press Return: 

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

You may need to add Homebrew to the path:

```
- Add Homebrew to your PATH in /Users/homefolder/.zprofile:
    echo 'eval $(/opt/homebrew/bin/brew shellenv)' >> /Users/homefolder/.zprofile
    eval $(/opt/homebrew/bin/brew shellenv)
```

* Type this, then press Return:

```
brew install git
```
 
## Reinstalling Git

If homebrew balks at installing Git over a previous installation, you can try this: [https://gist.github.com/brandonsimpson/54d9e085c9fde5e6ad3a](https://gist.github.com/brandonsimpson/54d9e085c9fde5e6ad3a)

## First-time setup
* Open a Terminal window.
* Type this, then press Return: 

```
git config --global user.name "John Smith" 
```

(Replace John Smith with your name. You must include the double quotes.)

* Type this, then press Return: 

```
git config --global user.email john.smith@gmail.com 
```

(Replace john.smith@gmail.com with your own email address.)
