# Project_Bahmni
Implementation of Hospital Management System in Rural Spaces as a case study using open source EMR Bahmni

INSTALLATION STEPS OF BAHMNI

•	Install Git.
Git: http://git-scm.com/book/en/v2/Getting-Started-Installing-Git
•	Next install VirtualBox.
VirtualBox:https://www.virtualbox.org/wiki/Downloads
•	Next install Vagrant box.
Vagrant: https://www.vagrantup.com/downloads.html (Please install newer Vagrant version)
•	Open Command Prompt.
•	Create a directory as Projects( any name).
•	Cmds: mkdir Projects (enter).
•	Change the directory: cd Projects(enter).
•	Create a folder in projects, name it as Bahmni
•	Cmds: mkdir Bahmni(enter).
•	Change the directory: cd Bahmni(enter).
•	Clone the code from the git by using the command        
git clone https://github.com/Bahmni/bahmni-vagrant.git.
•	Now type command as: cd bahmni-vagrant(enter).
•	Finally enter the command as: vagrant up(enter). It takes some time to complete the download.
•	After sometime open the google chrome and type the url as: https://192.168.33.10/home. 
•	Click on Bahmni Erp and Login with credentials 
Username: superman
Password: Admin123
•	Note: For best practice use google chrome only. After entering the url if it shows as untrusted connection or not supported just click on Advanced and click on proceed then the  Bahmni home page will be opened.
•	If any errors occurs while mounting the vagrant box on virtual box then type the command as: vagrant up --provider = virtualbox.
•	If any errors occurred with the version of the virtual box then update the virtual box version.
•	If you want to modify the source code of the Bahmni for implementing, then open virtual box and run the Bahmni-RPM. 
•	Login as: Username: vagrant
  	    Password: vagrant
•	Change the directory. 
•	Cmd: cd /var/www/bahmni_config/openmrs/apps/ and type ls then list of files will be displayed in that  change directory to applications.json and view the modules like registration.json, clinical.json, etc.


USE CASE:

•	Collect the data of the patients in a excel sheet(.csv file format) who visit the hospital in the form of Registration No, First Name, Middle Name, Last Name, Gender, Location.
•	Open Bahmni setup. Login using the credentials 
	Username: superman.
	Password: Admin123(default we can change).
	Location: Registration Desk.
•	Now in Home page click on admin tab, and again click on upload csv.
•	Then a page will be displayed click on the patient checkbox and upload the file from local system.
•	After uploading we can directly search the patient records by using their Registration No. Now this will be connected with appointment scheduling module.
•	Go to home page click on Appointment scheduling module. We can create the new appointments for the patients, manage the appointments of the patients and also can check the status of the patients whether they have consulted the doctor or not.
	If patient visits hospital for the first time then create the appointment and provide the doctor who are available.
	If required doctor is not available then manage the appointment by changing the  provider’s name.
	We can change the status whether the patient have completed their check up or still not completed. We can generate the graphs to know the status and pending appointments.

•	After completing all the process if we wants to generate the reports click on reports  module and enter the start date, end date and format (in which format to download the reports eg: html, pdf, docx, csv, etc). We can generate daily reports or from certain period to period.

We have other modules like Odoo for billing, OpenElis for laboratory Management, Ward Management and other modules which can be helpful for the staff.

