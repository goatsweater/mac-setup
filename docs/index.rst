
Mac setup documentation!
========================

Install and configure as much as possible on a Mac. The goal is to make the
setup resilient to failure beyond what basic backups can provide. This also
bypasses the use of system to system data transfers, avoiding the cruft that
can come from those kinds of data transfers.

This process leverages Jeff Geerling's excellent `Mac Development Ansible Playbook`_.

.. warning:: 

   This does not replace the requirement for backups. It is in addition to
   a good backup strategy.

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   setup
   software/ohmyzsh
   software/safari
   software/rancher
   software/webodm
   software/osm


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`


.. _Mac Development Ansible Playbook: https://github.com/geerlingguy/mac-dev-playbook