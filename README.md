# Linux-Dev-Setup
## My Linux Dev Environment Setup

**Check and Install Package Updates**
```
sudo apt-get update && sudo apt-get dist-upgrade
```
**Java**
```
sudo apt install openjdk-11-jdk
java -version
```
**Visual Studio Code**
```
sudo snap install code --classic
```
**Slack**
```
sudo snap install slack --classic
```
**Postman**
```
sudo snap install postman
```
**VLC**
```
sudo snap install vlc
sudo apt install ubuntu-restricted-extras
```
**Zoom**
https://support.zoom.us/hc/en-us/articles/204206269-Installing-or-updating-Zoom-on-Linux#h_89c268b4-2a68-4e4c-882f-441e374b87cb

**Installing curl, make, vim**
```
sudo apt install curl make vim
```

**Additional Archive Utilities**
```
sudo apt install rar unrar p7zip-full p7zip-rar
```
**Terminal Configuration — Case-insensitive tab completion**
```
if [ ! -a ~/.inputrc ]; then echo '$include /etc/inputrc' > ~/.inputrc; fi
echo 'set completion-ignore-case On' >> ~/.inputrc
```

## Git Set-up
```
sudo apt install git
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```
SSH for Github : https://github.com/settings/keys
SSH for Gitlab : https://gitlab.com/-/profile/keys
```
ssh-keygen -t ed25519 -C "your_email@example.com"
xclip -sel clip < ~/.ssh/id_ed25519.pub
touch ~/.ssh/config
nano  ~/.ssh/config
```

```
Host github.com
        User git
        Hostname github.com
        PreferredAuthentications publickey
        IdentityFile /home/user/.ssh/id_ed25519

Host gitlab.com
        PreferredAuthentications publickey
        IdentityFile /home/user/.ssh/id_ed25519
```

**Test Github and Gitlab SSH**
```
ssh -T git@github.com
ssh -T git@gitlab.com
```

