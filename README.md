# Udacity FSND Linux Server Configuration
An Ubuntu Linux server instance on Amazon Lightsail that has been configured with good security settings that runs a web server, an ssh server and a database server

- Public IP Adrress: 35.182.168.140
- Web Server Port: 80
- SSH Server Port: 2200
- Database Server Port: 5432

# Web Server Software Installed
 - Apache2HTTPServer: to get the server responding to HTTP requests on Port 80
 - Apache2Mod-WSGI: to configure Apache to handle requests using the WSGI module which is a specification that describes how a web server communicates with web applications
 
 - VirtualEnv: A python virtual environment to isolate the Item Catalog Application 
 
 # SSH Server 
 
 # Database Server Software Installed
 - PostgreSQL: An Object-Relational Database Management System for the Item Catalog Application. A user catalog was created with limited permissions and require authentication to the application database

- Host: Localhost
- Port: 5432
- Username: catalog
- Password: **********
- Database Name: catalog
