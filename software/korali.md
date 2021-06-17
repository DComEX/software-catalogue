# Korali

* Web: https://www.cse-lab.ethz.ch/korali/
* Github: https://github.com/cselab/korali
* Readthedocs: https://korali.readthedocs.io/en/master/
* CircleCI: https://app.circleci.com/pipelines/github/cselab/korali

## Domain

Bayesian uncertainty quantification, stochastic optimization, reinforcement learning, supervised learning, surrogate modelling.

## Development Status

* TRL 8 - Fully operational, used in scientific studies. 
* Code has >95% test coverage on multiple OS (docker) images and compilers.
* Code is fully documented (doxygen) and user manual is available on read the doce.

## Hardware Support

* NVIDIA - Optionally, when using the CUDNN neural network backend, it requires access to NVIDIA GPU devices.
* CPU CPU - Intensive computation (Dense Linear Algebra mostly) using GSL, Eigen3, and OneDNN
* Local Parallelism - It employs local parallel sampling through fork/join (multiprocessing). Some ML kernels in Korali use OpenMP for acceleration.
* Distributed Parallelism - It employs MPI for distributed sampling.

## Dependencies

* Python3 - For the python interface. Additionally: pip, pybind11, python3-config
* GSL - For random distribution sampling and some Dense LA operations.
* Eigen3 - For Dense LA operations and NN backend.
* (Optional) MPI - For distributed sampling
* (Optional) OneDNN - For faster NN backend.
* (Optional) CUDA RT, CuDNN - For GPU-based NN backend.
* Compiler: GCC or clang, with support for C++17 or newer.
* Building: Meson, CMake

## Platform Support

* Linux: Compiling and tested on Fedora and Ubuntu
* MacOS: Compiling
* Windows: No support yet

## Testing

* All commits to Pull Requests are automatically tested on CircleCI on a variety of Linux systems and compilers (the list of setups is under development)

## Planned Development

* Adding graph-like Bayesian networks to define complex prior dependencies.
* Adding new RL methods
* Improve testing/documentation overall

## Development Resources

* Sergio Martin (Postdoc, 100%) leads the overall project (design, testing, development). He also develops the Reinforcement Learning side.
* George Arampatzis (Postdoc, 100%) develops the Bayesian UQ and surrogate modelling side.

CSELab members that also collaborate on the development of new ML and BUQ methods:
* Daniel Waelchli
* Pascal Weber
