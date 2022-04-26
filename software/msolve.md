# MSolve

* Github: https://github.com/mgroupntua
* Documentation: https://mgroupntua.github.io/

## Domain

A series of autonomous modules bound together by MSolve.Core for the solution of computational mechanics problems.

## Development status

* TRL 6 - Under refactoring, most unit tests work. 

## Hardware support

* CPU - Intensive computation (sparse linear algebra) using MGroup.LinearAlgebra package
* nVidia GPU - Intensive computation (sparse linear algebra) using CuBLAS
* Shared memory and distributed parallelism - Employs MGroup.Environments which abstracts parallelism while using CUDA, TPL and MPI for multiprocessing.

## Dependencies

MSolve is built on .NET Standard 2.1, thus supporting Mono, .NET framework, .NET Core and .NET. The latest framework as of April 2022 is .NET 6.0 and this is what is used here

* (Optional) SuiteSparse - For linear algebra module
* (Optional) Intel MKL - For linear algebra module
* (Optional) CUDA RT, CuBLAS - For GPU computations
* NuGet v6.0 - For .NET package downloading
* xUnit v2.4.1 or higher - For unit testing
* ILGPU v1.1.0 or higher - For integrating GPU computing
* MPI .NET - For MPI support
* Compiler: .NET 6.0, support for C# 7.0 and higher

## Platform support

* Linux: Compiling and tested on Ubuntu
* MacOS: Compiling and tested on MacOS 12.0 (Monterey)
* Windows: Compiling and tested on Windows 11

## Testing

* All commits to pull requests are being handled by Azure DevOps where source code is checked for syntax, styling and successful tests

## Planned development

* Testing and improving of GPU modules
* Testing and improving MPI
* Improve testing/documentation overall

## Development resources

* George Stavroulakis (Postdoc%), software architect, HPC, domain decomposition
* Serafeim Bakalakos (PhD), HPC, linear algebra, domain decomposition, X-FEM, optimization
* Thofilos Christodoulou (PhD), machine learning

MGroup members that also collaborate on the development:
* Yannis Kalogeris - machine learning, stochastic processes
* Gerasimos Sotiropoulos - multiscale analysis
* Stefanos Nikolopoulos - machine learning
* Ambrosios Savvidis - constitutive modeling
* Kostas Margaronis - contact mechanics
* Stefanos Pyrialakos - AI-enhanced constitutive modeling
