# SDS Tutorial - Version: March 2018 
This is a tutorial for SDS, a Stokessian dynamics simulator with possible charge evolution between particles with RC simulators. For details of thoretical formulations please see two publications listed below:

- M. Karzar-Jeddi, H. Luo, P.T. Cummings, Mobilities of polydisperse hard spheres near a no-slip wall, Computers & Fluids, 2018
- M. Karzar-Jeddi, H. Luo, P.T. Cummings, K.B. Hatzell, Computational Modeling of Particle Hydrodynamics and Charging Process for the Flowable Electrodes of Carbon Slurry, Journal of Electrochemical Society


# Requirements

The SDS code can run on both Windows and Linux. On Windows, the code can be compiled is compiled on Microsoft Visual Studiio. SDS uses LAPCK - linear algebra package. To run SDS on Microsoft vsisual studio follow the instruction in:
https://icl.cs.utk.edu/lapack-for-windows/VisualStudio_install.html

On Linux machine the code can be compiled using g++. However LAPACK package has to be installed before and address through makefile.

# Input files

The input files for setting up simulation are:
- input.txt

this file defines setup for simulation and how the code should run. major parameters to set are 
--deltat: is size of time step for transient simulation
nstep: is the total number of time steps
sstep: is starting time step or initial time step (if you are starting from initial time, you may set it to 0)
nsamp: is the periodic saving time steps
version: defines the mobility tensor version, 0 is for F, 1 is for FT, and 2 is for FTS. Note that for simulation near to wall version bigger than 1 is not allowed.
flag_poly: set it to 0 for monodisperese particle size and set it to 1 for polydisperse size distribution
flag_mat: the code was being developed in two versions Matrix based and non matrix based. Later I decided to develop the code based on mobility matrix so keep it at 1
flag_lub: set it to 0 to solve set up with out lubrication assumption and set it to 1 for with lubrication consideration.
flag_prob: 0 is to define problem in free space, 1 is to set problem near a no-slip wall.
flag_fix: 

- location.txt
- force.txt


# Output files

Out put files for simulation are 
- dump.dis_xxx.cfg
- tec_xxx.dat
- velocity.txt


# Parameters
This is a brief list of parameters that are used in the code
