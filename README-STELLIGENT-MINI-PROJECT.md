<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-generate-toc again -->
**Table of Contents**

- [Stelligent Mini-Prjenct Requirements](#stelligent-mini-prjenct-requirements)
- [Setting up the Web server in Docker](#setting-up-the-web-server-in-docker)
    - [Ansible will be requirements on your development system](#ansible-will-be-requirements-on-your-development-system)
    - [Building and running the web server](#building-and-running-the-web-server)
    - [Building an AWS EC2 to run the web server](#building-an-aws-ec2-to-run-the-web-server)
    - [TO-DO Items](#to-do-items)

<!-- markdown-toc end -->









Stelligent Mini-Prjenct Requirements
====================================


    Stelligent Mini‐Project

    1. Write code in a programming language (or languages, configuration management
       platforms, etc.) of your choice that provisions an environment running on the Linux or
       Windows operating system (You can choose any supported version of Linux or
       Windows). The infrastructure code only needs to provision the environment resources
       and configure a web server. The home page should display a static HTML page with the
       words: “Automation for the People” . There should be a single command that launches
       this environment.

    2. Commit all code to a public version­control repository of your choice (e.g. Github) and
       provide usage instructions.

    EXTRA: Write automated infrastructure tests to verify the environment works as expected


Setting up the Web server in Docker
===================================

We will leverage the power of Docker for this project.


* The web server will be pulled from the offical Docker Hub image
      * httpd  version 2.4
	  * [httpd:2.4](https://hub.docker.com/_/httpd/)
		  
Ansible will be requirements on your development system
-------------------------------------------------------

* Installing Ansible on Ubuntu 
    * [Install Ansible](http://docs.ansible.com/ansible/intro_installation.html#latest-releases-via-apt-ubuntu)


Building and running the web server
-----------------------------------

* Documentation for running the web server
    * [Stelligent Mini-Project](https://github.com/thinkedg/skc-stel-proj-code/blob/master/README.md)
	
	
Building an AWS EC2 to run the web server
-----------------------------------------

* Documentation for building EC2 instance to run the web server
    * TO-DO

TO-DO Items
-----------

* cloudformation to send new cattle to the heard
* setup Jenkins
    * dockerized Jenkins master
	* Jenkins Slave 
	* CI test
	* CD to staging server
	
