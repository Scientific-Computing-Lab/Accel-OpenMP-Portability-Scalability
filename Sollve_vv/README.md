### SOLLVE OpenMP Validation and Verification (OMPVV)
The Sollve OpenMP Validation and Verification (OMPVV) project is a community-driven effort to improve the quality and correctness of OpenMP compilers and libraries. The project aims to ensure that OpenMP implementations conform to the OpenMP standard and provide reliable and consistent behavior across different hardware and software platforms. The OMPVV project includes a comprehensive suite of tests that cover a wide range of OpenMP constructs and usage patterns. These tests are designed to expose potential bugs and inconsistencies in OpenMP implementations and to validate that they adhere to the OpenMP specification. The OMPVV project also includes tools for debugging and profiling OpenMP programs, as well as documentation and training materials to help developers write correct and efficient parallel code. By providing a rigorous testing and validation framework for OpenMP, the OMPVV project helps to ensure the reliability and portability of OpenMP-based software and enables developers to write high-performance parallel code with confidence.

This directory contains the results of OMPVV test suite for Intel oneAPI with PVC1100 and for Nvidia NVHPC with A100. 

For Intel oneAPI, we use the ```-fopenmp-version={50,51,52}``` option to compile OpenMP directives in versions 5.0, 5.1, 5.2 respectively.

---
#### References

https://crpl.cis.udel.edu/ompvvsollve/project/

https://github.com/SOLLVE/sollve_vv
