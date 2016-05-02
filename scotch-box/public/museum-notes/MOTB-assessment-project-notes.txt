
Museum of the Bible Assessment Project
======================================
Project: Note Application
Developed by: Edwin Hopper
Date:   4/30/2016 - 5/1/2016


Overview of steps taken...
==========================
1. Attempted to build assessment in laravel/homestead
2. Scotch Box with LAMP stack features used to create/modify the web application
3. Vagrant used as the virtual box
4. Created a private network to host the app ip=192.168.33.10 (via scotchbox)
5. Stood up the web app in the virtual site 'http://192.168.33.10/museum-notes/index.html' 
6. Researched Registration and Login web apps.
7. Stood up the Registration and Login web apps 'http://192.168.33.10/'
8. Configured and tested db settings, pointed the User Login Home page to museum-notes.
9. Folder cleanup... research & development mess, trial & error file messes.
10. Researched GitHub repo add process, then Documentation and Review 


Original Request email and pdf info
===================================
Email Request Highlights:

- Build out this assessment and then add me to the repo come Monday morning. 
My github username is danielfrance.

- I would appreciate it if you would build this assessment in Laravel and use vagrant as your 
virtual box (if possible).  These are tools we use daily so we do not expect you to be a master 
of them in a weekend; we would just like to see how quickly you can pick them up.  

- I look forward to reviewing what you send over. 

PDF Ojectives:

The web application will allow users to create, read, update and delete notes. Notes consist
of a “title”, “description”, “created at” date and if the note has been updated, an “updated
at” date. A user might accidentally delete a note so create the ability to restore a deleted
note.
Since some of these notes may be of personal nature, a user will be required to login prior to
viewing any notes. Allow a new user to sign up and create a new account. Notes should be
persisted to the user’s account. Keep in mind that the user will need to access their account
from various devices.
A user may also want to share a note with another registered user. Build in the functionality
to allow a user to share a note with other users and have that note included in their note list.
Please use the LAMP stack to create this web application. You may use any framework, front
& back, you desire. Have fun with this assessment and make it your own. We encourage you
to implement any unique solutions to solving the issues above. Please be prepared to discuss
why you chose those solutions over others.

=======================
My Requirements Outline
=======================

I. Development Requests
	1. Build assessment in Laravel
	2. Vagrant as the virtual box
	3. Add danielfrance to repo by Monday Morning

II. Note App Functions
	1. Create, Read, Update, Delete Notes
	2. Restore a Deleted Note
	3. Each Note consists of a...
		- "Title"
		- "Description"
		- "Created at" date
		- "Updated at" date
		
III. Registration/Login, and Additional Features
	1. Login for each Note prior to reading a Note
	2. New User Sign up and Create New Account
	3. Access Accounts from Various Devices
	4. Share a Note Fuctionality 
	
IV.  Assumptions on my part (hopefully acceptable assumptions)
	1. Notes could be used by Museum Patrons as a journaling service to record the museum experience.
		- This assumption was a driving factor on the intent and purpose for decisions made.
		- I wanted to have a basic proof of concept to scale up to this project idea.
		- With some more time this could become an app that I would be willing to use. 

	2. Use of Open source code is acceptable within copyright rules and regulations.
		- I originally wanted to created an app that was more ground up, but due to the learing 
                  curve of some of the new tools for the virtual box, decided to go the Open Source route.
		- Now that I have seen some of the existing apps out there I could build a more custom app
                  for note taking, or journaling. 

	3. Limited timeframe to be taken in account and understanding the results are not a finished product.
		- I would have liked to have tested the apps in more detail to have a better presentation.



More Detail of Steps taken
==========================

1. Attempted to build assessment in laravel/homestead
	- I learned alot about laravel can be used, and will continue to learn more.
	- Had some dificulty in getting the app served, so I went with scotchbox which listed laravel
          in the list of apps so I knew I could continue to learn laravel with scotchbox.
	- Made a lot of progress and gained some hands on experience with the product.	

2. Scotch Box with LAMP stack features used to create/modify the web application
	- I decided to run scotchbox because it had the same components including laravel
          and it allowed me to setup the private virtual site with less effort.
        - Scotch Box is a preconfigured Vagrant Box with a full array of LAMP Stack features.
	- By the time I was able to get a feel of the file structure and apps in scotchbox I was left
          with a limited amount of time to get a working web app.  
    
3. Vagrant used as the virtual box
	- I really picked up on Vagrant in conjuction with Virtual Box, I have seen it used before, 
          but never actually used it myself.  I am used to working with Microsoft VM and really didn't
          have a need to use Vagrant or VirtualBox, but after using it I will use it alot now.
	- Once I was able to 'vagrant up' scotchbox and serve up the virtual site I knew I could 
          probably get the rest of the project to an acceptable state.

4. Created a private network to host the app ip=192.168.33.10 (via scotchbox)
	- This was suprisingly simple, as I just uncommented the config in the vagrantfile and ran the
          'vagrant up scotchbox' command and had a private network site to run the app.
	- Yay! the virtual configuration was now at a point where I could continue the project. 

5. Stood up the web app in the virtual site 'http://192.168.33.10/museum-notes/index.html' 
	- By this time I didn't have any code to fulfill the requirements so I made a decision to 
          research opensource to see if I could find something that was functional enough yet easy
          modify and have something to present.  Surprisingly there were existing apps that met my 
          expectations. I found many but narrowed it down to TiddleWiki for various reasons and the
          name was not one of them.

6. Researched Registration and Login web apps.
	- Now I needed to find a basic Register and Login application to connect to a database on the
          virtual box created users and point them to the Notes application.  I found one on github,
          it was not one that I am completely pleased with because it is throwing a deprecated error,
          but it did the job bugs and all.

7. Stood up the Registration and Login web apps 'http://192.168.33.10/'
	- I put the Reg Login app in place, configured it, and with some connectivity effort and
          obsticles I was able to get it going.  I created a couple of users to prove the concept,
          then made sure the links pointed some links to the notes page and had a "working" product.

8. Configured and tested db settings, pointed the User Login Home page to museum-notes.
	- I ran into some issues with the configuration, and was trying to connect to the MySql db
          using some tools that I was familiar with to no avail, so I had to test and check using the 
          command line editor on the virtual box using the MySql command line.  I stumbled through 
          and was able to confirm the app created a user table and added users.  

9. Folder cleanup... research & development mess, trial & error file messes.
	- I had a lot of extra files and folders that were un-needed so I did some quick cleaning
          and retesting to make sure I did not remove anything that was needed. 

10. Researched GitHub repo add process, then Documentation and Review 



Additional Comments:
====================
- Although most of the tools were new to me, I enjoyed the process of learning new and different ways 
  of applying these web apps.  This was definately a crash course in learning and was a fun 
  project.  I look forward to having an opportunity to explain more about this project and 
  more about what I can offer to the Museum of the Bible from my professional career experience.

 
