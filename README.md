# Udacity FSND Linux Server Configuration

###### This project is a configuration for AWS Lightsail to deploy a python web application.
###### ip: 35.176.50.241 ([click here](http://35.176.50.241) to visit it)



### Connect using SSH
- use the port `2200` and the SSH key to connect
- connet to the `grader` user
example: `$ ssh -p 2200 grader@35.176.50.241 -i [ssh key file]`

### Software installed
- Apache2
- Flask
- Postgresql

### Configurations made
- configured the firewall (UFW) to allow only connections from ports `80`, `2200` and `123`
- created new user called `grader`
- created a SSH key to connect to the user `grader`
- created a new postgresql database called `catalog` with a user `catalog`
- configured a new VirtualHost with file `/etc/apache2/sites-enabled/catalog.conf`
- wrote a new WSGI file in the project directory

### References
- http://flask.pocoo.org/docs/0.12/deploying/mod_wsgi/
- https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
