# note-project
A note taking web application for a project assessment

Project: Note Application
Developed by: Edwin Hopper
Date:   4/30/2016 - 5/1/2016

Overview of steps taken...
==========================
1. Attempted to build assessment in laravel/homestead
2. Scotch Box with LAMP stack features used to create/modify the web application
3. Vagrant used as the virtual box
4. Created a private network to host the app ip=192.168.33.10 host=defaulthost (via scotchbox)
5. Stood up the web app in the private virtual site 'http://defaulthost/museum-notes/index.html' 
6. Researched Registration and Login web apps.
7. Stood up the Registration and Login web apps 'http://defaulthost/reglogin/source/index.html'
8. Configured and tested db settings, pointed the User Login Home page to museum-notes.
9. Folder cleanup... research & development mess, trial & error file messes.
10. Researched GitHub repo add process, then Documentation and Review 

Application Experience
======================
1. Go to the Membership private website 
   - http://defaulthost/reglogin/source/index.html

2. Click Register
   - http://defaulthost/reglogin/source/register.php

3. Enter required fields, and click submit
   - (tesing note) Need to fix email sending process
   - check in MySQL db for confirmation code
     - login to scotch-box vagrant virtual box and go to the MySQL commandline
     - type SHOW DATABASES;
     - type USE museum;
     - type SELECT * from fgusers3;
     - find the new registered user record and enter the confirmation code into
       the confirmation code field on the confirmation page... 
       'http://defaulthost/reglogin/source/confirmreg.php' and click submit.

4. The thank you for registering page displays...
   - 'http://defaulthost/reglogin/source/thank-you-regd.html'

5. Click the 'Click here for login' link.
   - This takes you to the Login page'http://defaulthost/reglogin/source/login.php' 

6. Enter the login and password and click Submit.
   - This directs you to the Welcome Home Page...
    'http://defaulthost/reglogin/source/login-home.php'

7. Click on the 'Museum Experience Journal' link...
   - 'http://defaulthost/museum-notes/index.html'

8. Begin taking notes!

