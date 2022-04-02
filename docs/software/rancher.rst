Rancher Desktop
===============

While Rancher Desktop installs fine, the command line tools that accompany it fail to
be properly configured under macOS Monterey `due to a permissions error <https://github.com/rancher-sandbox/rancher-desktop/issues/1155>`_.
The tools could be installed through other means, but it is somewhat convenient to have them
bundled and updated along with Rancher Desktop.

The solution then is to get them onto the path through manual linking until the issue is resolved.

1. ``cd /opt/rancher-desktop/bin``
2. ``sudo ln -s /Applications/Rancher\ Desktop.app/Contents/Resources/resources/darwin/bin/kubectl .``
3. ``sudo ln -s /Applications/Rancher\ Desktop.app/Contents/Resources/resources/darwin/bin/nerdctl .``
4. ``sudo ln -s /Applications/Rancher\ Desktop.app/Contents/Resources/resources/darwin/bin/helm .``
5. Update :file:`.zshrc` to add the folder to ``%PATH``

.. code-block::

    # Rancher Desktop
    export PATH="/opt/rancher-desktop/bin:$PATH

Docker alias
------------

Given the prevalence of Docker, there are a lot of scripts and other tools that assume the presence
of the ``docker`` command. Although ``nerdctl`` performs the same operations, manually translating
things is a pain. Instead, create an alias in :file:`.zshrc`::

    alias docker='nerdctl'