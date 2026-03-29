GPU-Based Image Noise Reduction using CUDA Median Filter

Overview
This project implements median filter based image denoising using:

* CPU (C++)
* GPU (CUDA)

The program removes salt-and-pepper noise from grayscale images and demonstrates how GPU acceleration can improve performance for image processing tasks.

Requirements

* NVIDIA GPU
* CUDA Toolkit installed
* nvcc compiler
* g++

Compilation

Compile CPU version:

```bash
g++ cpu_version.cpp -o cpu
```

Compile GPU version:

```bash
nvcc gpu_version.cu -o gpu
```

Execution

Run CPU:

```bash
./cpu 
```

Run GPU:

```bash
./gpu image
```

Expected Output

* Execution time printed in milliseconds
* Output filtered image saved as `output_cpu.pgm` and `output_gpu.pgm`
* Improved image quality after noise reduction
