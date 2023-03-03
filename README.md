# Personal Linux setup

> **Change the look and add some extra essential packages**
1. If installed on virtual machine
    - `sudo apt install build-essential dkms linux-headers-$(uname -r)`
    - For ubuntu 22.04 lts
        - After above command insert the guest addition cd and hit below commands
        - `cd /media`
        - `sudo ./VBoxLinuxAdditions.run`
        - Restart the VM
2. Media codecs
    - `sudo apt install ubuntu-restricted-extras`
3. Load frequently used apps faster
    - `sudo apt install preload`
4. Add gnome tweak tools
    - `sudo apt install gnome-tweaks`
5. Numix Theme and Icons
    - `sudo add-apt-repository ppa:numix/ppa`
    - `sudo apt-get update`
    - `sudo apt-get install numix-gtk-theme numix-icon-theme-circle`

> **Change some default softwares**
1. Install zsh (refer https://youtu.be/Vj54klRlwIE)
    - sudo apt-get update
    - sudo apt-get install zsh
    - sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    - Restart terminal
    - chsh -s $(which zsh)
    - Restart the machine
