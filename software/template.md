# Software Name

Put the name of the software as the title.
Link to source code, e.g. GitHub. (if available).
Link to web site (if available). 

## Domain

What is the domain of the software?
e.g. "Quantum chemistry and solid state physics software package that can perform atomistic simulations of solid state, liquid, molecular, periodic, material, crystal, and biological systems."

## Development Status

Not started/prototype/early use in lab/mature/widely used community code

Is the code under active development today?
    
Think about a TRL (see the EU Horizon2020 TRL definitions):

https://ec.europa.eu/research/participants/data/ref/h2020/wp/2014_2015/annexes/h2020-wp1415-annex-g-trl_en.pdf

## Hardware Support

Describe HW support as it is implemented today.

examples

* **NVIDIA** calls to cublas, cuda runtime library and ~10 cuda kernels, built using cuda toolchain.
* **CPU** calls to BLAS (e.g. MKL), hand written intrinsics for AVX2 and NEON for vectorization, OpenMP multithreading
* **Kokkos** portable implementation of stencil motifs in Kokkos. Tested and tuned for NVIDIA GPU (A100, V100, P100) and Intel multicore.

## Dependencies

Describe the dependencies, e.g.
* BLAS and related libraries maybe you have a hard coded dependency on MKL specific function?
* math libraries FFTW, cuFFT, cuRand, Random123, Trilinos, ...
* cudatoolkit, GCC compiler
* Python packages
* Programming languages (e.g. C++14, Python 3.6, Fortran 90)
* Build systems (e.g. CMake, Meson, autotools, Basel)

## Platform Support

Linux, MacOS, Windows?
- how frequently is the software tested or run on the platforms?
- on which platform is development performed?

Note: target platforms are all HPC systems running Linux variants.

## Testing

Does the software have tests and/or verification?
Is it run automatically with CI? How often? etc.

## Planned Development

What development work is planned to meet the requirements of the project
- new featurews
- porting feature support to HPC platforms
- optimization and tuning

## Development Resources

What man power available for working on the software during the DComEX project. Important for scoping the planned feature work and choice of development frameworks.


