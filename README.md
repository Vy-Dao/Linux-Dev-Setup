# Linux-Dev-Setup

## Essential stuff
**Check and Install Package Updates**
```
sudo apt-get update && sudo apt-get dist-upgrade
sudo apt update && sudo apt dist-upgrade
```
**Installing curl, make, vim, npm**
```
sudo apt install curl make vim npm
```
**Git Set-up**
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


**Zsh - Oh-my-zsh**
```
apt install zsh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
sudo chsh -s $(which zsh) $(whoami)
https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md
https://github.com/zsh-users/zsh-syntax-highlighting/blob/master/INSTALL.md
```
**Java**
```
sudo apt install openjdk-8-jdk 
sudo apt install openjdk-11-jdk
java -version
```
**Installing yarn**
```
sudo apt update && sudo apt install yarn
```
**Node.js Current Version**
```
curl -fsSL https://deb.nodesource.com/setup_current.x | sudo -E bash -
sudo apt install -y nodejs
```
## Tools
**Visual Studio Code**
```
https://code.visualstudio.com/download
```
**Android Studio**
``
https://developer.android.com/studio/index.html#downloads
sudo apt-get install libc6:i386 libncurses5:i386 libstdc++6:i386 lib32z1 libbz2-1.0:i386
https://developer.android.com/studio/install#linux
Android Studio -> Tools -> Create Desktop Entry

``
**VLC**
```
sudo snap install vlc
sudo apt install ubuntu-restricted-extras
```
**Additional Archive Utilities**
```
sudo apt install rar unrar p7zip-full p7zip-rar
```

## React Native Setup
```
https://reactnative.dev/docs/environment-setup
```
