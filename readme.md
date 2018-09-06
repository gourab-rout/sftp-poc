#Sftp File Polling

This POC explains how we can read files from a SFTP location. This poc assumes you have already SFTP configured.
In order to run this project, please update the SFTP details in the file src/main/resources/local.propeties
The SFTP can have a username/password or identityfile/passphrase. For both the cases please see the below config.

Components Used To Develop Project
==================================

1. CrushFTP
2. Anypoint Studio

Project Setup
==============

### Step 1: Set Up Crush SFTP Server (Optional: If SFTP server is not already installed)

1. Download crush sftp server from <a href="http://www.crushftp.com/download.html"> http://www.crushftp.com/download.html.
2. Download the zip as per the operating system.
   Extract the zip file and run CRUSHFTP.exe. The following dialogue box is opened
 
   ![ScreenShot](https://raw.githubusercontent.com/indiramallick1988/Demo2/master/tool/crushftpexe.PNG)

3. Click on "Create New Admin User". Provide the username and password to create new admin user.
4. Click on "Start Temporary Server" to start sftp. Sftp server starts with the following message

   ![ScreenShot](https://raw.githubusercontent.com/indiramallick1988/Demo2/master/tool/serverstarted1.PNG)

5. To configure Sftp polling path as read only, log on to the server <a href="http://127.0.0.1:8080/">http://127.0.0.1:8080/.
   After log in below page is displayed.

   ![ScreenShot](https://raw.githubusercontent.com/indiramallick1988/Demo2/master/tool/admin.PNG)
  
6. Create a new user by navigating "Admin"---> "User Manager" -----> "Add".
  
   ![ScreenShot](https://raw.githubusercontent.com/indiramallick1988/Demo2/master/tool/usermanager1.png)
  
7. To configure the Sftp path click on the newly created user. Drag file from Server to user and give it read only access.

   ![ScreenShot](https://raw.githubusercontent.com/indiramallick1988/Demo2/master/tool/sftp%20path%20conf1.PNG)

8. Now log on to the Sftp server with credentials of newly created user to check if the path is correctly configured.
 
### Step 2: SFTP Config

1. If the SFTP has username and password, please provide the details as below

   ![ScreenShot](https://raw.githubusercontent.com/gourab-rout/Demo2/master/SFTP/Capture1.PNG)
    
2. If the SFTP has identityfile and passphrase, please provide the details as below

   ![ScreenShot](https://raw.githubusercontent.com/gourab-rout/Demo2/master/SFTP/Capture2.PNG)