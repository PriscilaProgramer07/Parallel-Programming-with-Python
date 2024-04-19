Creating a README file typically involves summarizing the project, including its purpose, how to set it up, and how to use it. Based on the provided content from the PDF document and the `.ipynb` filename, I can draft a README outline for a project about Parallel Programming with Python for calculating π.

---

# Parallel Programming with Python

## Overview
This project demonstrates the calculation of π (pi) using numerical integration in Python. We explore three different computational strategies, each leveraging the concept of parallelism to varying extents.

## Methods

### Non-Parallelized Python Solution
Utilizes a simple for-loop to calculate the area under the curve of a quarter circle to approximate π. This method is sequential and does not involve any parallel computing techniques.

### Multiprocessing
Employs Python's `multiprocessing` library to parallelize the calculation process across multiple CPU cores within a single machine, improving computational efficiency.

### Distributed Computing Using MPI
Leverages the Message Passing Interface (MPI) through the `mpi4py` library for computation across a distributed system, suitable for large-scale and high-performance computing environments.

## Installation

To run the scripts, ensure you have Python installed along with the necessary libraries:
- numpy
- mpi4py (only for the MPI method)
- multiprocessing (included in Python's standard library)

You can install the dependencies using pip:

```sh
pip install numpy mpi4py
```

## Usage

### Non-Parallelized Approach

```sh
python basicspython.py
```

### Multiprocessing Approach

```sh
python multiprocess.py
```

### MPI Approach

Make sure to run this on a system with MPI set up and configured:

```sh
mpiexec -n <number_of_processes> python mpi4pyparallel.py
```

Replace `<number_of_processes>` with the number of processes you wish to run.

## Profiling

Each script contains timing code to measure the execution time of the computation, which helps in analyzing the performance benefits of each method.

## Visualization

Figures demonstrating the results of the computations can be found within the Jupyter Notebook included in the project.

## Authors

- Priscila Guadalupe Tzuc Alonzo - 2109148@upy.edu.mx)

## Acknowledgements

Special thanks to the Universidad Politécnica de Yucatán for providing the resources to carry out this research.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
