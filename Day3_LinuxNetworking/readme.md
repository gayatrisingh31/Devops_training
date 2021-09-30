### Ques How many tables are there in iptables?

Ans. iptables contains five tables:

    1. raw is used only for configuring packets so that they are exempt from connection tracking.
    
    2. filter is the default table, and is where all the actions typically associated with a firewall take place.
    
    3. nat is used for network address translation (e.g. port forwarding).
    
    4. mangle is used for specialized packet alterations.
    
    5. security is used for Mandatory Access Control networking rules (e.g. SELinux

Ques. What is prot, opt, in, out, source & destination?
Ans. prot:prot is a combination of the following access flags: PROT_NONE or a bitwise-or of the other values in the following list: PROT_NONE The memory cannot be accessed at all. PROT_READ The memory can be read. PROT_WRITE The memory can be modified. PROT_EXEC The memory can be executed.
Opt: It means reserved for the installation of add-on application software packages. In this context, “add-on”  means software that is not part of the system; for example, any external or third-party software.
In: packets coming from the network and going to your server.
Out: An OUT file is a compiled executable file created by various source code compilers in Unix-like operating systems, such as Linux and AIX. It may store executable code, shared libraries, or object code. OUT files have been largely replaced by the newer COFF (Common Object File Format) format.
Source: source is a shell built-in command which is used to read and execute the content of a file(generally set of commands), passed as an argument in the current shell script.
OR
Specifies which packets the command filters based on the source of the packet.

Destination: Specifies which packets the command filters based on the destination of the packet.
Ques. Why are rules added to the top?
Ans.
Ques. What type of rules can we add to the iptables?
Ans.
    1. Delete Existing Rules
    2. Set Default Chain Policies
    3. Block a Specific ip-address. 
    4. Allow ALL Incoming SSH. 
    5. Allow Incoming SSH only from a Specific Network. 
    6. Allow Incoming HTTP and HTTPS. 
    7. Combine Multiple Rules Together using MultiPorts. 
    8. Allow Outgoing SSH.
    9.  Allow Outgoing SSH only to a Specific Network
    10. Allow Outgoing HTTPS
    11.  Load Balance Incoming Web Traffic
    12. Allow Ping from Outside to Inside
    13.  Allow Ping from Inside to Outside
    14. Allow Loopback Access
    15. Allow Internal Network to External network.



Ques. Can we block a website by its domain name only?
Ans.Blocking a domain name involves ordering a domain name lookup service (for most users, a function performed by their ISP) not to respond to any user request to look up the IP address associated with that name.
Ques. How can we persist rules in iptables?
Ans.Add rules to the iptables according to your requirement.
    1. Verify that all the rules are present using the command “iptables -L“. # iptables -L.
    2. Save the iptables. # service iptables save.
    3. Restart the service.
    4. Making service permanently ON using chkconfig.

Ques. How can we save rules in iptables?
Ans. Saving iptables firewall rules permanently on Linux
    1. Step 1 – Open the terminal. 
    2. Step 2 – Save IPv4 and IPv6 Linux firewall rules. 
    3. Step 3 – Restore IPv4 and IPv6 Linux firewall rules.
    4. Step 4 – Installing iptables-persistent package for Debian or Ubuntu Linux.
    5. Step 5 – Install iptables-services package for RHEL/CentOS.

Ques. Difference between ufw & iptables?
Ans. iptables provide a complete firewall solution that is both highly configurable and highly flexible.ufw aims to provide an easy to use interface for people unfamiliar with firewall concepts, while at the same time simplifies complicated iptables commands to help an administrator who knows what he or she is doing.
Ques. What are public & private keys?
Ans. You keep the private key a secret and store it on the computer you use to connect to the remote system. Conceivably, you can share the public key with anyone without compromising the private key; you store it on the remote system in a . ssh/authorized_keys directory.
Ques. How does ssh work?
Ans. SSH (short for Secure Shell) is a network protocol that provides a secure way for two computers to connect remotely. SSH employs encryption to ensure that hackers cannot interpret the traffic between two connected devices.
Ques. Difference between HTTP & HTTPS.
Ans. HTTPS is HTTP with encryption. The only difference between the two protocols is that HTTPS uses TLS (SSL) to encrypt normal HTTP requests and responses. As a result, HTTPS is far more secure than HTTP.
Ques. What is SSL?
Ans. An SSL certificate is a digital certificate that authenticates a website's identity and enables an encrypted connection. SSL stands for Secure Sockets Layer, a security protocol that creates an encrypted link between a web server and a web browser.
Ques. Difference between apt update and apt upgrade.
Ans. apt-get update updates the list of available packages and their versions, but it does not install or upgrade any packages. apt-get upgrade actually installs newer versions of the packages you have. After updating the lists, the package manager knows about available updates for the software you have installed.
Ques. What do repositories contain in the Linux System?
Ans. A Linux repository is a storage location from which your system retrieves and installs OS updates and applications. Each repository is a collection of software hosted on a remote server and intended to be used for installing and updating software packages on Linux systems.
Ques. Difference between apt & apt upgrade.
Ans. update: like the regular apt-get update with color output enabled, but apt update also shows the number of upgradeable packages (if any). install,remove: adds progress output during the dpkg run. upgrade: the same as apt-get upgrade --with-new-pkgs .
Ques. What does the number represent after the file permission?
Ans. The first number of the ls -l output after the permission block is the number of hard links. It is the same value as the one returned by the stat command in "Links''. This number is the hard link count of the file, when referring to a file, or the number of contained directory entries, when referring to a directory.
Ques. Difference between apt and apt -get?
Ans.  apt-get may be considered as lower-level and "back-end", and support other APT-based tools. apt is designed for end-users (human) and its output may be changed between versions. Note from apt(8): The `apt` command is meant to be pleasant for end users and does not need to be backward compatible like apt-get(8).

