Initial setup
=============

The initial setup of the system consists of following the basic setup wizard,
then leverages Jeff Geerling's `Mac Development Ansible Playbook`_ to install and
configure as much as possible.

Setup wizard
------------

Follow the setup wizard to configure a new mac, including signing into iCloud.
Rather than transfering data from an existing mac, just complete the basic setup
steps and come back to this once complete.

CLI tools
---------

Apple's command line tools are required to complete the setup, but more than that
they are just generally useful. Install them through the Terminal::

    xocde-select --install

Homebrew
--------

Use the instructions from the `Homebrew project <https://brew.sh>`_ to install
the ``brew`` command.


.. _Mac Development Ansible Playbook: https://github.com/geerlingguy/mac-dev-playbook