sbrc-2015-simulation
====================

Simulation for article submited to SBRC 2015

How to run
----------

Run ```{arch,ubuntu}-setup.sh``` from folder ```setup``` according to your distro. This will create a new [virtualenv][1], inside the folder ```env```, including all necessary dependencies to run. Source this ```virtualenv```:
  
    $ source env/bin/activate

After that, run the commands in the following order:

    $ cd ..
    $ bash 00submodules.sh
    $ python 01simulate.sh simulations-configs/experiment5/pycloudsim-20140615-00658-linear.conf
    $ python 02summarizedata.py simulations-configs/experiment5/pycloudsim-20140615-00658-linear.conf

The results will be available in the folder ```results```.

[1]: http://virtualenv.readthedocs.org/en/latest/
