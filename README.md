# Ansible configuration for our home

This repo contains the [ansible](http://docs.ansible.com/ansible/latest/index.html) configuration for our home, including laptops
and raspberry pies.

It contains (in `infrastructure.yml`, unless specified otherwise)

- initial setup (`init.yml`)
- basic setup
- optimization
- bluetooth setup

The inventory is described in `hosts`.

We lean on the ansible config of MGM at HUS in Bergen, Norway - shoutout to
@inful.

## Setup & Usage

- clone the repository
- ([get
ansible](https://www.google.no/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=0ahUKEwjCutH56s7WAhVmP5oKHQXWCTcQFggtMAE&url=http%3A%2F%2Fdocs.ansible.com%2Fintro_installation.html&usg=AOvVaw0QBIODybz7M47MR5vx6WwZ))
- modify the `hosts` file to reflect your own setup
- run the `init.yml` playbook to ensure python is setup on all machines
- check out the playbook `infrastructure.yml` and choose and pick which roles
  you would like to deploy using tags, or apply everything : )

You can also [learn more about ansible and
playbooks](http://docs.ansible.com/ansible/latest/playbooks_intro.html).
