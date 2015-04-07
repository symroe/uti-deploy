# Under The Influence deployment

Ansible playbook for deploying Under The Influence.

## Setup

 * [Install ansible](http://docs.ansible.com/intro_installation.html) on your computer
 * Add your ssh key to `~/.ssh/authorized_keys` on the UTI server
 * Add the UTI server to your local `~/.ssh/config`, with hostname “uti”

## Provisioning and Deploying

To fully provision and deploy the latest code to the server, run:

```
ansible --limit production provision.yml
```

If you only want to deploy the latest code to the server, you can instead run:

```
ansible --limit production deploy.yml
```
