Ques. How can 1 give access to someone to my AWS instance?
Ans. 1.    Connect to your Linux instance using SSH.

2.    Use the adduser command to add a new user account to an EC2 instance (replace new_user with the new account name). The following example creates an associated group, home directory, and an entry in the /etc/passwd file of the instance.

$ sudo adduser new_user

3.    Change the security context to the new_user account so that folders and files you create have the correct permissions:

$ sudo su - new_user

4.    Create a .ssh directory in the new_user home directory:

$ mkdir .ssh

5.    Use the chmod command to change the .ssh directory's permissions to 700. Changing the permissions restricts access so that only the new_user can read, write, or open the .ssh directory.

$ chmod 700 .ssh

6.    Use the touch command to create the authorized_keys file in the .ssh directory:

$ touch .ssh/authorized_keys

7.    Use the chmod command to change the .ssh/authorized_keys file permissions to 600. Changing the file permissions restricts read or write access to the new_user.

$ chmod 600 .ssh/authorized_keys

Ques. What are daemon applications?
Ans. Daemon processes are used to provide services that can well be done in the background without any user interaction. For example a process that runs in background and observes network activity and logs any suspicious communication can be developed as a daemon process.some examples of use cases for daemon apps:

    • Web applications that are used to provision or administer users or do batch processes in a directory
    • Desktop applications (like Windows services on Windows or daemon processes on Linux) that perform batch jobs, or an operating system service that runs in the background
    • Web APIs that need to manipulate directories, not specific users



Ques. What .d represents after a file?
Ans. "d" stands for directory and such a directory is a collection of configuration files which are often fragments that are included in the main configuration file. The point is to compartmentalize configuration concerns to increase maintainability.

Ques. What happens when a pem gets deleted?
Ans. PEM files are used to store SSL certificates and their associated private keys.This is the file you use in nginx and Apache to encrypt HTTPS without it you can’t access your instance from your system.
Ques. What is in the host file?
Ans. The /etc/hosts is an operating system file that translates hostnames or domain names to IP addresses. This is useful for testing website changes or the SSL setup before taking a website publicly live.
Ques. What is SCP & what does this command do?
Ans. SCP (secure copy) is a command-line utility that allows you to securely copy files and directories between two locations. With scp , you can copy a file or directory: From your local system to a remote system.
Ques. How port forwarding works?
Ans. SSH Port forwarding is used to forward ports between a local and a remote Linux machine using SSH protocol. It is mainly used to encrypt connections to different applications. Even if that application doesn't support SSL encryption, SSH port forwarding can create a secure connection.
Ques. How can we connect without IP to AWS instance?
Ans. Go into the EC2 dashboard, then in the NETWORK & SECURITY menu go to Elastic IPs. Click on Allocate a new address. Right click on the new IP and select Associate address. Associate it with your EC2 instance that doesn't have an elastic IP.
