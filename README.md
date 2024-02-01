# sftplinux
Tutorial steps on how to create SFTP access on a Linux server.

#Scenario 
You work at company X which would want to have a shared folder with its clients. Due to privacy and data policies, Company X  would like to retain the documents dropped in this folder within their systems. The shared folder is accessible by an internal department within the organisation that should not have Login  access to the server. The internal  department and the clients should be restricted to only accessing Sftp service on the server hosting the files.

#Important 
Since the access is being shared to external parties Sftp should not be set by its defaults rather it should be restricted by chroot sftp jail. 
