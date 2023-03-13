## How to Install Kali Linux in Windows Subsystem for Linux (WSL)

### Step 1: Enable WSL in Windows 10

To enable WSL in Windows 10, open PowerShell as an administrator and run the following command:
```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

### Step 2: Install WSL

To install WSL, open a new PowerShell window as an administrator and run the following command:

```
wsl --install
```

### Step 3: Set WSL 2 as Default

To set WSL 2 as the default version of WSL, open PowerShell as an administrator and run the following command:

```
wsl --set-default-version 2
```

### Step 4: Install Kali Linux

To install Kali Linux, run the following command in a PowerShell window:

```
wsl --install -d kali-linux
```

### Step 5: Install Kali Linux Desktop Environment (Optional)

To install the Kali Linux desktop environment (XFCE), run the following command:

```
sudo apt install kali-win-kex -y
```

### Step 6: Start Kali Linux Desktop Environment (Optional)

To start the Kali Linux desktop environment (XFCE), run the following command:

```
kex --win -s
```

### Step 7: Install Zsh Shell (Optional)

To install the Zsh shell, run the following command:

```
sudo apt install zsh*
```

### Step 8: Set Zsh as the Default Shell (Optional)

To set Zsh as the default shell, run the following command:

```
chsh -s $(which zsh)
```

### Step 8: If you have the space, why not install “Kali with the lot”? (Optional)

Here, run the following command:

```
sudo apt install -y kali-linux-large
```

That's it! You should now have Kali Linux installed in WSL with optional GUI and Zsh shell support. Your computer has now become a lethal weapon! 💣🚀💥
