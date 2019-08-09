# Walk-through the guide part one

https://wiki.cybera.ca/display/RAC/Rapid+Access+Cloud+Guide%3A+Part+1

1. create ssh key pair
	* `.pem` is private key file extension
2. security group
	* all ports are by default closed
	* so we need to open one
	* egress rule: virtual machine connect to the internet
	* ingress rule: laptop access to virtual machine
	* cidr: specify the IP address block (tutorial just makes completely open)
3. launch instances
	* here can configure the various sizes
	* if you haven't been assigned resources it will show up in red at the bottom
	* can also install the different operating systems
	* each instance can only have one thread because of Spectre mitigation
4. allocate IPs
	* the instance has two: ivp4 and ivp6
	* ipv4s are older, less plentiful and more expensive
	* floating IP can be moved from instance to instance:
		* each project has only one floating IP
5. ssh into the virtual machine
	* you will have password-less admin access (so can use `sudo` freely)
6. volumes
	* create
	* attach to instance
	* go through mounting recipe to get Access

there is a part ii here:

https://wiki.cybera.ca/display/RAC/Rapid+Access+Cloud+Guide%3A+Part+2