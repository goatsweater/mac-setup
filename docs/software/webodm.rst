Open Drone Map
==============

Open Drone Map is used for processing drone imagery to create various types of outputs.
Rather than running the app directly, it is run inside a docker container.

:guide: https://github.com/OpenDroneMap/WebODM#getting-started

In particular, the command for `running odm through docker <https://opendronemap.org/odm/>`_
works well after Rancher Desktop (``nerdctl``) is enabled on the path.

.. note:: 

    In order for the CLI to work the drone images need to be in a folder called :file:`images`
    under the project directory. The project directory should also be referenced by absolute
    path for the volume mount, not relative.