# Accel-OpenMP-Portability-Scalability

Over the last decade, most of the increase in computing
power has been gained by advances in accelerated many-core architec-
tures, mainly in the form of GPGPUs. While accelerators achieve phe-
nomenal performances in various computing tasks, their utilization re-
quires code adaptations and transformations. Thus, OpenMP, the most
common standard for multi-threading in scientific computing applica-
tions, introduced offloading capabilities between host (CPUs) and accel-
erators since v4, with increasing support in the successive v4.5, v5.0, v5.1,
and the latest v5.2 versions. Recently, two state-of-the-art GPUs – the
Intel Ponte Vecchio Max and the NVIDIA A100 GPUs – were released
to the market, with the oneAPI and GNU LLVM-backed compilation for
offloading, correspondingly. In this work, we present early performance
results of OpenMP offloading capabilities to these devices while specif-
ically analyzing the potability of advanced directives (using SOLLVE’s
OMPVV test suite) and the scalability of the hardware in representative
scientific mini-app (the LULESH benchmark). Our results show that the
vast majority of the offloading directives in v4.5 and 5.0 are supported in
the latest oneAPI and GNU compilers; however, the support in v5.1 and
v5.2 is lacking. From the performance perspective, we found that PVC
is up to 1.6x better than the A100 on the LULESH benchmark.
