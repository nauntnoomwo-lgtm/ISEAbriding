# 1b-2 Linux File Permissions and Group Access Control 

## Creating Users
First, we will add three users called Alice, Bob and Mallory bu using bash **sudo adduser NAME**.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 7 46 25 PM" src="https://github.com/user-attachments/assets/c1ff215f-74b9-4de5-9615-d3b624ff052c" />
<br><br><br>

## Creating Group
Then, we will create a group with **sudo groupadd sharedgroup** and add the three users to the group with the command **sudo usermod -aG sharedgroup USERNAME**.
(I messed up using bash **sudo usermod -aG USERNAME** so I have to move them to the shared group with command **sudo usermod -g sharedgroup USERNAME**.

<img width="713" height="257" alt="Screenshot 2026-09-22 at 8 04 54 PM" src="https://github.com/user-attachments/assets/161116f5-4b75-4d09-bec0-a0bbbc38e203" />
<br><br><br>

## Creating Directory

Next, we will create directory using bash **sudo mkdir /home/shared** and check if the file exits.
(The output must contain shared file name but mine doesn't. I checked through it and the correct output is in second picture.)

<img width="523" height="120" alt="Screenshot 2026-09-22 at 8 31 25 PM" src="https://github.com/user-attachments/assets/dc27c2c4-b197-4c01-af1b-1fa60cdfa21d" />

<img width="574" height="122" alt="Screenshot 2026-09-22 at 8 39 53 PM" src="https://github.com/user-attachments/assets/bf2dfb84-576f-4245-964e-fadf025c4371" />



## Creating ten files

We will use bash **sudo touch /home/shared/files{1..10}** to create 10 files and then check with bash **la -l /home/shared** to make sure 10files are created.

<img width="504" height="289" alt="Screenshot 2026-09-22 at 9 33 42 PM" src="https://github.com/user-attachments/assets/0fd52b74-233c-4be2-be61-9dafbc8cb4c4" />

## Change Group Ownership

We will use bash **sudo chgrp -R sharedgroup /home/shared**. [ _**home/shared**_ ], file1 root root will become file root sharedgroup.Now we can control access of the group 
members' using the group permission.

<img width="563" height="294" alt="Screenshot 2026-09-22 at 9 42 17 PM" src="https://github.com/user-attachments/assets/c34c8b57-e8df-4b42-a4ce-8f2c855545c7" />


## Removing a member

If we want to remove a member from the group, we can use command **sudo gpasswd -d USERNAME sharedgroup**. And then check with **id USERNAME** to confirm they are no longer in the group.
(In this screenshot, I removed Mallory as an example).

<img width="640" height="99" alt="Screenshot 2026-09-22 at 9 51 30 PM" src="https://github.com/user-attachments/assets/b49abfdd-9a0e-416a-87e0-9617f84f4d57" />


## Switch User

We can switch user from us to other members by using command **su - USERNAME**. (In this screenshot I switch to Alice, I'm ubuntu@ubuntu, Now I'm Alice@ubuntu). After switching user, 
we will see that **whoami** change to the switched username and **ls -l /home/shared** shows the access of them to the files.

<img width="526" height="359" alt="Screenshot 2026-09-22 at 10 03 11 PM" src="https://github.com/user-attachments/assets/a77862b4-16b8-42a4-a163-589d42ddb028" />


## Reflection

In this section, I've learned about how shared files work, and commands for the access and control between users.






