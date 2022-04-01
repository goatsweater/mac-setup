Oh My Zsh
=========

To make configuring the shell easier the `on my zsh <https://ohmyz.sh/>`_ project can
be used.

Install
-------

A simple installer exists as a single command. Recognizing the risk of running a shell file
straight from the internet, it can be downloaded and inspected before using it.

Terminal configuration
----------------------

With Oh My Zsh installed, there's still some terminal configuration to do.

1. Ensure the ``$PATH`` is set properly. Right near the top of the :file:`.zshrc` file
   should be ``export PATH=$HOME/Library/Python/3.8/bin:/opt/homebrew/bin:$PATH``.
2. Enable the following plugins:

   * git
   * history

3. Update the terminal profile in preferences

   * Open Terminal preferences
   * On the "Profiles" tab, select "Pro"
   * Press the "Default" button to set it as the default
   * Set the window size to 120 columns and 30 rows