# sftplinux
Tutorial steps on how to create SFTP access on a Linux server.

#Scenario 
You work at company X which would want to have a shared folder with its clients. Due to privacy and data policies, Company X  would like to retain the documents dropped in this folder within their systems. The shared folder is accessible by an internal department within the organisation that should not have Login  access to the server. The internal  department and the clients should be restricted to only accessing Sftp service on the server hosting the files.

#Important 
Since the access is being shared to external parties Sftp should not be set by its defaults rather it should be restricted by chroot sftp jail. This means we will limit this users to only access a directory called "Shared".
This tutorial considers your users are accessing the server from a Windows environment.  To test the success your users will have to use sftp clients/softwares to access the server. This can be gotten from below link: 

  https://www.thegeekstuff.com/2011/06/windows-sftp-scp-clients/
  
