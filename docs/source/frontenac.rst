Frontenac cluster
=================

Tips and tricks for the `Frontenac CAC cluster <https://cac.queensu.ca>`_

Read through the CAC wiki for a primer on logging in and submitting batch jobs. 

.. mesa:

Running MESA
------------
`MESA <https://docs.mesastar.org/en/release-r22.11.1/>`_ requires its own SDK to clobber default compilers. To get this to work on Compute Canada systems, including Frontenac, you need to invoke

.. code-block:: bash

   >> module force purge 

Before any attempt to compile or run MESA. This directive should also be included in your bash script when submitting a slurm job. 

.. group directory:

Our Shared Group Directory
--------------------------
In addition to your user directory on the cluster, our group ``hpcg1719`` has a
shared directory found at:

.. code-block:: bash

   /global/project/hpcg1719

Here you can share files with the group without needing to
`secure copy <https://man7.org/linux/man-pages/man1/scp.1.html>`_ (``scp``) the
files to your computer and send it to someone else on the team.
