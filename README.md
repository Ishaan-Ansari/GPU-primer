## GPU-primer

1. **CUDA** (by Nvidia, so only runs on NVIDIA GPUs) and **OpenCL** (open source) are softwares for efficient management of threads on the GPUs.


2. CUDA has two primary APIs, so we have two corresponding versions
    * **Driver API** -- installed by GPU driver installer -- includes *libcuda.so*, etc.
    * **Runtime API** -- installed by cuda-toolkit installer -- includes *libcudart.so*, *nvcc*, etc.


3. Code snippets for GPU inspections 
    ```bash
    lspci | grep -i nvidia
    nvidia-smi -L    # displays gpus full name
    ```

4. NVIDIA GPU Architecture and Compute Capability:

    * [https://arnon.dk/matching-sm-architectures-arch-and-gencode-for-various-nvidia-cards/](https://arnon.dk/matching-sm-architectures-arch-and-gencode-for-various-nvidia-cards/)

    * [nvidia official](https://developer.nvidia.com/cuda-gpus)

    * [stackoverflow answer](https://stackoverflow.com/questions/28932864/which-compute-capability-is-supported-by-which-cuda-versions/28933055#28933055)

5. GPU comparisons

    * [https://fullstackdeeplearning.com/cloud-gpus/](https://fullstackdeeplearning.com/cloud-gpus/)

    * [https://lambdalabs.com/gpu-benchmarks](https://lambdalabs.com/gpu-benchmarks)
