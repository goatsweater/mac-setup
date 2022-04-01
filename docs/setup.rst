Initial setup
=============

The initial setup of the system consists of following the basic setup wizard,
then leverages parts of Jeff Geerling's `Mac Development Ansible Playbook`_ to 
install and configure as much as possible.

Setup wizard
------------

Follow the setup wizard to configure a new mac, including signing into iCloud.
Rather than transfering data from an existing mac, just complete the basic setup
steps and come back to this once complete.

Run software update to get any recent updates.

CLI tools
---------

Apple's command line tools are required to complete the setup, but more than that
they are just generally useful. Install them through the Terminal::

    xcode-select --install

Ansible
--------

Install ansible to be able to run the playbook.

1. Upgrade pip: ``sudo pip3 install --upgrade pip``
2. Install ansible for the user: ``pip3 install --user ansible``
3. Update $PATH: ``export PATH="$HOME/Library/Python/3.8/bin:$PATH"``

Using the files under :file:`ansible`, run the playbook.

.. code-block::

   ansible-galaxy install -r requirements.yml
   ansible-playbook main.yml --ask-become-pass

.. note::

    If homebrew commands fail it's likely a license agreement prompt. Run
    ``brew doctor`` to see what is going on.

.. _Mac Development Ansible Playbook: https://github.com/geerlingguy/mac-dev-playbook