# Installation
* Install Vagrant and VirtualBox
* In a terminal navigate to the project root
* Provision the VM: `vagrant up`
* SSH into the VM: `vagrant ssh`
* Create the Python virtual environment
* Add an entry in your hosts file for 192.168.56.101 -> ballmercurve.com

```
cd /var/www/
mkdir env
cd env
virtualenv-3.4.0 .
```
* If the virtualenv command is not found, run `vagrant provision` -- virtualenv is not always installed on initial provisioning.

From /var/www/env, active the virtual environment and install the django package:

```
source bin/activate
pip install django
```

Navigate to /var/www/django-durr and run the migrations

`python manage.py migrate`

Create the super user:

`python manage.py createsuperuser`
