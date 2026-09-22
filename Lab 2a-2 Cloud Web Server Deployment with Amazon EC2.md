# 2a-2 Cloud Web Server Deployment with Amazon EC2

## Launching EC2 on AWS
In this lab, the main task is to use AWS to create a virtual machine and the rest will be describe through documentation.

First, we will launch EC2 from AWS, and make sure it's running.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 11 07 12 PM" src="https://github.com/user-attachments/assets/693b7e72-7339-45fb-893c-7030d38628a6" />


Then check inbound rules in security group.

<img width="1154" height="200" alt="Screenshot 2026-09-22 at 11 16 14 PM" src="https://github.com/user-attachments/assets/62c9e976-cf6c-4ab8-9fab-415d81f16aad" />


## Connect to EC2 using SSH 
<img width="1470" height="956" alt="Screenshot 2026-09-22 at 11 28 52 PM" src="https://github.com/user-attachments/assets/910769b1-f29f-4945-81f9-106795047380" />

## Apache Installation

If we enter  http://publicIPfromAWS before installing apache2 on mac terminal, the page will not load. Use bash **sudo apt update** **sudo apt install apache2** and press y, 
then check the status with **sudo systemctl status apache2** to see if it's running. If yes, http://publicIPfromAWS should work as shown in screenshot.
<img width="1470" height="956" alt="Screenshot 2026-09-23 at 12 01 34 AM" src="https://github.com/user-attachments/assets/40a5798c-b4a6-47d0-804b-4d33374f635a" />

After all the labs done, we should terminate or shut down the VM to save budget. 
<img width="1470" height="956" alt="Screenshot 2026-09-22 at 11 51 08 PM" src="https://github.com/user-attachments/assets/01b4c48b-316b-4ab9-9cea-9f3e685e0ae3" />
