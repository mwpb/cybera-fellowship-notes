# Cloud computing

## What is the cloud?

Delivery of computing services over the internet.
Faster, more flexible and leverage economies of scale.

### Various options

Off-load various components of your computing stack onto the pcloud provider.

1. Infrastructure as a service
	* manages networking to virtualisation
	* you manage operating system and upwards
2. Platform as a service
	* manages networking to runtime
	* you manage data and applications
	* e.g. Heroku
3. Software as a service
	* run everything including the application!
	* e.g. Dropbox

The more you run yourself the more flexible you will be.
The more others run the better economies of scale apply.

### Why?

* On-demmand:
	* pay for what you use
* Elastic:
	* probably scales better: you just pay for more
* Efficient:
	* pooling of resources
		* e.g. CPU of laptop is mostly not running
		* indeed can assign 16 virtual CPUs to one physical one
			* but for GPU hasn't been practical until recently
	* allows for economies of scale
* Flexible
	* changing requirements: just pay for different services

## Terminology

* Tenant
* Image
	* virtual machine template
* Instance 
	* a virtual machine
* Snapshots
	* a point-in-time saved state of your instance
	* can branch in different directions from snapshot
		* can add resources to instances spawned from snapshot
* Volumes
	* permanent storage

## What is the Rapid Access Cloud

* Cybera's Infrastructure as a Service
* low barrier and rapid access to a virtual machine
* like Virtualbox but hosted non-locally
* like Amazon EC2

Guide:

https://wiki.cybera.ca/display/RAC/Rapid+Access+Cloud

### Why use RAC?

* GPU processing
* programmatic API to control virtual machines
* publicly host your work
* experiment













