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

* `1.0.3` - `ami-4ae9ec22`
  * Still fixing logstash issues
* `1.0.2` - `ami-4aede822`
  * Update logstash role due to missing literal " in command.
* `1.0.1` - `ami-3ee4e156`
  * Lock versions, included Environment in all logstash tags
* `1.0.0` - `ami-b8c3f9d0`

## Notes

This project declares it's own `image.json` file.
This is a copy of the default template in `packerw` but includes the installation of Ansible on the machine before executing the Ansible provisioner.
