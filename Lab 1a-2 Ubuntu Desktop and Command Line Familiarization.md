#Lab 1a-2 Ubuntu Desktop and Command Line Familiarization

In this section, I will make myself  familiarize with Ubuntu Desktop and basic command-lines tools, using them to navigate and work with 
various utilities.

## Ubuntu Desktop GUI Familiarization 

To check the internet suing Firefox, first, open the Firefox in the Ubuntu Application Menu. And then launch any website(eg. Wikipedia 
as shown in screenshot). If the page loads, that means the internet connection works.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 1 43 54 AM" src="https://github.com/user-attachments/assets/79d09d77-b8ca-42b5-b2ca-71ce4c664646" />
<br><br><br>

To explore through Ubuntu desktop environment if it works normally, we will try to use LibreOffice through website and type some words in the document.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 3 06 22 AM" src="https://github.com/user-attachments/assets/97c35ef4-67da-4b54-8d85-1879ed8900ba" />
<br><br><br>

We can also navigate directories using file manager.
-Open file on menu
-and go through the files

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 3 23 54 AM" src="https://github.com/user-attachments/assets/fce5f943-d121-4623-a942-6701823bd5c4" />
<br><br><br>

In the App Center,we can try to download a program. This screenshot will show downloading YouTube client for linux.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 3 31 39 AM" src="https://github.com/user-attachments/assets/420321c0-69b1-4445-8e0c-5e0c139a8aae" />
<br><br><br>


# CLI Basics and File Operations

We will go through some commands that are used for processes and CPU.

First, if we use bash **ps -e**, we will see a snapshot of processes running on Ubuntu such as PID — Process ID, TTY — Terminal associated with the process,
TIME — CPU time used, and CMD — Command/program name.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 3 49 33 AM" src="https://github.com/user-attachments/assets/c8349905-1c15-4485-af58-85859c345939" />
<br><br><br>


Then we will use bash **top** to see a live update of CPU. And then, if we press 1, we will see some changes such as overall to individual CPU lines.

Bash **top**
<img width="1470" height="956" alt="Screenshot 2026-09-22 at 3 48 50 AM" src="https://github.com/user-attachments/assets/0f516441-b00f-4c85-821d-26e38fc30be8" />

After pressing 1,
<img width="1470" height="956" alt="Screenshot 2026-09-22 at 3 49 11 AM" src="https://github.com/user-attachments/assets/7ff9a908-2765-4297-82b1-7ecaa85337db" />
<br><br><br>

Bash **ls** shows basic file lists while bash **ls -la** shows detail file lists including hidden files.
<img width="1470" height="956" alt="Screenshot 2026-09-22 at 12 02 00 PM" src="https://github.com/user-attachments/assets/b620b277-b9b2-4f0e-9bd0-386b34195bae" />
<br><br><br>

Now we will create a file using bash **touch testfile**. To edit, we will use bash **gedit testfile**, a separate window will appear opening the file in gedit. But if we 
use bash **nano testfile**, the file is opened inside the terminal. **gedit testfile** let us use menu, keyboard, mouse like a normal editor while **nano testfile**
makes us use a command line editor, which needs to use keyboard shortcuts to save and edit.

**gedit testfile**
<img width="1470" height="956" alt="Screenshot 2026-09-22 at 12 25 11 PM" src="https://github.com/user-attachments/assets/395a47fe-06ac-4d63-831a-bcde95bf4e09" />

**nano testfile** (keyboard shortcuts are shown below)
<img width="1470" height="956" alt="Screenshot 2026-09-22 at 12 26 32 PM" src="https://github.com/user-attachments/assets/3eb0aaec-e576-498b-a94d-1448f244f690" />

Now we will display the file using bash **cat testfile** and **less testfile**. Both commands are for displaying file, but **cat testfile** will display the entire file 
directly in the terminal. **less testfile** will open the file in scrollable viewer which is better for long files. **cat testfile** is more suitable for short file.

**cat testfile**
<img width="1470" height="956" alt="Screenshot 2026-09-22 at 12 38 50 PM" src="https://github.com/user-attachments/assets/e11920f4-6e5e-4fd1-92d2-ef9598d5eb38" />


**less testfile**
<img width="1470" height="956" alt="Screenshot 2026-09-22 at 12 38 24 PM" src="https://github.com/user-attachments/assets/4822b113-08dc-465f-b0e1-9e235ad34fee" />
<br><br><br>


Bash **uname -a** shows kernal and system information. Bash **lsb_release -a** shows information about the Linux distribution (Ubuntu).

<img width="739" height="193" alt="Screenshot 2026-09-22 at 12 48 34 PM" src="https://github.com/user-attachments/assets/76797ce6-62d3-46cc-bad2-2923c20ce5ae" />
<br><br><br>

Bash **hostnamectl** can be used to view or change the host name and related system information in Ubuntu.
<img width="487" height="372" alt="Screenshot 2026-09-22 at 12 55 10 PM" src="https://github.com/user-attachments/assets/9cd3ac2c-8114-4765-9e31-c25c3f7dabfa" />

Bash **ls -alt** also shows details about files, including the hidden files, but with modification time and minus the human-readable -h.
<img width="1470" height="956" alt="Screenshot 2026-09-22 at 12 57 47 PM" src="https://github.com/user-attachments/assets/fea7e804-1a45-4f98-9e5d-6ad460c8aaed" />
<br><br><br>

# Super User and Permissions 

In this section, we will learn about the differences of the commands that have different privileges level. If we use bash **whoami**, it will shows the current username 
as a regular user. But if we use bash **sudo whoami**, it will runs "whoami" with root privileges. When we try to add new user, using bash **adduser (name)**, it will not
allowed because we are just a user. But if we use bash **sudo adduser (name)**, it will allow us to add new user and starts the process. This is the difference between user and root.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 1 24 12 PM" src="https://github.com/user-attachments/assets/36d60993-f3a9-4282-b9c7-2eadfd5047dc" />
<br><br><br>

# Network Configuration and DNS 

In this section, we will learn about network configuration, public vs private IP, hosts and DNS.

First, we will use bash **ip a** to view network interfaces and IP addresses. Then we will use bash **ping 8.8.8.8** to test if the Ubuntu can connect with the internet. "8.8.8.8" is
a pubic IP created by Google for network connectivity testing. If we see "**64 bytes from 8.8.8.8: icmp_seq=1 ttl=117 time=20 ms**" that means VM is able to reach the IP address and receiving 
responds. Then use control+C to stop.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 1 44 57 PM" src="https://github.com/user-attachments/assets/4f9fe24f-24d4-4127-9ba7-e39a308232a6" />
<br><br><br>


If we want to avoid remembering IP addresses we can edit our own name by using bash **sudo nano /etc/hosts**. Then we will add " 8.8.8.8 GoogleEpicDNS" in a black space of the terminal and save the 
file. Then use **ping GogleEpicDNS** to see whether the hostname is resolved and communicate with the IP address we just added.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 2 06 26 PM" src="https://github.com/user-attachments/assets/615900b3-6e89-4487-b25c-09636e6d5074" />
<br><br><br>


We will use google to check DNS and domain information by using bash **nslookup google.com**

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 2 30 44 PM" src="https://github.com/user-attachments/assets/73db82b2-e808-423a-92c5-126cc1cf6a46" />
<br><br><br>


But if we wanna check the domain registration information, we have to install whois program with bash **sudo apt install whois**. Then we can check Google's domain registration information with bash **whois google,com**.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 2 35 00 PM" src="https://github.com/user-attachments/assets/264e1098-b2d1-41b4-90af-de9f98bf4bf0" />
<br><br><br>


Bash **ip a** shows our private IP address. So, to check our public IP address we can use whatismyipaddress.com.

<img width="1456" height="878" alt="Screenshot 2026-09-22 at 2 40 42 PM" src="https://github.com/user-attachments/assets/340f159c-baa6-4c83-b64e-2ec9864bb151" />
<br><br><br> 


# System and Hardware Info

This section is hardware related commands.Bash **lsusb**  displays information about USB devices connected to the system. Bash **lspci*8 displays PCI devices detected by the system, such as network, graphics, 
and audio controllers.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 2 50 05 PM" src="https://github.com/user-attachments/assets/70d55479-24ba-44c0-9a67-5bfac3955ab3" />
<br><br><br>


Bah **less /proc/cpuinfo*8  displays detailed information about the CPU in a scrollable format.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 2 49 16 PM" src="https://github.com/user-attachments/assets/864ab30c-d8df-40ab-9a1e-6b59f59cbb56" />
<br><br><br>


# Software Installation Methods 

In this section, I'll try to install a software using bash **sudo apt install (software name)**.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 3 02 44 PM" src="https://github.com/user-attachments/assets/75eaee92-163e-45f2-8025-628667ffe217" />
<br><br><br>


# Reflection

From this lab, I've learned a lot of commands and privileges in commands. 

