# Udacity Full Stack Nanodegree linux server project
This project aims to turn a linux barebones server into a secured web application server.

## How to connect
* Using the provided private key, run `ssh -i <key_path>.pem grader@34.243.174.128.xip.io -p 2200` to get to the sudo user `grader`.

## The web app
* The catalog app can visited [here](http://34.243.174.128.xip.io/).

## Assignment details
* User `grader` created and given sudo permissions.
* `root` user can't login remotely (configured in `/etc/ssh/sshd_config`).
* Firewall configured to only allow SSH (port 2200), HTTP (port 80), and NTP (port 123).
* Key-based SSH authentication is enforced (configured in `/etc/ssh/sshd_config`).
* System packages updated to the latest versions.
* SSH is hosted on non-default port (2200).
* A web server is listening on port `80` serving the [catalog](https://github.com/M-Dahab/fsnd_catalog) application using `sqlite` database.

## Packages and Dependencies used
* `python3` interpreter.
* `apache2` server.
* `sqlalchemy` python ORM package.

## Resources
* [How to use Flask with WSGI](http://flask.pocoo.org/docs/1.0/deploying/mod_wsgi/).
* [Apache2 mod_wsgi with python3](http://terokarvinen.com/2017/write-python-3-web-apps-with-apache2-mod_wsgi-install-ubuntu-16-04-xenial-every-tiny-part-tested-separately).
