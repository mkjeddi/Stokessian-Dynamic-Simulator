# SDS Manual and Examples - Version: December 2018 
This is a tutorial for SDS, a Stokessian Dynamics Simulator, is a C++ code to simulate time evolution of particulate suspensions with possible charge transfer between particles. The time evolution of particles is simulated using Stokesian dynamics formulation and the electric potential interactions between particles are simulated using Resistor-Capacitor formulation. For details of thoretical formulations please see two publications listed below:

- M. Karzar-Jeddi, H. Luo, P.T. Cummings, Mobilities of polydisperse hard spheres near a no-slip wall, Computers & Fluids, 2018
- M. Karzar-Jeddi, H. Luo, P.T. Cummings, K.B. Hatzell, Computational Modeling of Particle Hydrodynamics and Charging Process for the Flowable Electrodes of Carbon Slurry, Journal of Electrochemical Society


# Requirements

The SDS code can run on both Windows and Linux. On Windows machine, the code can be compiled using Microsoft Visual Studiio. Prequisite for using Microsoft Visual Studio to run the code is installation of LAPACK package, linear algebra package. Instructions on how to install LAPACK in Microsoft Visual Studio are provided in:
https://icl.cs.utk.edu/lapack-for-windows/VisualStudio_install.html

On Linux machine the code can be compiled using g++. However LAPACK package has to be installed before and address through makefile.
