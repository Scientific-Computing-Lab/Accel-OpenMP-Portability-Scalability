### LULESH Pefromance Scalability on Intel PVC and NVIDIA A100 GPUs

The LULESH version we run supports OpenMP 4.0 offloading and is available in https://github.com/AMDComputeLibraries/OpenMPApps/tree/master/lulesh-mp4.

#### Compilation flags for PVC with oneAPI (icx 2023):
```-Ofast -qopenmp -fopenmp-targets=spir64 -fiopenmp ```
#### Compilation flags for PVC with oneAPI (gcc 12.2.0):
```-Ofast -fopenmp -foffload='-lm -latomic'```

### Results
The results are shown in PVC and A100 subdirectories. \
GPU analytics were collected with NVIDIA Nsight Profiler for A100 and with ```LIBOMPTARGET_PLUGIN_PROFILE=T``` debugging option available in oneAPI for PVC.
