# How to create a Attack and Defense Cyber Security Lab

## Objective

The primary objective of this cybersecurity attack and defense lab is to create a safe, controlled, and realistic environment for developing, testing, and refining cybersecurity skills such as: reconnaissance, vulnerability analysis, exploitation, privilege escalation, and post-exploitation for Offensive Security and threat detection, log analysis, intrusion prevention, incident response, and system hardening for Defensive Security. This setup enables cybersecurity professionals, students, and enthusiasts to experiment with both offensive and defensive techniques without impacting production systems or violating ethical boundaries.

### Skills Learned

- Setting up and managing virtual machines (VMs) using platforms like VMware, VirtualBox, or Proxmox.
- Designing and configuring network topologies, including VLANs and subnets, for isolation and traffic control.
- Configuring guest operating systems such as Windows Server, Linux distributions (Kali, Parrot OS, RHEL), and specialized security tools.
- Understanding and implementing protocols such as TCP/IP, DHCP, DNS, and routing.
- Using tools like Wireshark to monitor and analyze network traffic.

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



  
