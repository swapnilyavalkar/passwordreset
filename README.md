# passwordreset Web Application for resetting user's passwords on SAP BI4.1 Servers in an automated way.

# Notes:

  <ol> 1. Using this web applications SAP BI4.1 users can reset their own passwords without taking any help from BO administrators.</ol>
  <ol> 2. This application gets the user email id from BO server, so please ensure that you have entered the email ID for all of the users in CMC.</ol>
  <ol> 3. This application only works for Enterprise users as of today.</ol> 
  <ol> 4. Kindly make the necessary changes suggested below before deploying this application in your environments.</ol>
  <ol> 5. This application does not allow to reset the password of administrator user.</ol>
  <ol> 6. This application also checks whether the user id exists on BO server or not.</ol>
  
# Screenshots:  

  <ol> Please check all the screenshots given in the screenshots folder.</ol>

# Changes to be done before deployment:

   <ol>1. Modify the file "myerrors.jsp" as per your requirement for the custom errors.</ol>
   <ol>2. Modify file "ResetUserPasswordId.jsp" to mention your administrator's or support team's email IDs, you can simple replace the email ID xxxxx@xxxxxxx.com in this file with your email id. Also mention your mail server details in this file, you can mention this at SmtpClient client = new SmtpClient("xxxxxxx.com"). Please change the email body in this file as per your requirement.</ol>
   <ol>3. You can modify the file "tutorials.html" to modify the instructions given on the home page of this application as needed.</ol>
   <ol>4. Modify the file "AuthCode.jsp" to mention your admin's email id for String from="xxxx@xxxxx.com" and mail server details for SmtpClient client = new SmtpClient("xxxxx.com"), also change the body of the email id mentioned in this file.</ol>
   <ol>5. Copy your logo file into the images folder and rename it as logo.png</ol>
   <ol>6. Modify the file "logon.jsp" to mention the login details of your BO server as below:</ol>
             <ol> a. //Enter your Admin equivalent User Id </ol>
                <ol> String username = "administrator"; </ol>
             <ol> b. //Password for the ID entered above </ol>
                <ol> String password = "Enter your password here"; </ol>
     
# Usage:
  <ol>1. Download the zip file passwordreset.zip</ol>
  <ol>2. Unzip this file and make the changes as suggested above.</ol>
  <ol>3. After making all of the above changes, you can deploy this web application on your BO server.</ol>
  <ol>4. Copy the folder passwordreset to your web application server's web app folder e.g. BO_INSTALL_DIR\tomcat\webapps\passwordreset</ol>
  <ol>5. Restart your web application server.</ol>
  <ol>6. Open the browser and navigate to passwordreset URL e.g. http://ip_of_bo_server:port/passwordreset</ol>
  <ol>7 .Follow the instructions given on the home page to reset the passwords.</ol>
  
# Credits:  
  <ol>1. This application was originally developed by someone else, I don't recall his name but I have modified it to have more secured procedure and added OTP on email option.</ol>
  <ol>2. Also changed the view and layout of the application as per my requirements.</ol>
  
# License:
  <ol> Free to all :) </ol>
  <ol></ol>
  
  
