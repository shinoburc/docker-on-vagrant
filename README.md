# docker-on-vagrant

Vagrantfile for docker(and docker-compose) on vagrant.

## Require

* [Vagrant](https://www.vagrantup.com/)

## Install

Git clone 

```shell
 $ git clone git@github.com:shinoburc/docker-on-vagrant.git
 $ cd docker-on-vagrant
```
Install vagrant plugin

```shell
$ vagrant plugin install vagrant-docker-compose
```

Install vagrant plugin (In http_proxy environment ONLY)

```shell
$ vagrant plugin install vagrant-proxyconf
```

## Run

```shell
$ vagrant up
$ vagrant ssh docker
```

## Reference

* [vagrant-docker-compose](https://github.com/leighmcculloch/vagrant-docker-compose)
