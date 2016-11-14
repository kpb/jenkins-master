# A Jenkins Master Vagrant Box

## What is this?

An Ubuntu Vagrant box that installs and configures a Jenkins2 server,
bypassing the web gui configuration and installing plugins automatically.

The Jenkins box is provisioned using Ansible, and was mostly a way for me to
play around with various Ansible features and best practices.

## Use

`$ vagrant up` and wait a while. Visit
[http://localhost:8080](http://localhost:8080) and log in as `jenkins` with
password `jenkins` and enjoy playing around with a Jenkins master.



## TODO

- Consider moving to Alpine, a much lighter weight box

