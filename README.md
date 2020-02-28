# pyOpenCL-LBM
Implementation of 2D lid driven cavity in Python and pyOpenCL.  This jupyter notebook can utilize an OpenCL device to compute with Lattice Boltzmann method.  This includes CPUs and GPUs (Nvidia or AMD).

## Features implemented
* Single relaxation time (SRT) /  Bhatnagar-Gross-Krook (BGK)
* Two relaxation time (TRT)
* Halfway bounce-back boundary condition
* Any aspect ratio
* Comparison to Ghia et al. profiles

## Notes
* Depending on the devices on your computer, you might need to play with the device/platform selection.  If you just have one OpenCL device, this should work correctly out of the box.
* This is adapted and extended from the example CUDA code from Timm Kruger at https://github.com/lbm-principles-practice/code
* This includes an option to under-relax the solution in time, which can help when trying to converge to steady state for high Reynolds Numbers.  

## Dependencies
* Python 3 and standard libraries
* pyopencl
* matplotlib
* Numpy
* Scipy
