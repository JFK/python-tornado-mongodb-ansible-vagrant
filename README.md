# python-tornado-mongodb-ansible-vagrant

## Preparation

* Vagrant
* ansible

## What gets installed:

* Python3.4
* vim with python3 support
* Python3, Pip & VirtualEnv
* ntp
* mongodb
* redis
* Nignx

## Let's get rolling!

Before run ```vagrant up```, you may need to do...

```
$ ssh-add  ~/.ssh/id_rsa
$ echo 'ForwardAgent yes' >> ~/.ssh/config
```

Setup

```
$ git clone git@github.com:JFK/python-tornado-mongodb-ansible-vagrant.git
$ cd python-tornado-mongodb-ansible-vagrant
$ vagrant up
```

In order to access the site, configure hosts file.

```
$ echo "192.168.33.100 <server_name>" | sudo tee -a /etc/hosts
```

## Contribute

If you have any suggestions, feel free to create an issue here on Github and/or fork this repo, make changes and submit a pull request!
