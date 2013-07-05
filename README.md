Vagrant OBiBa
=============

Vagrant files for OBiBa stack.

## Vagrant VirtualBox

### Prerequisites

* [Vagrant](http://www.vagrantup.com/)
* [VirtualBox (4.1)](https://www.virtualbox.org/)

### Opal

Example on the VirtualBox VM running Opal:

	cd vagrant-virtualbox/opal
	vagrant up

Then connect to:
* opal on https://localhost:8843
* RStudio on https://localhost:8887

### Mica

Example on the VirtualBox VM running Mica:

	cd vagrant-virtualbox/mica
	vagrant up

Then connect to:
* mica on http://localhost:8800/mica

### Opal + Mica

Example on the VirtualBox VM running Opal and Mica:

	cd vagrant-virtualbox/opal-mica
	vagrant up

Then connect to:
* mica on http://localhost:8800/mica
* opal on https://localhost:8843
* RStudio on https://localhost:8887

## Vagrant AWS

### Prerequisites

* [Vagrant](http://www.vagrantup.com/)
* [Vagrant AWS](https://github.com/mitchellh/vagrant-aws): `vagrant plugin install vagrant-aws`

### Opal

Example of a AWS instance running Opal:

	cd vagrant-aws/opal
	# edit AWS credentials
	vagrant up --provider=aws

Then connect to:
* opal on https://<aws-instance>:8443
* RStudio on https://<aws-instance>:8787

### Mica

Example of a AWS instance running Mica:

	cd vagrant-aws/mica
	# edit AWS credentials
	vagrant up --provider=aws

Then connect to:
* mica on http://<aws-instance>/mica

### Opal + Mica

Example of a AWS instance running Opal and Mica:

	cd vagrant-aws/opal-mica
	# edit AWS credentials
	vagrant up --provider=aws

Then connect to:
* mica on http://<aws-instance>/mica
* opal on https://<aws-instance>:8443
* RStudio on https://<aws-instance>:8787 
