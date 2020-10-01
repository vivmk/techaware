---
title: "How to install Kali Linux on Windows 10 through WSL"
date: 2020-09-13T19:49:57+05:30
draft: false
---

The Windows Subsystem for Linux lets developers run a GNU/Linux environment -- including most command-line tools, utilities, and applications -- directly on Windows, unmodified, without the overhead of a traditional virtual machine or dual-boot setup.

### Installing WSL

Before we get started, update your machine. You need to be running on Windows 10 version 1903 build 18362 or higher.

#### Method I - Using GUI

Search for (windows key + S) `Windows Features` in your PC and check the `Windows Subsystem for Linux` and `Virtual Machine Platform` options ticked.

![Windows Features](https://www.linkpicture.com/q/Screenshot-103.png)

Now restart your machine.

#### Method II - Using Powershell

Open PowerShell as an Administrator and run the following commands:

---

To enable Windows Subsystem for Linux:

`dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart`

Now restart your machine.

---

To enable Virtual Machine Platform:

`dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart`

Restart your machine again.

---

To set WSL2 as your default version:

`wsl --set-default-version 2`

---

### Installing Kali

Download and Install Kali from the [Microsoft Store](https://aka.ms/wslstore). Open the installed app from the Start menu. Add a new User and set up a Password as shown in the screenshot below -

![Kali on Windows 10](https://www.linkpicture.com/q/Screenshot-108.png)

You are halfway there, you have successfully installed kali using WSL.

### Configuring Kali (Setting up a GUI)

Now let us Install the Desktop Environment (win-kex).
Open Kali terminal and run the following commands:

---

To update the Kali repositories:

`sudo apt update`

---

To install the updates available for Kali:

`sudo apt upgrade`

---

To install the win-kex (Kali Desktop Experience for Windows):

`sudo apt install kali-win-kex`

---

Note: If you get error while installing `kali-win-kex` then make sure you have enabled `Virtual Machine Platform` and are using Kali in WSL2 and not WSL1.

![Trubleshoot](https://www.linkpicture.com/q/Screenshot-135.png)

Now, run the command `kex` to install the GUI. It takes sometime. After it is installed, you can press F8 key to open VNC options and exit full screen!

Congrats! You have Kali up and running:

![Kali on windows 10](https://www.linkpicture.com/q/Screenshot-130.png)

If you want to install complete Kali, you can do so by running the command `sudo apt install kali-linux-large`. This step is optional. You can do it if you need it and have enough space.
