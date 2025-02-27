.. _VUB storage:

VUB storage
==================

The storage is organized according to the :ref:`VSC storage guidelines<data location>`

+--------------------------+------+---------+--------+----------------+
|Variable                  | Type |  Access |Backup  | Default quota  |
+==========================+======+=========+========+================+
|$VSC_HOME                 | GPFS |  VSC    |YES     | 6 GB           |
+--------------------------+------+---------+--------+----------------+
|$VSC_DATA                 | GPFS |  VSC    |YES     | 50 GB          |
+--------------------------+------+---------+--------+----------------+
| | $VSC_SCRATCH           | GPFS |  Hydra  |NO      | 100 GB         |
| | $VSC_SCRATCH_SITE      |      |         |        |                |
+--------------------------+------+---------+--------+----------------+
|$VSC_SCRATCH_NODE         | ext4 |  Node   |NO      | (no quota)     |
|                          |      |         |        |                |
+--------------------------+------+---------+--------+----------------+

VUB users can join a Virtual Organization (VO), giving access to extra storage
that is shared between the members of the VO. See the VUB-HPC docs on `Virtual
Organization <https://hpc.vub.be/docs/vo/>`_ for more info.

For users from other universities, the quota on $VSC_HOME and $VSC_DATA are
determined by the local policy of your home institution as these file systems
are mounted from there. The path names are similar with trivial
modifications based on your home institution and VSC account.

+--------------------------+--------------------------------+
|Variable                  |Path                            |
+==========================+================================+
|$VSC_HOME                 |/user/brussel/10X/vsc10XYZ      |
+--------------------------+--------------------------------+
|$VSC_DATA                 |/data/brussel/10X/vsc10XYZ      |
+--------------------------+--------------------------------+
| | $VSC_SCRATCH           |/scratch/brussel/10X/vsc10XYZ   |
| | $VSC_SCRATCH_SITE      |                                |
+--------------------------+--------------------------------+
|$VSC_SCRATCH_NODE         |/tmp                            |
+--------------------------+--------------------------------+

