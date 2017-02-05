<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-generate-toc again -->
**Table of Contents**

- [Stelligent Mini-Prjenct Requirements](#stelligent-mini-prjenct-requirements)
- [Setting up the Web server in Docker](#setting-up-the-web-server-in-docker)
    - [Building the Base Docker Image](#building-the-base-docker-image)

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

    1

    this environment.

    2. Commit all code to a public version­control repository of your choice (e.g. Github) and

    provide usage instructions.

    EXTRA: Write automated infrastructure tests to verify the environment works as expected


Setting up the Web server in Docker
===================================

We will leverage the power of Docker for this project.




                         +-------------------------------+
    					 |                     	         |
    					 |                     	         |
    					 |      Base Image     	         |
    					 |                               |
    					 |                               |
    					 +-------------------------------+
    								   ^
    					 			   |
    								   |
    								   |
    					 +-------------+------------------+
    					 |                                |
    					 |        Web Server              |
    					 |         -                      |
    					 |                                |
    					 +--------------------------------+



* The web server will consitis of two Docker images
      * A base Ubunut Image
      * An Apache Image
          * The Apache Image will inherit from the base image
		  

Building the Base Docker Image
------------------------------
