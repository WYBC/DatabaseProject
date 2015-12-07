# DatabaseProject
Database Project for CPSC 437 final. Can eventually tie in to 2015 site project.

## Access:
ssh -i <key> ec2-user@52.91.177.0

### bashrc
sudo vim /etc/bashrc
change this line to:
[ "$PS1" = "\\s-\\v\\\$ " ] && PS1="\[\e[0;36m\]$NICKNAME:\[\e[m\] \[\e[1;31m\]\W\[\e[0m\] > "

## Operation
### Start server:
sudo node start-app.js
Run in screen, detach with ctrl-a,d
reattach with screen -r

## Credits

### Starter framework

Base code, including all install files and basic webserver/app taken from code written for *CrowdSound*, a project for Yale's CPSC439 in 2015. It was created by
Eli Block, Jack Feeny, Tim Follo, Jared Katzman, and Terin Patel-Williams.

### What CrowdSound used (from MGT656)

This application relies on a number of open source projects.
Obviously, it is a [node.js](http://nodejs.org/) application.
We are using the following components, which are built for node
applications and written by people that have made them open 
source.

* [express.js](http://expressjs.com/): Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.
* [nunjucks](http://mozilla.github.io/nunjucks/): A templating language for JavaScript. This allows us to say there is a certain default page and every other page should like just like it, maybe changing just small parts.
* [morgan](https://github.com/expressjs/morgan): HTTP request logger middleware for node.js, written by the people who write Express. This allows us to print human-readable logging statements while the application is handling requests.
* [validator](https://github.com/chriso/validator.js): A library of string validators and sanitizers. This helps us ensure that parameters sent to our application by users are valid.
* [body-parser](https://github.com/expressjs/body-parser): Node.js body parsing middleware by the people who write Express.