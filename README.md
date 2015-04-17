# Base AMI Build

This project builds a base AMI for use in all other builds.
This AMI contains the following items:

* Ansible
* Java
* Docker
* Userify Shim
* Userify Credentials from User Date Upstart
* Peoplenet Consul Configuration

## Versions

* `1.0.1` - `ami-3ee4e156`
* `1.0.0` - `ami-b8c3f9d0`

## Notes

This project declares it's own `image.json` file.
This is a copy of the default template in `packerw` but includes the installation of Ansible on the machine before executing the Ansible provisioner.
