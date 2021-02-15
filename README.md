# RPIWordpressInstaller
This 'one-click' installer is all you need to create multiple instances of Wordpress on a Raspberry Pi computer. The shell script is made specifically for classroom use, where the amount of students outnumber the amount of raspberry pi devices.

The user is prompted to type in a desired folder name, this will also create a database and a mysql user with the same input. (Password is by default set to 'password)

There should be zero requirements except a fresh install of Raspbian. This shell script requires MySQL (if installed) to not have a root password, (it doesn't by default).

# Installation
It's as simple as copy-pasting the following text:

```
git clone https://github.com/sondregronas/RPIWordpressInstaller && \
cd RPIWordpressInstaller && \
sudo chmod +x rpiwp-install.sh && \
sudo ./rpiwp-install.sh
```

You may have to run `sudo apt-get install git` beforehand.
