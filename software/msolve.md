# MSolve

A series of autonomous modules bound together by MSolve.Core

* Github: https://github.com/mgroupntua
* Documentation: https://mgroupntua.github.io/

## Domain

A series of autonomous modules bound together by MSolve.Core for the solution of computational mechanics problems.

## Development Status

* TRL 6 - Under refactoring, most unit tests work. 

## Hardware Support

* CPU CPU - Intensive computation (Dense Linear Algebra mostly) using GSL, Eigen3, and OneDNN
* Local Parallelism - It employs local parallel sampling through fork/join (multiprocessing). Some ML kernels in Korali use OpenMP for acceleration.

## Dependencies

* (Optional) SuiteSparse - For linear algebra module
* (Optional) Intel MKL - For linear algebra module
* Compiler: Roslyn, support for C# 7.0 and higher.

## Platform Support

* Linux: Compiling
* MacOS: Compiling
* Windows: Compiling

## Testing

* No CI yet, unit tests are embedded in each module

## Planned Development

* Incorporation of GPU modules
* Testing and improving MPI
* Improve testing/documentation overall

## Development Resources

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
