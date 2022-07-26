Lunch Linux Server (in this case, Ubuntu server in AWS EC2)
![alt text](./images/01.png)
Create a project folder.
```bash
mkdir Shell && cd Shell
```
In the new directory, create the following require files - ***names.csv id_rsa.pub onboarding_users.sh***
![alt text](./images/2.png)

Open and populate with names.csv, one entry per line. Save and exit.
![alt text](./images/33.png)

Open and populate the id_rsa.pub file the public key. Save and exit.
![alt text](./images/4.png)

Add shell script to automate the onboarding of 20 users. Save and exit.
![alt text](./images/5.png)


Create the developers group
```bash
sudo groupadd developers
```
![alt text](./images/44.png)

Make the shell script executable
```bash
sudo chmod +x onboarding_users.sh
```
![alt text](./images/22.png)

Change user to super and run script.
![alt text](./images/21.png)

User are created successfully
![alt text](./images/23.png)

Verify the new users, 
```bash
cd ../..
```
```bash
ls -la
```
![alt text](./images/25.png)

From a window client using putty, Login as James.
Prepare private using PUTTYGEN, copy the private key and save.
![alt text](./images/31.png)

Save as private Key
![alt text](./images/32.png)

Open PUTTY, click Auth inside the ssh tab, load the just created ppk file.
![alt text](./images/35.png)

Scroll to the top and click on Session and insert the public ip of the ubuntu server. Click open and accept the prompt
![alt text](./images/36.png)

Login as James
![alt text](./images/40.png)

Click to view **[Demo video](https://drive.google.com/file/d/15Rcy48DctwKd7UkBwIgBAdj88PXLiLAe/view?usp=sharing)**