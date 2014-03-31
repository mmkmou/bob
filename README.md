bob
===

Bob is a python + ansible tool to facilitate our local Drupal project provisioning.
This tool is built for our specific way of doing things, but since our way of doing things isn't so far out there, Bob might be useful for others.

We hope to make Bob more generic as time goes by. 

For now, the assumptions are:
- vagrant is running on your host
- you have an Ubuntu based guest OS
- you use this VM for local Drupal development
- your Drupal project files remain on your host system and are shared with the VM
- your project itself runs on the VM (so apache, mysql and drush interactions happen on the VM)

Pre-requisites:
- ansible 1.5.x
- vagrant 1.5.1

Usage:

Bob is not used to set up your local development environment. For this we have a different set of ansible playbooks. Bob is only concerned with building projects.

$ bob build <projectname> [--target=(local|vagrant)]


