# Installation
* Install Vagrant
* In a terminal navigate to the project root
* Provision the VM: `vagrant up`
* SSH into the VM: `vagrant ssh`
* Create the Python virtual environment

```
cd /var/www/
mkdir env
cd env
virtualenv-3.4.0 .
```

* Add an entry in your hosts file for 192.168.56.101 -> ballmercurve.com
