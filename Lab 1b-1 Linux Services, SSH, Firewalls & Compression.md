# Lab 1b-1 Linux Services, SSH, Firewalls & Compression

## Apache Webserver

We will install apache with bash **sudo apt download apache2**, and then launch this page in Firefox.

<img width="1470" height="956" alt="Screenshot 2026-09-22 at 4 12 34 PM" src="https://github.com/user-attachments/assets/c5fc2bdb-4fe7-4c35-9d24-b9ac2fb3b0b1" />

And then create a partner VM to carry on other commands. Use bash **ip a** to get the IP address.
<img width="1470" height="956" alt="Screenshot 2026-09-22 at 5 49 39 PM" src="https://github.com/user-attachments/assets/d3e7b015-1ca2-4fe5-9062-1b93930b6d65" />

## Nmap

Use command *nmap ip_of_partner** to check partner's ports.
<img width="627" height="229" alt="Screenshot 2026-09-22 at 6 05 14 PM" src="https://github.com/user-attachments/assets/6fbfecf3-a749-417f-92d4-6fa0bc8ab7b6" />

## UFW

Use bash **sudo ufw status verbose** to check if firewall is activated. If not, use bash **sudo ufw enable** and then check again.
<img width="592" height="213" alt="Screenshot 2026-09-22 at 6 08 34 PM" src="https://github.com/user-attachments/assets/d1d244fb-86ab-4613-931c-a3f8b0a26f97" />

## SSH

Use **ssh ip_of_partner** to check if ssh login work.
<img width="514" height="86" alt="Screenshot 2026-09-22 at 7 11 33 PM" src="https://github.com/user-attachments/assets/bcd8f481-ad21-4723-9bcb-2e4706f31347" />

# Reflection

In this lab, I've learned about networking and firewall, and how security tools work together.
