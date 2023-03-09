# WSL2-kali-setup | Windows 10 / Windows 11

In windows terminal
```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```
Output:
```
Deployment Image Servicing and Management tool
Version: 10.0.22621.1

Image Version: 10.0.22621.1265

Enabling feature(s)
[==========================100.0%==========================]
The operation completed successfully.

```
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
```
wsl --set-default-version 2
```
output:
```
For information on key differences with WSL 2 please visit https://aka.ms/wsl2
The operation completed successfully.
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
BOOM ur in
press F8 to disconnect

zsh update
```sudo apt install zsh*```
```chsh -s $(which zsh)```
Note: If you encounter any issues, you can always switch back to bash by running the command `chsh -s /bin/bash`.


## WSL HELP
```
wsl --help

Usage: wsl.exe [Argument] [Options]

Arguments:
  --list, -l              List the available distributions.
  --set-default <Distro>  Set the specified distribution as the default.
  --unregister <Distro>   Unregister the distribution.

Options:
  --import                Imports a distribution.
  --terminate             Terminates the specified distribution.
  --exec, -e              Execute a command in the specified distribution.
  --run, -r               Run the specified command in the specified distribution.
  --user                  Run as the specified user.
  --distribution, -d      Specifies the distribution to use.
  --help, -h              Displays this help message.
```

# Screenshots
--------------
![neofetch-wsl](https://user-images.githubusercontent.com/55411358/222261692-573bbe80-8ff3-4432-88f4-00abca11c8e9.png)
