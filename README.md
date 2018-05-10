# Project_Bahmni
Implementation of Hospital Management System in Rural Spaces as a case study using open source EMR Bahmni

INSTALLATION STEPS OF BAHMNI

Install Git.
Git: http://git-scm.com/book/en/v2/Getting-Started-Installing-Git

Next install VirtualBox.
VirtualBox:https://www.virtualbox.org/wiki/Downloads

Next install Vagrant box.
Vagrant: https://www.vagrantup.com/downloads.html (Please install newer Vagrant version)

Open Command Prompt.

Create a directory as Projects( any name).

Cmds: mkdir Projects (enter).

Change the directory: cd Projects(enter).

Create a folder in projects, name it as Bahmni

Cmds: mkdir Bahmni(enter).

Change the directory: cd Bahmni(enter).

Clone the code from the git by using the command        
git clone https://github.com/Bahmni/bahmni-vagrant.git.

Now type command as: cd bahmni-vagrant(enter).

Finally enter the command as: vagrant up(enter). It takes some time to complete the download.

After sometime open the google chrome and type the url as: https://192.168.33.10/home. 

Click on Bahmni Erp and Login with credentials 
Username: superman
Password: Admin123

Note: For best practice use google chrome only. After entering the url if it shows as untrusted connection or not supported just click on Advanced and click on proceed then the  Bahmni home page will be opened.

If any errors occurs while mounting the vagrant box on virtual box then type the command as: vagrant up --provider = virtualbox.

If any errors occurred with the version of the virtual box then update the virtual box version.

If you want to modify the source code of the Bahmni for implementing, then open virtual box and run the Bahmni-RPM. 
Login as: Username: vagrant
Password: vagrant

Change the directory. 

Cmd: cd /var/www/bahmni_config/openmrs/apps/ and type ls then list of files will be displayed in that  change directory to applications.json and view the modules like registration.json, clinical.json, etc.

