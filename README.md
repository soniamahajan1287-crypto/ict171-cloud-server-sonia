# ICT171 Cloud Server Project
Student: Sonia Mahajan
Student ID: 35834886

# Public IP Address:
16.170.155.205

# Domain
https://myproject171.duckdns.org/

# Steps I followed:
- Launched EC2 Ubuntu 22.04 cloud server
- SSH into server
- Installed nginx
- Edited /var/www/html to customize website
- Setup the DuckDNS domain: myproject171.duckdns.org
- Installed SSL
- Created backup script
- Documented everything in GitHub

---

# Commands Used
![Screenshot](1.png)
## Installing updates:
sudo apt update && sudo apt upgrade -y
![Screenshot](2.png)
## Install nginx:
sudo apt install nginx -y
![Screenshot](3.png)
## Edit web files:
sudo nano /var/www/html/index.html
![Screenshot](4.png)
## Install Certbot:
sudo apt install certbot python3-certbot-nginx -y
![Screenshot](5.png)
## Enable HTTPS:
sudo certbot --nginx -d mycloudprj.duckdns.org
![Screenshot](6.png)
## Create script:
nano backup.sh
![Screenshot](7.png)
## Make script executable:
chmod +x backup.sh
![Screenshot](8.png)
## Run script:
./backup.sh
![Screenshot](9.png)

# Video Link
https://youtu.be/hugz6yTGWcQ
