### LULESH Pefromance Scalability on Intel PVC and NVIDIA A100 GPUs

The LULESH version we run supports OpenMP 4.0 offloading [[1]](#1) and is available in https://github.com/AMDComputeLibraries/OpenMPApps/tree/master/lulesh-mp4.

#### Compilation flags for PVC with oneAPI (icx 2023):
```-Ofast -qopenmp -fopenmp-targets=spir64 -fiopenmp ```
#### Compilation flags for PVC with oneAPI (gcc 12.2.0):
```-Ofast -fopenmp -foffload='-lm -latomic'```

### Results
We run LULESH for 20 iterations per execution. The results are shown in PVC and A100 subdirectories. \
GPU analytics were collected with NVIDIA Nsight Profiler for A100 and with ```LIBOMPTARGET_PLUGIN_PROFILE=T``` debugging option available in oneAPI for PVC.

## References
<a id="1">[1]</a> 
Bercea, Gheorghe-Teodor, et al. "Performance analysis of OpenMP on a GPU using a CORAL proxy application." Proceedings of the 6th International Workshop on Performance Modeling, Benchmarking, and Simulation of High Performance Computing Systems. 2015.
