# **1a-1 Virtualisation & Linux Setup**

This is about setting up a Linux environment.

To set up a Linux environment,as a MAC user, I downloaded UTM for the hypervisor and Ubuntu for LOS. This is a screenshot of successfully downloading Ubuntu on UTM,
showing terminal of the Ubuntu.

<img width="1470" height="956" alt="Screenshot 2026-09-21 at 11 13 25 PM" src="https://github.com/user-attachments/assets/da58d401-2997-4001-91c9-3bf037e5c623" />
<br><br><br>


This screenshot shows the details of my VM. "Shared Network(virtio-net-pci)" is the same network configuration as NAT in VirtualBox.
<img width="1470" height="956" alt="Screenshot 2026-09-21 at 11 22 02 PM" src="https://github.com/user-attachments/assets/a35644f7-f63b-4271-af94-9d4b73cd9ead" />
<br><br><br>

This is the screenshot of the terminal window(CLI) to confirm that OS is operational.

<img width="1470" height="956" alt="Screenshot 2026-09-21 at 11 48 24 PM" src="https://github.com/user-attachments/assets/af75691a-d836-48b0-a06c-53d94f5402fb" />
<br><br><br>

SSH Enabled <br>
-sudo apt update <br>
-sudo apt install openssh-server<br>
-the y for y/n <br>
SSH is active(running) <br>
-q for quit

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 12 02 13 AM" src="https://github.com/user-attachments/assets/74a8998d-f281-4931-91cb-4f472b244f5e" />
<br><br><br>

# Reflection

## Advantages of Virtual Machine

To test and develop Linux environment as a Student, creating a virtual machine is really helpful as it provides an isolated environment
without replacing the main operation system. A lot of operation systems can be run on the same computer, making it easier to test applications
across different environments. And virtual machines can be easily created and deleted, helping testers to make experiments easily.

## Difficulities

As a MAC user, except having to find the right software and version that support ARM-based M-chips, the setup and the rest was easy.



