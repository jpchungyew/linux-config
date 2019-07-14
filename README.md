# Linux Server Configuration
Linux Server Configuration project for Udacity's Full Stack Web Developer Nanodegree Program

## IP address and SSH port
IP: 99.79.51.217 Port: 2200
```
$ ssh <username>@99.79.51.217 -p 2200
```

## URL to Item Catalog app
[http://99.79.51.217.xip.io](http://99.79.51.217.xip.io)

## Installs and Configurations
- All current packages on the server were updated
- Created a user for reviewer, generated SSH key pair for that user and made user sudoer
- Changed the time zone on server to UTC `sudo timedatectl set-timezone UTC`
- Setup server in preparation for hosting web app
  - Installed Python 3, Apache2, WSGI (for Python 3), and PostgreSQL
  - Configured/Organized Flask App and moved appropriate files from Item Catalog repository
  - Ensured files were owned by www-data
  - Configured .conf file for site to be enabled using a2ensite
  - Setup Flask App to use PostgreSQL
  - Updated Client_Secret to include the URL of this server
- Disabled default site on server
- Launched Item Catalog application

## Third-Party Resources
- This server was hosted on [Amazon Lightsail](https://aws.amazon.com/lightsail/)
- [xip.io](xip.io) was used to obtain a DNS
- The OS used was [Ubuntu](https://ubuntu.com/)
- Reference materials that proved indispensable:
  - https://www.codementor.io/abhishake/minimal-apache-configuration-for-deploying-a-flask-app-ubuntu-18-04-phu50a7ft
  - https://www.digitalocean.com/community/tutorials/how-to-deploy-a-flask-application-on-an-ubuntu-vps
  - https://knowledge.udacity.com/questions/21727
  - https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-xvii-deployment-on-linux
  - https://stackoverflow.com/questions/9353822/connecting-postgresql-with-sqlalchemy
  - https://www.codevoila.com/post/2/python3-connect-postgresql-with-psycopg2-on-ubuntu

## Notes
Whew! This was a challenging project, if I had a penny everytime I thought I was in the clear on this project something will come at me out of the blue. After I checked off the last box, I was sort of expecting something to "break" but it didn't! Had a great time with this, thank you to the folks at Udacity!
