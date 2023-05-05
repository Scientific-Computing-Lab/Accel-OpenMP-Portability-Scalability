## LULESH Pefromance Scalability on Intel PVC and NVIDIA A100 GPUs

The LULESH version we run supports OpenMP 4.0 offloading [[1]](#1) and is available in https://github.com/AMDComputeLibraries/OpenMPApps/tree/master/lulesh-mp4.

#### Compilation flags for PVC with oneAPI (icpx 2023):
```-O3 -fiopenmp -fopenmp-targets=spir64```
#### Compilation flags for A100 with NVHPC (nvc++ 23.3):
```-O3 -mp=gpu -gpu=cc80```

### Results
We run LULESH for 20 iterations per execution. The results are shown in PVC and A100 subdirectories. \
GPU analytics were collected with NVIDIA Nsight Profiler for A100 and with ```LIBOMPTARGET_PLUGIN_PROFILE=T``` debugging option available in oneAPI for PVC.

### Running LULESH Demo on PVC
Watch a short demo on how to compile and run LULESH on PVC with oneAPI:

[![LULESH Demo on PVC](https://img.youtube.com/vi/IUOIF6rIvAE/0.jpg)](https://www.youtube.com/watch?v=IUOIF6rIvAE)

## References
<a id="1">[1]</a> 
Bercea, Gheorghe-Teodor, et al. "Performance analysis of OpenMP on a GPU using a CORAL proxy application." Proceedings of the 6th International Workshop on Performance Modeling, Benchmarking, and Simulation of High Performance Computing Systems. 2015.
