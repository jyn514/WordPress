# WordPress
This is a repository documenting the steps to create a network of Dockerized Wordpress instances on a single virtual machine.
It will walk you through each of the required softwares, files, and DNS configurations to get it working.
We will be using Google Cloud Platform to host our VM and configure the DNS settings. 

Table of Contents
* [Getting Started](#Getting-Started)
* [DNS configurations](#DNS)
* [Deployment](#Deployment)
* [Is It Working?](#Testing-and-troubleshooting)
* [Credits](#Credits)

# Getting started
To create a working network of containers hosting wordpress sites, the host machine must have the following software installed.

**_Nginx_**
Used on the machine to manage connections. By using the exampleSitesEnabled file, you can see that we are able to
connect site10.wordpress.cdhsc.org to port 8010, which is defined to be container 10.

How to install

Images of the file and its location

**_Certbot_**
Used to generate ssl certification settings, located in the same sitesEnabled file that was previously referenced.
It uses the same certifcate for all website, located in /etc/letsencrypt/live/site1.wordpress.cdhsc.org/privkey.pem


How to install

Images of the file and its location

**_Docker_**
Docker daemon for running the docker containers

How to install

commands to see the version/testing if it was correctly installed

**_Docker-Compose_**
An orchestraion tool for starting up the front end and back end containers (the script)

How to install

Images of the file and its location

# DNS
This is where we will explain how to configure the DNS settings in Google Cloud

Images of the DNS configs in GCP



# Testing and troubleshooting
Testing the configure



# Credits
Credits to the people that worked together to get this tech stack working
