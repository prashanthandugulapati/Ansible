

Jenkins Playbook 

Which can create the base image of jenkins and installs the standard plugins based on the application requirnmnet 

and can also configure LDAPs with it.



#Backup Script.

In this script we are going to use it for the backing up the configuration files, plugins, jobs, secerts and nodes for jenkins instance

where its going to create the desired directories and switches to home directory of jenkins and starts taking 
the backup of all .Xml file and stores in var/lib/cicd-assets/jenkins_backup 



*Backup of plugins folder if exists
 we are backing up the plugins if exists then its going to create directory plugins and copies the plugins to /var/lib/cicd-assets/jenkins_backup/plugins



*Backup of secerts folder if exists 
 we are backing up the secerts if exists then its going to create directory secerts and copies the secret to /var/lib/cicd-assets/jenkins_backup/secerts



*Backup slave nodes folder if exits
 we are backing up the slave node if exists then its going to create directory called nodes and copies the nodes to /var/lib/cicd-assets/jenkins_backup/nodes



*Backup Jobs folder if exits
 we are backing up the Jobs if exists then its going to create directory called jobs and copies all the jobs to /var/lib/cicd-assets/jenkins_backup/jobs

where all backup are stored in var/lib/cicd-assets/jenkins_backup/ in compressed form with date and time taged to it. 



title=Importing_SSL_cert_to_Linux_Jenkins_instance

#Process_to_import_ssl_cert_into_test.jenkins.com_instance 
to raise a request to get ssl cert file. 


