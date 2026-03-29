## GPU-Based Image Noise Reduction using CUDA Median Filter

## Overview
This project implements median filter based image denoising using:

* CPU (C++)
* GPU (CUDA)

The program removes salt-and-pepper noise from grayscale images and demonstrates how GPU acceleration can improve performance for image processing tasks.

## Requirements

* NVIDIA GPU
* CUDA Toolkit installed
* nvcc compiler
* g++

Compilation

## Compile CPU version:

```bash
g++ cpu_version.cpp -o cpu
```

## Compile GPU version:

```bash
nvcc gpu_version.cu -o gpu
```

Execution

Run CPU:


./cpu
<img width="257" height="34" alt="image" src="https://github.com/user-attachments/assets/8f467f9c-d534-4855-9d0b-ea0c9c27cc51" />



Run GPU:


./gpu
<img width="1698" height="60" alt="image" src="https://github.com/user-attachments/assets/b40ac142-5c7c-462b-afe9-513c52eb0091" />



## Expected Output
![GPU image](https://github.com/user-attachments/assets/2ea1f015-0e5d-4252-a373-ba845e2ef375)

* Execution time printed in milliseconds
* Output filtered image saved as `output_cpu.pgm` and `output_gpu.pgm`
* Improved image quality after noise reduction
