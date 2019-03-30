# Udacity FSND Linux Server Configuration
An Ubuntu Linux server instance on Amazon Lightsail that has been configured with good security settings that runs a web server, an ssh server and a database server. A grader user was created the ssh key for this user is located at <b>/home/grader/.ssh/authorized_keys</b>

- IP Address: 35.182.168.140
- Web Server Port: 80
- SSH Server Port: 2200
- Database Server Port: 5432


# Web Application
- Language: Python v2.7
- Project Source: <a href="https://github.com/fkrishna/item-catalog">item catalog</a>
- virtualenv: A python virtual environment to isolate the Item Catalog Application

# Web Server
- Apache2HTTPServer: to get the server responding to HTTP requests on Port 80
- Apache2Mod-WSGI: to configure Apache to handle requests using the WSGI module which is a specification that describes how a web server communicates with web applications
 
# SSH Server 
The server require Key Based Authentication for all user and listening on port 2200 instead of the default port 22 using SSH v2 protocol 
- ssh-keygen: to generate new authentication key pairs for SSH using RSA encryption
 
# Database Server
- PostgreSQL: An Object-Relational Database Management System for the Item Catalog Application. A user catalog was created with limited permissions and require authentication to the application database
 - Username: catalog
 - Password: **********
 - Database Name: catalog
 
 # Firewall
 The UFW firewall was configured to allow incoming connection on port 80, 123 and 2200
