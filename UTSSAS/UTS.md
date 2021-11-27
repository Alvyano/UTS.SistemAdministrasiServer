# UTS-Sistem Administrasi Server
Alvyano Rizqilla Riananta 1202190035 - IT0201
---
---
                            Question

![](Gambar\Pendahuluan.png)

Answer
---
---
```
A. Instalasi Windows Serever 2022
```
* Download ISO Installer Windows Server 2022

https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022

* Select download the ISO then follow it step by step.

![](Gambar/100.png)

* Open Oracle VM

![](Gambar/1.png)

* Then click New, and Enter the machine name and system type to use

![](Gambar/2.png)

* Define ram, create the disk defining type and size

![](Gambar/3.png)

![](Gambar/4.png)

![](Gambar/5.png)

![](Gambar/6.png)

![](Gambar/7.png)

* Go to the machine configuration and in the “Network” section set “Bridge adapter” 

![](Gambar/8.png)

* Click on Start and select the ISO downloaded

![](Gambar/9.png)

![](Gambar/10.png)


* Click on Start and the Windows Server 2022 installation wizard will load

![](Gambar/11.png)

* Click on Install now

![](Gambar/12.png)

![](Gambar/13.png)

* Select Windows Server 2022 desktop experience

![](Gambar/15.png)

* Accept the license and then proceed with the installation of Windows Server 2022

![](Gambar/17.png)

* Location installation of windows server 2022

![](Gambar/18.png)

* Installation Progress

![](Gambar/19.png)

* The system will reboot to complete the process

![](Gambar/20.png)

* Next, custom your password administrator

![](Gambar/21.png)

* Access the menu Input – Keyboard – Insert Ctrl + Alt + Del. Enter the password created and wait for the configuration to load

![](Gambar/22.png)

![](Gambar/24.png)

* Windows Server 2022 has been successfully installed

![](Gambar/29.png)

```
B. Instalasi Active Directory Domain Services
```
* Before doing the installation, we change the computer name first by going to windows powershell. Then type rename-computer -Newname Server2022

    * Open the start menu and select Windows PowerShell

![](Gambar/35.png)

* Then Restart, and openServer Manager

![](Gambar/31.png)

* Select menu manage, then add rules and features

![](Gambar/34.png)

* Select Next

![](Gambar/37.png)

* Select optionRole-based or feature-based installation. And next

![](Gambar/39.png)


* Click select a server from the server pool to select a local storage directory. Then next

![](Gambar/40.png)

* Next, put a check mark in the Active Directory Domain Services box. When you check the box, on the right appears a brief description of ADDS and how it works. Then click Add Features.

![](Gambar/41.png)

```
C. Instalasi DNS Server
```

* We need to install and configure the Active Directory role and DNS server to work together. Checklist DNS Servers then add features

![](Gambar/42.png)

```
D. Instalasi Net Framework 3.5
```
* Checklist .NET Framework 3.5 features

![](Gambar/43.png)

* Click Next

![](Gambar/44.png)

* Click Nextagain

![](Gambar/45.png)

* Select Install

![](Gambar/46.png)

* And Success

![](Gambar/48.png)

![](Gambar/49.png)


```
E. Promote Server to a Domain Controller
```

* Setting to static ip using cmd, type sconfig

![](Gambar/51.png)

* Choose Network Settings

![](Gambar/52.png)

* Setting the IP Address Server-ADDS and pointing the DNS to the static IP address used.

![](Gambar/53.png)

![](Gambar/59.png)

![](Gambar/61.png)

* Click Promote this server to a domain controller for ADD configuration

![](Gambar/63.png)

![](Gambar/64.png)

* Select Add a new forest and enter the domain name to be used in the Root Domain Name. For example here I use the domain Alvyano.com

![](Gambar/65.png)

* Select Windows Server 2016 at the functional level, put a check mark on Domain Name System (DNS) server and Global Catalog (GC). And fill in the Directory Services Restore Mode password with strong password criteria.

![](Gambar/66.png)

* Then click Next

![](Gambar/67.png)

* Fill in The NetBIOS domain name according to the domain name used.

![](Gambar/68.png)

* Skip the Paths section, click Next.

![](Gambar/69.png)

* Check the configuration specified in Review Options, if it is TRUE. Click Next.

![](Gambar/70.png)

* If there is All prerequisite checks passed successfully. Click Install to apply the specified configuration.

![](Gambar/71.png)

* After the installation is complete, the laptop will restart automatically. Then login using administrator password

![](Gambar/73.png)

![](Gambar/74.png)

![](Gambar/75.png)

* To check the configuration results, open cmd and type netdom query fsmo

![](Gambar/76.png)

![](Gambar/77.png)

* After logging in with the Active Directory Domain Controller, open the TCP/IP properties of your network connection. You can see the DNS server IP Address.

![](Gambar/78.png)
---
---
# FINISH 
