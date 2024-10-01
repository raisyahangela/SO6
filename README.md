# How to Install and Configure SSH on Ubuntu 22.04

**NAMA : RAISYAH MEPA ANGELA
NIIM : 09011282328033
KELAS : SK3C
MATA KULIAH : PRAKTIKUM SISTEM OPERASI**


**How to Install and Configure SSH on Ubuntu 22.04**

**Step 1: Prepare Ubuntu**

sudo apt update && sudo apt upgrade

![Step 1](1.png)

**Step 2: Install SSH on Ubuntu**

sudo apt install openssh-server

![Step 2](2.png)

**Step 3: Start SSH**

Now you need to enable the service you just installed using the command below:

**sudo systemctl enable --now ssh**

![Step 3a](3.png)

To verify that the service is enabled and running successfully, type:

**sudo systemctl status ssh**

![Step 3b](4.png)

If you want to disable the service, execute: 

**sudo systemctl disable ssh**

![Step 3c](5.png)

**Step 4: Configure the firewall**

Before connecting to the server via SSH, check the firewall to ensure it is configured correctly.
In our case, we have the UFW installed, so we will use the following command:

**sudo ufw status**

![Step 4](6.png)

**Step 5: Connect to the server**

Once you complete all the previous steps, you can log into the server using the SSH protocol.
To do this, you will need the server's IP address or domain name and the name of a user created on the server.
In the terminal line, enter the command:

**ssh username@IP_address**

![Step 5](7.png)

Selanjutnya, masuk ke view network connection, pilih Ethernet, klik properties, ke internet protocol version 4 lalu buka propertiesnya dan atur IP_Address nya.

![Network Config 1](8.png)

![Network Config 2](9.png)

Lalu, kita bisa beralih ke command prompt dan memastikan jaringan terhubung dengan cara mengeceknya.

![Network Check](10.png)

Selanjutnya adalah membuka Powershell dan memasukan perintah ssh -p 2222 username@IP_Address.

![SSH Connection](11.png)

Terakhir, adalah memberi perintah ls untuk mengecek dan perinta neofetch untuk memastikan data yang ada didalamnya.

![ls Command](12.png)

![neofetch Command](13.png)
