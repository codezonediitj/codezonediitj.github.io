---
layout: post
title:  "CPU, GPU and TPU in Deep Learning"
date:   2019-05-30
author: "Anukriti Jha"
excerpt: "GPU (Graphical Processing Unit) is one of the most widely used processing unit used in training data models. It is a single processor chip which frees the CPU cycles from jobs of image processing and mathematical computations. For example, a game with a lot of graphics: many shadows to cast, lots of atmospheric effects, various lighting sources, complex textures, etc."
image: "/images/benchmark-cpu-gpu.png"
is_pinned: false
---

GPU (Graphical Processing Unit) is one of the most widely used processing unit used in training data models. It is a single processor chip which frees the CPU cycles from jobs of image processing and mathematical computations. For example, a game with a lot of graphics: many shadows to cast, lots of atmospheric effects, various lighting sources, complex textures, etc. All these eat up extra GPU processing. Also, settings at higher resolutions means each single frame needs more such calculations to just display each pixel on that frame. Everything is handled by the GPU. When the GPU cannot remain at par with the CPU, it causes bottlenecks.

#### Some stark differences between CPU and GPU

CPU processes data sequentially whereas a GPU has several threads running simultaneously. A GPU thus utilizes parallel computing to increase the speed of training models.

CPU assigns Graphics rendering, vector computations and other complex tasks to the GPU.

GPUs are bandwidth optimized whereas CPUs are latency time (memory access time) optimized.

In deep learning, the host code is run on the CPU and the CUDA code runs on GPU. Serial workload is handled by the CPU and offload parallel computation is handled by GPU.

Due to large datasets, the CPU takes up a lot of memory while training the model. The standalone GPU, on the other hand, comes with a dedicated VRAM memory. Thus, CPU’s memory can be used for other tasks. Computing huge and complex jobs takes up a lot of clock cycles in CPU. The reason being, CPU takes up the jobs sequentially and it has a fewer number of cores than its counterpart, GPU.

The High bandwidth, hiding the latency under thread parallelism and easily programmable registers makes GPU a lot faster than a CPU.

#### The new Intel Xeon phi processing chip

It fetches and decodes instructions from four hardware thread execution contexts and has 4 clock latency, hidden by round-robin scheduling of threads. Each microprocessor core is a fully functional, in-order core capable of running IA instructions independently of the other cores. It has two pipelines and ring interconnection.

#### The TPU chip

The chip has been specifically designed for Google's TensorFlow framework. In Google Photos, an individual TPU can process over 100 million photos a day. Google's Cloud TPU is currently only in beta, offering limited quantities and usage. In machine learning training, the Cloud TPU is more powerful in performance and four times larger in memory capacity than Nvidia's best GPU Tesla V100.

Concluding, ML and DL is very much dependent on the three pillars of computer engineering, OS, Computer Organization and Architecture and Compiler Design. While general-purpose computing is still the CPU’s domain, GPUs are the hardware backbone of nearly all intensive computational applications.
