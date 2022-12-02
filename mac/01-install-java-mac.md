# Install Java on the Mac

## Verify
Check to see if Java 17+ is already installed. Type this, then press Return

```
java --version
```

If the Java version is shown, and if it is version 17, you are all set.

## Download

* Download the Mac .pkg file from [here](https://corretto.aws/downloads/latest/amazon-corretto-17-x64-macos-jdk.pkg).

## Install

* Double-click the downloaded file to begin the installation wizard. Follow the steps in the Wizard.
* Run the following command in the Terminal to set the JAVA_HOME environment variable.

```
export JAVA_HOME=/Library/Java/JavaVirtualMachines/amazon-corretto-17.jdk/Contents/Home
```

## Help! It didn't work!!

You may get a message that says Amazon Corretto can't be installed on this computer. If so, you can try an alternate approach. Below, you will find instructions to install Java using sdkman. If you prefer brew, you can research directions for that.

### Verify sdkman

1. Open a Terminal window.
1. Type: **sdk --help**. If you don't get a help page listing sdkman options, you will need to install sdkman.

### Install sdkman

1. In a Terminal window, type: **curl -s "https://get.sdkman.io" | bash**.

### Install Java

1. Open a __new__ Terminal window. Type: **sdk list java**. Note the identifier of the latest version of Amazon Corretto version 17 (something like 17.0.5-amzn). Type **q** to exit sdkman.
1. Type **sdk install java {{identifier}}** - so, something like **sdk install java 17.0.5-amzn**.
1. When the installation is complete, type **java -version** to verify.

Note: Java is installed in ~/.sdkman/candidates/java/{{identifier}}/bin.
For example: ~/.sdkman/candidates/java/17.0.5-amzn/bin.