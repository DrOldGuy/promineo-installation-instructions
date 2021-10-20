# Install Java on the Mac

## Verify
Check to see if Java 11+ is already installed. Type this, then press Return

```
java -version
```

If the Java version is shown, and if it is version 11 or greater, you are all set.

## Download

* Download the Mac .pkg file from [here](https://corretto.aws/downloads/latest/amazon-corretto-11-x64-macos-jdk.pkg).

## Install

* Double-click the downloaded file to begin the installation wizard. Follow the steps in the Wizard.
* Run the following command in the Terminal to set the JAVA_HOME environment variable.

```
export JAVA_HOME=/Library/Java/JavaVirtualMachines/amazon-corretto-11.jdk/Contents/Home
```