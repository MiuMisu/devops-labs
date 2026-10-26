# LAB 00

 ## Step 1. Run Linux by QEMU/KVM. 
    Sudo apt update 
    Sudo apt install qemu-system-x86 virt-manager libvirt-daemon-system libvirt-clients bridge-utils virtinst

    sudo usermod -aG libvirt $USER
    sudo usermod -aG kvm $USER
    sudo systemctl enable --now libvirtd

    {Reboot}

## Step 2. Create Lab-rep
    2.1 Create connection and preparation
    Git init for initialization
    Git remote add origin <URL> - bound to network

## Step 3. Hello Git! (Solution a proplem "Who are you?")
    3.1 Git config --global <user.email> and <user.name> 

## Step 4. Locking structure of folders
 Face with the folders aren't show
    4.1 Creation the files ,gitkeep
    find . -type d -empty -not -path './git*' -exec touch {}/.gitkeep \;

## Step 5. Git add
    git commit -m "name"

## Step 6. Sending to NET
    git push -u origin main
 send my save files to the rep. origin in the branch main. I bounded a local branch with cloud. 

## Step 7. Create .gitignore
    7.1 echo .env > .gitignore
Hiding secrets ;1)
