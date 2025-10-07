# Basic-Home-Lab
A Step-by Step guide on how to make a standard home lab for testing security tools and analyzing malware
# What is a Home Lab?
A home lab is a personal, at-home computing environment used for experimenting with and learning about various technologies. It's a space where individuals can safely explore software, networking, and hardware without the fear of affecting production systems. Home labs can range from simple setups on a single computer to more complex arrangements mimicking business environments. 


# Purpose of the Project
This write-up demonstrates how to build a basic home lab that can be tailored to the owner's specifications. Using the software VirtualBox, a Windows 10 ISO, and a Kali Linux ISO, 2 virtual machines (VMs) can be made and configured to communicate with each other on a private network. As well as being used for testing security tools and malware analyisis.


# Software and Hardware Needed
* VirtualBox
* Windows 10 ISO
* Kali Linux (Prebuilt VirtualBox Version)
* 7zip
* 4 GB of RAM
* 50 GB Disk Space



# Step-by-Step Guide:

Step 1: Download VirtualBox

Download and install VirtualBox at: https://www.virtualbox.org/wiki/Downloads

Download the platform for the computer that you are using. In this project, I will be using the Windows version. Once downloaded, follow the installation steps, and once finished, VirtualBox should autorun. If not, simply double-click the shortcut.
<img width="1913" height="976" alt="Screenshot 2025-08-08 172008" src="https://github.com/user-attachments/assets/c7c8da43-6d18-41a4-8cdc-e88ec08fdb98" />
<img width="1131" height="676" alt="Screenshot 2025-08-08 173106" src="https://github.com/user-attachments/assets/6b20d018-8a03-488c-b8cb-b0f4eca8179f" />








# Step 2: Download Microsoft Windows 10 ISO

You can go to https://www.microsoft.com/en-us/software-download/windows10 and under the tab that says Create Windows 10 installation media, click Download Now, create a folder for your home lab, and save the file there. 
<img width="1185" height="977" alt="Screenshot 2025-08-08 175635" src="https://github.com/user-attachments/assets/e27bb8c7-5464-4103-af4e-3ac03d4e2d3b" />




Then open the file, accept the user agreement, and select Create installation media. 
<img width="757" height="607" alt="Screenshot 2025-08-08 173806" src="https://github.com/user-attachments/assets/c0f715b5-fb38-433c-a755-728bf35f6e11" />
<img width="777" height="592" alt="Screenshot 2025-08-08 173905" src="https://github.com/user-attachments/assets/f8d6d2f8-1a78-4488-95fd-410ef83b256c" />







Select the language of your choice, and leave everything else default, and click next. Lastly, select the ISO file and save it to your HomeLab folder.

<img width="775" height="605" alt="Screenshot 2025-08-08 173941" src="https://github.com/user-attachments/assets/a82a7e99-839c-4bff-8817-439b2ba5bd7c" />
<img width="933" height="409" alt="Screenshot 2025-08-08 174229" src="https://github.com/user-attachments/assets/ed9e5255-f8a1-4cca-81be-4a764170cb47" />






# Step 3: Download Kali Linux

Go to Kali Linux at: https://www.kali.org/get-kali/#kali-platforms 
Click on the virtual machine option and download and save the VirtualBox file to the HomeLab folder. Note that the default username and password are both: kali
<img width="1656" height="982" alt="Screenshot 2025-08-08 174450" src="https://github.com/user-attachments/assets/1dc81214-0165-40f0-9b7a-3adbaa43c746" />
<img width="1804" height="933" alt="Screenshot 2025-08-08 174704" src="https://github.com/user-attachments/assets/a17dc499-42fc-4d2c-b3b4-bc6c678f36a2" />



# Step 4: Create a Windows VM

Go to VirtualBox and select New, name your home lab, in this example, I named mine: homelab1. For ISO image, select the Windows ISO we downloaded in the home lab folder. Leave everything else under this tab as the default.
<img width="1035" height="582" alt="Screenshot 2025-08-08 175957" src="https://github.com/user-attachments/assets/c7ada56b-51bd-49a7-be1b-23fd7d1978f5" />
<img width="1039" height="638" alt="Screenshot 2025-08-08 180258" src="https://github.com/user-attachments/assets/90c2fe44-8771-481c-9861-22695660339d" />



Select the Hardware tab and set the base memory to 4GB. Leave everything else as the default. (Note: You can choose to go higher depending on how much available memory your host computer has. But for this basic example, 4GB will be enough.)
<img width="1034" height="660" alt="Screenshot 2025-08-08 180411" src="https://github.com/user-attachments/assets/4c740d9d-9fef-4e57-b5db-d314f1488d24" />



Select the Hard Disk tab next and ensure that the disk space is set to 50GB. Then click finish.
<img width="873" height="617" alt="Screenshot 2025-08-08 180448" src="https://github.com/user-attachments/assets/d0fbbf60-2999-4d4a-ace2-d6082f88aba2" />


Select the homelab you created and hit Start.
<img width="1045" height="642" alt="Screenshot 2025-08-08 180558" src="https://github.com/user-attachments/assets/13a974fc-13ef-4af0-910f-c3a4ae5dddc2" />


Once it is started, you should see the setup screen. Click on Next, Install Now, and the 2nd screen.
<img width="1102" height="894" alt="Screenshot 2025-08-08 180729" src="https://github.com/user-attachments/assets/5981c78b-cff6-4c0b-9b12-67e402e3e6e7" />
<img width="1116" height="890" alt="Screenshot 2025-08-08 180748" src="https://github.com/user-attachments/assets/f8f1a530-9468-4653-a8b5-1db64a957531" />



For the active Windows screen, select “I don’t have a product key” and select “Windows 10 Pro” for the operating system.
<img width="1112" height="894" alt="Screenshot 2025-08-08 180811" src="https://github.com/user-attachments/assets/097ed939-622b-449e-8560-b223443d1973" />
<img width="1064" height="884" alt="Screenshot 2025-08-08 180916" src="https://github.com/user-attachments/assets/2821953a-ff6e-4d21-b1e9-af75da4e8a84" />


Accept the license terms on the next screen and select “Custom: Install Windows only” and then select the drive, and wait ‘til Windows is installed. Once finished, follow the steps to set up your Windows homelab account until you get to the homescreen.
<img width="1107" height="892" alt="Screenshot 2025-08-08 181020" src="https://github.com/user-attachments/assets/4002f125-031d-46bd-94f4-32710d7f67bc" />
<img width="1088" height="887" alt="Screenshot 2025-08-08 181115" src="https://github.com/user-attachments/assets/ee3b473e-9323-4e2a-9b77-591e23741953" />
<img width="1090" height="910" alt="Screenshot 2025-08-08 181226" src="https://github.com/user-attachments/assets/674a3fa3-ce68-4d9a-842e-b34eeb57b6ed" />


(Do NOT link your personal account to the homelab. Make sure to select “Offline account” and “limited experience” when you get to those screens.)
<img width="1109" height="886" alt="Screenshot 2025-08-08 182213" src="https://github.com/user-attachments/assets/49668184-fc12-4c69-a9c9-e84e87a4b0b1" />
<img width="1122" height="897" alt="Screenshot 2025-08-08 182302" src="https://github.com/user-attachments/assets/7240cd6a-1cdb-49f5-8749-c3b75e4e527d" />


After you set up your offline account and are at the homescreen, shut down the VM.


# Step 5: Create Kali VM 

Click on the Kali Linux archive and go to the 7-Zip option, and select “Extract kali-linux-2025.2-virtualbox-amd64.” (If you have Windows 11, select Show more options to see the drop-down menu.)
<img width="986" height="607" alt="Screenshot 2025-08-08 182803" src="https://github.com/user-attachments/assets/90a3508f-22ce-4f56-a3db-81dc0c0e376a" />
<img width="669" height="592" alt="Screenshot 2025-08-08 182602" src="https://github.com/user-attachments/assets/ee03075a-81df-41f5-9805-f99e777b5f17" />




Go into the folder and double-click the Kali Linux. Make sure it is the machine definition and not the disk image. Then, go to VirtualBox and Kali Linux will appear.
<img width="666" height="69" alt="Screenshot 2025-08-10 111933" src="https://github.com/user-attachments/assets/ed11ff88-779d-4d28-b90f-cf44de02a687" />
<img width="1065" height="604" alt="Screenshot 2025-08-08 183540" src="https://github.com/user-attachments/assets/66926f5d-84c5-42b2-acb0-19b3965ccc0d" />

Run Linux and make sure it is installed correctly. Remember, the default username and password are: kali
