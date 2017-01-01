# Linux Server Config

The application is running on:

  http://ec2-35-166-161-179.us-west-2.compute.amazonaws.com/
  IP address: 35.166.161.179
  SSH port: 2200


##  Update all installed packages

**Google Search 'ubuntu update packages'**
```bash
sudo apt-get update
```


### Install Software packages 

installed python **Google Search 'ubuntu install python'**

installed PostgresQL  **Google Search 'install PostgresQL on ubuntu'**
```bash
sudo apt-get update
sudo apt-get install postgresql postgresql-contrib
```
installed git **Google Search 'install git on ubuntu'**


##  Third Party resources

Digital ocean
https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-postgresql-on-ubuntu-14-04

You can set up your system in a way that it only accepts traffic on
certain ports and blocks everything else. The traditional linux tool to
do that is 'iptables'. As this is powerful but hard to use for beginners,
ubuntu comes with a firewall setup tool that is much easier to use: 'ufw',
the 'uncomplicated firewall'.

**configuration changes: 'linux firewall setup', 'ubuntu ufw'**

We are asked to block everything, and allow incoming connections for these
services:

- SSH on port 2200 (we moved it there in the step above)
- HTTP on port 80 (we will run a webserver later)

The ubuntu documentation of UFW is detailed enough to do this. You configure
the firewall by calling



