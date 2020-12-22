# Ansible Setup for Winston

**Winston** is the hostname for my main computer. It goes with me on all new hardware I get, no matter how many computers / devices I have, Winston is always there as my main machine. 

Trivia: Winston is the name of the protagonist in George Orwell's novell, **1984**. 

## What is included?

This repository contains the Ansible setup to get my favourite Linux based setup up and running. It configures my favourite tools, window manager, scripts, shortcuts, etc. 

While I mostly stick to Fedora as my main OS, the Ansible playbooks and roles are written in such so they are usable on all modern Linux distributions.

## How to run it? 

I'm not sure if these scripts are useful for anyone else, perhaps as an inspiration. I use one private Github repository in the *dotfiles* role as I haven't gotten around to clean any secrets/passwords from my dotfiles. 

When I get a new computer (or completely re-install it), I simply need to copy over my SSH key and run the following commands:

```
ansible-galaxy install gantsign.golang

ansible-playbook -K winston.yml
```

and that will setup my entire machine. 
