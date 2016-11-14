# A Jenkins Master Vagrant Box

## What is this?

An [Ubuntu 16.04][1] [Vagrant][2] box that installs and configures a
[Jenkins2][3] server, bypassing the web gui configuration and installing
plugins automatically. The base box is from the [Bento project][5].

The Jenkins box is provisioned using [Ansible][4], and was mostly a way for me to
play around with various Ansible features and best practices.

## Use

`$ vagrant up` and wait a while. Visit
[http://localhost:8080](http://localhost:8080) and log in as `jenkins` with
password `jenkins` and enjoy playing around with a Jenkins master.

## TODO

- Consider moving to [Alpine][5], a much lighter weight [box][6].



[1]: http://releases.ubuntu.com/16.04/ "Ubuntu 16.04 Xenial"
[2]: http://vagrantup.com "Vagrant"
[3]: http://jenkins.io "Jenkins2"
[4]: http://ansible.com "Ansible"
[5]: https://alpinelinux.org/ "Alpine Linux"
[6]: https://atlas.hashicorp.com/maier "Alpine Boxes"
