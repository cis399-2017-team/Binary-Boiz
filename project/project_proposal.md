# Project website: https://binaryboiz.ddns.net/

### Goals: 
* Create a new instance for hosting our project server.
* Create and maintain a web server which hosts the open source software Paperwork https://github.com/twostairs/paperwork/blob/master/README.md .
* Test if the website is working correctly: creating accounts, creating notes, etc.

### Testing Methods:
* Go through all the links in the website and make sure that they are working correctly.
* Go though each task that website provides, like creating accounts, creating notes, etc., and make sure it's working correctly.
* Check the web server and the database if they are running correctly.
      
### Use:
* Gives a set of users access to useful software which may help with productivity.
* Difficulties with using the software can be answered through the Paperwork documentation, or through our expanded knowledge through working with the application.
      
### Difficulties:
* Had to temporarily upgrade our instance's RAM to install and set up the software's dependencies.
* There was problem with 'Forgot password' page it was not sending a 'Password Reset' email and instead it showed an error. (problem is fixed)
      
### User Support Issues:
* A user forgot the account email and password, so there is no way that we can verify the account belong to the user.
* A user deleted a note and want us to recover the note, which can be done if we have the note is in our database backups.

### Security Issues:
* Since Paperwork is an open source software, anyone could look at the source code and try to find a way to breach the website.
* Our server sends and receives sensitive information so we must configure an SSL certificate with nginx to encrypt the information we are sending

### Work needed to complete the project:
* To complete the project we created a new instance for the project and connected it Dynamic DNS http://binaryboiz.ddns.net
* We went through the documentation in the Paperwork github to install and run the web app [link to the docs](https://github.com/twostairs/paperwork/wiki).
* We created an email to send the a password recovery link, in case if a user forgot the account password.
* for more information: https://github.com/cis399-2017-team/Binary-Boiz/edit/master/project/Admin_doc.md

### Maintenance:
* To maintain this software we want to continually update it to the latest version. 
* We would want to keep backups of the website's database so that people who have made user accounts don't lose their information if we make a mistake when updating.
* Making backups could be automated with a time based Cron job.

### Documentation:
* Administration documentation https://github.com/cis399-2017-team/Binary-Boiz/blob/master/project/Admin_doc.md.  
* User documentation: https://github.com/cis399-2017-team/Binary-Boiz/blob/master/project/user_doc.md or http://binaryboiz.ddns.net/help
      
