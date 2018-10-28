nullible
========

Peter Robinson (nullr0ute) ansible playbooks for various tasks because I'm lazy!

In this repo you will find my laptop/workstation configs for GNOME setups
as well as various other tasks like ARM machine provisioning, IoT and Cloudy
things. Basically it's random ansible playbooks for things I do regularly and
find useful.

It was oroiginally based on ideas and concepts from maxible by maxamillion.

Usage - General
---------------

Install ``ansible`` and ``git``

    dnf -y install ansible git-core

Clone this repo and run the ansible-playbook (run the ``bootstrap-fedora`` if
running a recemt Fedora release.

    git clone https://github.com/nullr0ute/nullible.git
    cd nullible

    # On a recent Fedora release start with
    ansible-playbook -i inventory bootstrap-fedora.yml

Usage - GNOME Desktop/Workstation/Laptop
----------------------------------------

Run the following playbook:

    ansible-playbook -i inventory workstation.yml

Notes
-----
There are no dotfiles or configs included in this ansible-playbook.
Data retention is handled outside the scope of this playbook

References
----------
* [Ansible](http://www.ansible.com/)
* [Ansible Docs](http://docs.ansible.com/ansible/index.html)
* [maxible](https://github.com/maxamillion/maxible)
