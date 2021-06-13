## Task0: Environment Setup and Configuration

**I. Linux Setup: WSL or VMWare**

1. To enable Windows Subsystem for Linux, open PowerShell and run as adminstrator. Execute the following: 
```
  dism.exe /online /enable-feature/featurename: Microsoft-Windows-Subsytem-Linux /all /norestart
```

2. To enable virtual machine function, execture the following command: 
```
  dism.exe /online /enable-feature/featurename: VirtualMachinePlatform /all /norestart
```

Upon completion of above steps, simply reboot the computer for the system to be carried out.\
\
__II. Download the Linux kernel update package and Install Ubuntu__

1. Download the latest version release: [Download the Linux kernel update package!](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)
2. Set WSL2 as your default by running the following in PowerShell: 
```
wsl --set-default-version 2
```
3. Download a Linux distribution of your choice from Microsoft Stores: [Ubuntu 20.04 LTS!](https://www.microsoft.com/store/apps/9n6svws3rx71)
4. (Recommended) Download the latest release of Windows Terminal: [Windows Terminal!](https://docs.microsoft.com/en-us/windows/terminal/get-started)
5. Intialize username and password for WSL. \
\
__III. VSCode Installation and Configuration__

1. Download the latest version of VSCode. 
2. Install Remote-WSL extension. 
3. Create a connection to WSL from the green cursor on the bottown left and select `New WSL Windows`\
\
__IV. Installation of Python3 and Django__

1. To install Python3, open a Ubuntu Terminal and Execute 
```
sudo apt-get install python3
```
2. To install pip, execute the following:
```
sudo apt-get install python-pip
```
3. Intialize environment for Django: 
```
python -m venv django
```
4. Activate the virtual environment:
```
cd django && source bin/activate
```
5. Use pip to install Django
```
# Default install
pip install Django

# 国内请使用以下镜像源：
# Temporary Usage
pip install -i https://pypi.tuna.tsinghua.edu.cn/simple django

# Permenant Configuration
pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple/
```

6. Install VSCode extension for Django.
