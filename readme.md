# Lab 15 - DVWA practical

This lab helps you to deploy the DVWA to your development environment.

Please read https://github.com/ethicalhack3r/DVWA carefully

## Caution

Do not upload it to your hosting provider's public html folder or any Internet facing servers, as they will be compromised. It is recommended using a virtual machine (such as VirtualBox or VMware), which is set to NAT networking mode. Inside a guest machine, you can download and install XAMPP for the web server and database.

## RECAPTCHA

Visit https://www.google.com/recaptcha/admin/create to obtain an API key for RECAPTCHA

Place the keys into the `docker/config/config.inc.php` file

## Disclaimer

We do not take responsibility for the way in which any one uses this application (DVWA). We have made the purposes of the application clear and it should not be used maliciously. We have given warnings and taken measures to prevent users from installing DVWA on to live web servers. If your web server is compromised via an installation of DVWA, it is not our responsibility, it is the responsibility of the person/s who uploaded and installed it.

## Running this application

On a virtual machine dedicated to this project (with nothing else running on it) that is not connected to the internet you can run the commands:
    
    docker build -t dvwa .
    docker run --rm -it -p 80:80 dvwa
