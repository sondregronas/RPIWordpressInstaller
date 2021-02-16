# RPIWordpressInstaller
This 'one-click' installer is all you need to create multiple instances of Wordpress on a Raspberry Pi computer. The shell script is made specifically for classroom use, where the amount of students outnumber the amount of raspberry pi devices.

The user is prompted to type in a desired folder name, this will also create a database and a mysql user with the same input. (Password is by default set to 'password)

There should be zero requirements except a Raspberry Pi using Raspbian. Only works if the MySQL root password has not been set, though the shell script is made to be easily read and modified.

Adjust it to your own needs in your own classrom!

# How it works
When running the script it prompts you for a directory name, this creates a folder in the `/var/www/html` directory, where it'll install the latest version of WordPress. A database and mysql user is added with the same name, with the password 'password'.

When the setup is complete, it'll give you the url, 192.168.10.58/mydirectory, where you will be able to plot in the directory name. In this instance, Username and Database would be 'mydirectory'

# Installation
It's as simple as copy-pasting the following text:

```
git clone https://github.com/sondregronas/RPIWordpressInstaller && \
cd RPIWordpressInstaller && \
sudo chmod +x rpiwp-install.sh && \
sudo ./rpiwp-install.sh
```

You may have to run `sudo apt-get install git` beforehand.

You can also put the .sh file on a local machine, and replace git clone & cd with a `wget <url-to-file>`.
Feel free to modify it and personalize it!
