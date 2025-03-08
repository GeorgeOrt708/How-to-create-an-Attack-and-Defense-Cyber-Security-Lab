# 📀How to create a Attack and Defense Cyber Security Lab

## Objective

The primary objective of this cybersecurity attack and defense lab is to create a safe, controlled, and realistic environment for developing, testing, and refining cybersecurity skills such as: reconnaissance, vulnerability analysis, exploitation, privilege escalation, and post-exploitation for Offensive Security and threat detection, log analysis, intrusion prevention, incident response, and system hardening for Defensive Security. This setup enables cybersecurity professionals, students, and enthusiasts to experiment with both offensive and defensive techniques without impacting production systems or violating ethical boundaries.

### Skills Learned

- Setting up and managing virtual machines (VMs) using platforms like VMware, VirtualBox, or Proxmox.
- Designing and configuring network topologies, including VLANs and subnets, for isolation and traffic control.
- Configuring guest operating systems such as Windows Server, Linux distributions (Kali, Parrot OS, RHEL), and specialized security tools.
- Understanding and implementing protocols such as TCP/IP, DHCP, DNS, and routing.

### Tools Used

- Windows Media Creation Tool
- Virtual Box
- Kali Linux VM ISO's


## Download VirtualBox
  
You will need to download a virtualization software otherwise known as a Hypervisor such as VMware, Hyper-V, or even Virtualbox. For this Lab, we will be using VirtualBox. Download whatever version of Virtualbox fits your current OS using the following link: https://www.virtualbox.org/wiki/Downloads.
![image](https://github.com/user-attachments/assets/971d842a-ff91-4a57-9247-3f396de514c0)

You can customize settings such as where the software will be downloaded to if you have multiple drives, but the defaults work perfectly fine

![image](https://github.com/user-attachments/assets/10f9824d-d31e-4063-bc3a-9b09efa89668)


## Downloading your Windows Virtual Machine.
### For the Windows VM you will need to create a windows OS Image. The safest way to do so will be to create our own via the following link: https://www.microsoft.com/en-ca/software-download/windows10

Once you reach this page you will need to scroll down and click "Create Windows 10 installation media"

![image](https://github.com/user-attachments/assets/6e10f8b2-77fc-4f15-aecb-cf7b1f1a499f)

During the setup process you will be asked to either:

 - Upgrade this PC now
 
 - Create Installation Media (USB flash drive, DVD, or ISO file) for another PC

 Select "Create Installation Media"
 
 ![image](https://github.com/user-attachments/assets/ebc89575-64cc-4272-a91e-25463c822fa2)

You may customize or use the recommended settings for your pc. I recommend using the default settings.

After that you prompted with the option of either:

- USB Flash Drive

- ISO File

Choose ISO File.

Once the ISO File is installed you can go ahead and open Virtual Box.

With Virtual Box open you will want to choose the option "New"

![image](https://github.com/user-attachments/assets/ecce861f-b0da-43e6-a128-f8d33a99b0fe)

Here you will be able to name your Virtual machine, choose where the VM files will be located, etc.
In the row: " ISO Image" click the drop down arrow and select "Other". From here find the Windows ISO file you downloaded previously and select it

![image](https://github.com/user-attachments/assets/9f355125-22ba-4646-b0f2-65702af4e05b)

Virtualbox will automatically detect that you are using a Windows OS and fill in the Type and Version information. Underneath those you will see the option to "Skip Unattended Installation".

You will want to select this as it will allow you to manually install the OS. If you would rather it be down automatically you can leave it unselected.

From here you will be prompted to setup the amount of Memory and CPU usage you want the VM to take. This will depend on your devices capabilities, but for now we will be using 4 GB of RAM (4096 MB) and 1 CPU Core

![image](https://github.com/user-attachments/assets/05d528f2-6fa7-401d-9496-2349aab54da4)

Next you will need to allocate a "Virtual Hard Disk" Size to the machine. For this Lab we can leave it at the default of 50 GB's

![image](https://github.com/user-attachments/assets/b4fa79ea-be7a-44d3-b73e-13288dc2175f)

When you reach the Summary page click "Finish"

At this time you can start your new Windows VM and setup Windows

Once the machine launches you'll be prompted to change your Install Language, Time Format, etc. You can leave this default and click "Next" and "Install Now" afterwards.

![image](https://github.com/user-attachments/assets/4c03494a-fb74-4fc4-a8c8-f5ebf1da5a90)

When prompted to "Activate Windows" Click "I dont have a product key" on the bottom

![image](https://github.com/user-attachments/assets/1e48ad8d-6e47-4450-bdbd-8be0f818b707)

Then select Windows 10 Pro as your OS option.

![image](https://github.com/user-attachments/assets/286ba59c-b98e-4839-ac0e-6a3d52f1cbb0)

After this you will be asked to Accept the License Terms. Click I accept.

![image](https://github.com/user-attachments/assets/d4b4cffd-4043-4847-8292-9f1fae308e16)

When asked what type of installation you want choose "Custom" to Install Windows Only.

![image](https://github.com/user-attachments/assets/832af7c0-3cbf-4c8f-90d9-16422d9d49ec)

Finally, you will be prompted with a place to install Windows. Choose Drive 0 and hit "Next" and allow Windows to install fully.

![image](https://github.com/user-attachments/assets/a83019f1-e868-4307-b114-c898e1017db5)

  ## Download Kali Linux Virtual Machine

For the Kali Linux VM you will want to visit: https://www.kali.org/ and click Download

![image](https://github.com/user-attachments/assets/c6c0ad9f-fc39-4660-9ce1-b8583c033d14)

Here you'll see multiple different options to download Kali. For now we will be choosing the Virtual Machine option as these provide pre-built images for VMWare and Virtualbox.

![image](https://github.com/user-attachments/assets/73411058-8392-4e72-ab6a-4693a7a697b7)

From here Select the VirutalBox Option and begin the download

![image](https://github.com/user-attachments/assets/d26ef825-e023-472f-9d29-c82b540edadb)

Due to this being a 7-Zip file you will need to install 7zip.

To do so navigate to the following website: https://7-zip.org/

Once here click the Download button that fits whatever version of Windows you have. In this case x64 or 64 bit

![image](https://github.com/user-attachments/assets/e0c2af1b-3eb6-40da-bb6d-311851a800af)

If your not sure what version you currently have simply go to the Windows Search button on the bottom left of your screen and type in "System Information"

Here you will see all the information on your current machine including your "System type which tells you what version of Windows you have.

![image](https://github.com/user-attachments/assets/240837f9-7a2d-4a36-996b-7ee2b4f9876e)

Now with 7-Zip installed you can go to the Kali Linux file you downloaded and extract the file via 7-Zip

![image](https://github.com/user-attachments/assets/bf7f7bdd-a80b-4751-92dc-fd80c7c714c3)

Once the file is extracted you will need to enter the kali-linux virtual box folder.

Here you will see two files. Double click the file with the .vbox extension and it will automatically be imported to the virtual box menu.

![image](https://github.com/user-attachments/assets/b53294d8-0600-44f8-9362-07844784ba38)

If you cannot see the .vbox extension then click view on the top of the file explorer options and select file name extensions.

![image](https://github.com/user-attachments/assets/12182e7e-c1d2-4fc2-aee6-1b526bcba8fd)

## Network Configuration

### This is one of if not the MOST important step when it comes to malware analysis as improper network configuration can lead to you damaging or destroying your host machine and any others on the network.

For this lab we will be using an internal network topology as this will not allow any external communications to our host or internet as shown below

![image](https://github.com/user-attachments/assets/e42c6361-5575-4ea9-bf59-e8ac646a9ed6)

More information on the different network types can be found in this document from VirtualBox: https://www.virtualbox.org/manual/ch06.html

In order to set these VM's to internal network mode we will need to launch virtualbox, click either of the VM's, click settings and click network.

Here we will see the option to change our network adapter and what it is attatched to. Select Internal Network and provide a name for the network. Repeat these steps for the second machine

![image](https://github.com/user-attachments/assets/5c042b40-fff2-43ff-bb23-33066932569b)

Due to the nature of an internal network we will need to statically (Manually) assign an IP address to each device so that they can communicate with each other.

Launch the Windows machine first. In the bottom right corner you will need to right click the globe icon and select "Open Network and Tnternet Settings".

![image](https://github.com/user-attachments/assets/14c6545c-49e0-45a6-9483-006755e20702)

Scroll down until you see change adapter options. This will open a window called "Network Connections". There will be an option called Ethernet. Right click it and hit "Properties"

![image](https://github.com/user-attachments/assets/97fd8cc7-8891-4144-abef-1f7f79650cbe)

A list of connections will appear before you. Double click "Internet Protocol Version 4 (TCP/IPv4)"

![image](https://github.com/user-attachments/assets/1f917cfa-d7b8-4fe4-8d55-3e77bdd938c1)

By default it will be set to obtain an IP automatically, but we want to switch this to "Use the following IP address"

The IP we will be using for the Windows machine is: 192.168.20.10

The subnet mask will be 255.255.255.0 and we will not be using a DNS Server.

Once finished it should look like this:

![image](https://github.com/user-attachments/assets/3f418006-b987-4ddf-a310-5a313697491c)

Once this is done hit "Ok" and close the window. To ensure we properly set up the new IP Address we can open a cmd prompt and type the cmd: ipconfig

![image](https://github.com/user-attachments/assets/01f34dd1-0036-47ac-b423-7899e1ce2a00)

Now that this is complete we want to do the same thing for the Kali machine

Open your kali machine with the default credentials (kali, kali) and go to the ethernet port icon located in the top right of the page.

Right click the icon and select "Edit Connections"

![image](https://github.com/user-attachments/assets/5fb395bc-93e9-414e-9a65-b15d1233cda7)

Click "Wired Connection 1" and then hit the gear icon on the bottom left

![image](https://github.com/user-attachments/assets/b68dbfb2-a03c-4fca-898e-89f8349befcd)

From here select IPv4 Settings and switch from automatic DHCP to Manual.

After that we will click Add and Enter the following IP: 192.168.20.11 and for Netmask: 24.

![image](https://github.com/user-attachments/assets/603741cb-5436-4c06-9d18-b0664385f6cd)

Now hit Save and close the page.

Now to test we will be doing the same as with the Windows Machine.

Right click anywhere on the screen and hit "Open Terminal Here"

The cmd for Linux is slightly different to check your IP: ifconfig

![image](https://github.com/user-attachments/assets/341655c8-87cd-4a85-b2bd-e4258066bf6f)

Now that these VM's have both their IP's set up we can test and see if they are able to communicate with each other by using the ping cmd.

Ensure that both machines are currently online and type in the following cmd in your windows cmd terminal: ping 192.168.20.11

![image](https://github.com/user-attachments/assets/d193884c-14d3-43f7-928b-7ad3503f6096)

# Congratulations!

You have successfully created an attack and defense lab that will allow you to test all kinds of different malware and anti malware techniques.

This is only the beginning of your journey so make sure to keep learning and trying new things!

Thanks for joining me!
