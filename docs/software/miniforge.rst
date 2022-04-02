miniforge/conda
===============

While fully installed and (mostly) ready to use by homebrew, ``conda`` still needs to be
initialized::

    conda init zsh

This updates :file:`.zshrc`, and from that point on conda is ready for use.

Tensorflow
----------

Being relatively new, tensorflow doesn't yet know how to leverage all the power of the M1.
In order to be able to leverage the full power of the GPU tensorflow needs to be installed
from Apple's conda channel. Instructions are available from
https://developer.apple.com/metal/tensorflow-plugin/.