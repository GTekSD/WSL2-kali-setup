# WSL2-kali-setup | Windows 10 / Windows 11

In windows terminal
```
wsl --install
```
Output:
```
Installing: Virtual Machine Platform
Virtual Machine Platform has been installed.
Installing: Windows Subsystem for Linux
Windows Subsystem for Linux has been installed.
Downloading: WSL Kernel
Installing: WSL Kernel
WSL Kernel has been installed.
Downloading: GUI App Support
Installing: GUI App Support (Win11 only)
GUI App Support has been installed .
Downloading: Ubuntu
The requested operation is successful.
Changes will not be effective until the system is rebooted.
```
Next
```
wsl --list
```
Output:
```
Windows Subsystem for Linux Distributions:
Ubuntu (Default)
```

install kali
```
wsl --list --online
```
Output:
```
The following is a list of valid distributions that can be installed.
Install using 'wsl --install -d <Distro>'.

NAME            FRIENDLY NAME
Ubuntu          Ubuntu
Debian          Debian GNU/ Linux
kali-linux      Kali Linux Rolling
openSUSE-42     openSUSE Leap 42
SLES-12         SUSE Linux Enterprise Server VI 2
Ubuntu-16.04    Ubuntu-16.04   
Ubuntu-18.04    Ubuntu-18.04
Ubuntu-20.04    Ubuntu-20.04
```

Install from CLI or MS Store
```
wsl --install -d kali-linux
```

Update before installing KEX
```
sudo apt-get update
```

Install kex
```
sudo apt install kali-win-kex -y
```
Installing Other Linux apps
```
sudo apt install gimp -y
```


For Windows 10. Setup Kex
```
kex --win -s
```
Enter password
```
Password :
Verify :
Would you like to enter a view-only password (y/ n)?
```
Hit `n`
