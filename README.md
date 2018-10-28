# Mac Development Ansible Playbook

This is my mac setup. 

This is a fork of [@ricbra](https://github.com/ricbra)'s mac setup which, in turn, is a fork of [@gerlingguy](https://github.com/geerlingguy)'s mac setup script.

For installation:

    $ xcode-select --install
    $ sudo easy_install pip
    $ sudo pip install ansible
    $ mkdir projects && cd projects
    $ git clone git@github.com:ricbra/mac-dev-playbook.git
    $ cd mac-dev-playbook
    $ ansible-galaxy install -r requirements.yml

    For Ansible < 2.0
    $ ansible-playbook -i inventory --ask-sudo-password main.yml
    For Ansible >= 2.0 use
    $ ansible-playbook -i inventory --ask-become-pass main.yml

    $ cd ~/dotfiles
    $ bin/install
    $ bin/setup_osx
