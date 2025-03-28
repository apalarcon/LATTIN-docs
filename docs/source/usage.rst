Run LATTIN
=================================

How do I run LATTIN?
----------------------

To run LATTIN, create a file with the following code (could be **run_lattin.py**)

.. code-block:: python

   #!/usr/bin/env python3
  import lattin as lt
   import sys

   lt.lattin_main(sys.argv[1])

Once this code is created, LATTIN can be run as follows:

1- On a Linux computer:

.. code-block:: bash

   mpirun -n N_proc python run_lattin.py input_file

   e.g:  mpirun -np 4 python run_lattin.py test_case.cfg

2- On a HPC with Linux: 

Create a bash script (run_lattin.sh). This example is valid for FINESTARRAE III cluster at the Galician Supercomputing Center.

.. code-block:: bash

   #!/bin/bash -l

   #SBATCH --mem=512GB
   #SBATCH -N 1
   #SBATCH -n 40
   #SBATCH -t 7-00:00:00

   module --purge
   module load cesga/2020
   module load miniconda3/4.9.2
   conda activate envname


   srun -n $SLURM_NTASKS  --mpi=pmi2 python run_lattin.py test_case.cfg


.. code-block:: bash
   sbatch run_lattin.sh

- N_proc: The number of processor should be divisible by 4.


