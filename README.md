# Efficient Neural Networks (NN) Project

Our project is divided into several sections, each focusing on a different aspect of efficient neural networks. Here's an overview of each section:
there gonna be several situaiton to build efficient model. 

## Section 1: Efficient Model.
In this section, we compare various computer vision models for image classification benchmarks, such as ImageNet1K and CIFAR100. We evaluate the models based on several metrics, including latency, throughput (across various devices like cloud GPUs [A100], CPUs, and mobile devices), GFLOPs, GMACs, and the number of parameters. This analysis is inspired by the findings in "Paper Title", specifically replicating Figure 1 and Table 1 from the paper. 

**Figure 1. Reimplementation of [Paper Title] Figure 1.**

<p float="left">
  <img src="/images/efficient_vit_fig1.png" width="48%" height="300px"/>
  <img src="/images/efficient_vit_fig1_rei.png" width="48%" height="300px" />
</p>

                  Efficient Vit Figure 1.                                               Our Replication

This figure is a major figure for papers that are reporting their efficient model. Both figures get throughput via TensorRT. In our reimplementation, which is on the left, we use an A100 GPU, batch size 64, and TensorRT version 8.6.1. As a result, it slightly differs from the original report. We didn't include EfficientNetV2 because its accuracy is obtained from other resolutions like 382, 480, not 224, and ConvNext performs better than CoatNet. However, in the original paper, CoatNet achieved better throughput than ConvNext.


## Section 2: Exporting Models and Measuring Latency
We'll provide a detailed tutorial on how to export models to different devices and measure their latency. This section aims to guide users through the practical aspects of deploying efficient neural networks.

## Section 3: Implementation of Quantization
In this part, we will explore quantization techniques and their impact on neural network performance. We're in the process of selecting relevant papers to base our experiments on.

## Section 4: Combining Knowledge Distillation, Pruning, and Quantization
Here, we focus on further improvements through a combination of knowledge distillation, pruning, and quantization. This section aims to push the boundaries of efficiency in neural networks.

## Section 5: Training Efficiency
The final section delves into training efficiency, exploring methods such as pre-training and architectural innovations like Mixture of Experts (MoE). We'll examine how these methods can be

![Example Image](/images/acc_latency_3060.png "Example Image Titl")
