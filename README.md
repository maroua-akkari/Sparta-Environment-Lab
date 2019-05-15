# Sparta Environment Lab


A development environment was set up to house the tools needed to connect a database to an app and run it on a web server.

This repository contains a *vagrant file* which allows us to build a virtual machine to run an app, and includes the IP address as well as paths to the provision and app files.

This file also has commands to direct the default nginx port to the index page of this app.  

This repo also contains a *provision* file which has instructions to install nginx (runs webservers), nodeJS and pm2 (acts as a reloader).

To run this app:

1. In the terminal clone this repository and go into the directory.

2. Run the command `vagrant up`.

3. Run the command `vagrant ssh`.

4. Go into the directory containing the app.js file by running the command `cd /vagrant/app`

5. Run the command `node app.js`

Now your app is ready to open:

Open up a web browser e.g. Chrome and enter http://development.local to see the app work.

6. To end this session run the command `vagrant destroy` in the terminal.
