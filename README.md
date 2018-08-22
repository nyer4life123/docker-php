# Docker-php-apache
> How to Setup a PHP environment using docker apache and php

As part of the docker build process we will create a phpinfo page, which we will use to verify the PHP environment settings.

update php.ini to set sys_temp_dir to “/tmp/whateverfolderyouspecify”

update php.ini to enable and set php error_log file

## Installation:

Linux: Install docker:
1. yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo
2. yum install docker-ce
3. Clone the repository
4. cd docker-php

## Build the app
3. docker build -t phpinfo .

## Run the container
4. docker run -d -p 80:80 phpinfo

## Verifying the container and website is up:
1. curl http://localhost on the host where you ran the container
2. Open a browser to http://ec2-52-71-64-160.compute-1.amazonaws.com/ (this is temporary and will be removed shortly).
