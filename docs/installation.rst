.. highlight:: bash

============
Installation
============

From sources
------------

The sources for ChemFlow can be downloaded from the `Github repo`_.

.. _Github repo: https://github.com/IFMlab/ChemFlow.git

You can either clone the public repository:

    ``git clone https://github.com/IFMlab/ChemFlow.git``


Required software
-----------------

+-----------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| Program               | Link to Download - Licencing may apply                                                                                                    |
+=======================+===========================================================================================================================================+
| PLANTS                | http://www.mnf.uni-tuebingen.de/fachbereiche/pharmazie-und-biochemie/pharmazie/pharmazeutische-chemie/pd-dr-t-exner/research/plants.html  |
+-----------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| AmberTools & Amber    | http://ambermd.org/GetAmber.php   ( An Amber licence is needed for CUDA )                                                                 |
+-----------------------+-------------------------------------------------------------------------------------------------------------------------------------------+
| Anaconda              | https://www.anaconda.com/download/#linux                                                                                                  |
|                       |                                                                                                                                           |
|                       | After installing Anaconda, add some packages packages:                                                                                    |
|                       |                                                                                                                                           |
|                       |   ``conda install -c rdkit rdkit``                                                                                                        |
|                       |                                                                                                                                           |
|                       |   ``conda install -c schrodinger pymol``                                                                                                  |
+-----------------------+-------------------------------------------------------------------------------------------------------------------------------------------+

Additional configuration
-------------------------
In addition to downloading the required software, you must be able to run then flawlessly.
Please set up the PATHS to the their install locations. (modify to your own)

+-----------------------+-----------------------------------------------------------------------------------------------------+
| ChemFlow              | ``export CHEMFLOW_HOME=/home/USER/software/ChemFlow/ChemFlow/``                                     |
|                       | ``export PATH=${PATH}:${CHEMFLOW_HOME}/bin/``                                                       |
+-----------------------+-----------------------------------------------------------------------------------------------------+
| PLANTS                | ``export PATH=${PATH}:/home/USER/software/plants/``                                                 |
+-----------------------|-----------------------------------------------------------------------------------------------------+
| Autodock Vina         | ``export PATH=${PATH}:/home/USER/software/autodock_vina_1_1_2_linux_x86/bin/``                      |
| (qvina2, smina...)    | ``export mgltools_folder=/home/USER/software/mgltools_x86_64Linux2_1.5.6/``                         |
|                       | ``export PATH=${mgltools_folder}/bin:$PATH``                                                        |
+-----------------------|-----------------------------------------------------------------------------------------------------+
| Gaussian              | # Setup some variables                                                                              |
| (required for RESP)   | g09root="/home/USER/software/"                                                                      |
|                       | GAUSS_SCRDIR="${HOME}/scratch/"                                                                     |
|                       | export g09root GAUSS_SCRDIR                                                                         |
|                       | . $g09root/g09/bsd/g09.profile                                                                      |
+-----------------------|-----------------------------------------------------------------------------------------------------+
| AmberTools18          | source /home/USERdgomes/software/amber18/amber.sh                                                   |
+-----------------------|-----------------------------------------------------------------------------------------------------+
