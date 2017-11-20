# How to setup
> git clone https://github.com/shizus/ubuntu64-lamp7.git

> cd ubuntu64-lamp7

> vagrant up

# Check setup

After `vagrant up` browse to:
[http://www.lamp7.dev/](http://www.lamp7.dev/)

You should see:

```
Contragutlations!

Ubuntu64-lamp7 is working!
```

# How is this working?

## Host names

Vagrant uses vagrant-hostmanager plugin to create a host name, in this case `www.lamp7.dev` while the vm is loading.

If you do not have vagrant-hostmanager installed you should run

> vagrant plugin install vagrant-hostmanager

before running vagrant up. See more information in [https://github.com/devopsgroup-io/vagrant-hostmanager](https://github.com/devopsgroup-io/vagrant-hostmanager)

## Synchronized folders

Your current directory where you run `vagrant up` will be synchronized with guest folder `/var/www/html` which is the default Apache directory
