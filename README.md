# Bottleneck ResNet16D Family  

<div style="display: flex; gap: 10px; flex-wrap: wrap; margin-bottom: 10px;">  
    <img src="https://img.shields.io/github/license/AliKHaliliT/BResNet16D-Family" alt="License">  
    <img src="https://img.shields.io/github/last-commit/AliKHaliliT/BResNet16D-Family" alt="Last Commit">  
    <img src="https://img.shields.io/github/issues/AliKHaliliT/BResNet16D-Family" alt="Open Issues">  
</div>  
<br/>

This repository provides links to custom-improved variants of the ResNet16 architecture. 

BResNet16 variants are a set of architectures inspired by ResNet but designed with efficiency in mind. Unlike conventional ResNet models, which use basic residual layers (for ResNet-18 and ResNet-34) and bottleneck residual layers (for ResNet-50 and above), BResNet16 variants are optimized for lightweight performance, making it ideal for edge devices and performance-critical applications.

## Architectural Design
In traditional ResNet architectures:
- **Basic residual layers** stack two convolutional layers on the main path and one convolutional layer on the shortcut path.
- **Bottleneck residual layers** stack three convolutional layers on the main path, with the first and last layers being 1x1 convolutions (bottleneck layers) to reduce computation.

### Why "16"?
A conventional ResNet model has an input stem, four stages, and an output layer. Each stage typically contains at least two residual blocks, making it impossible to create standard 18 and 34 variants using only bottleneck layers. The closest possible variant is 16, hence the name **BResNet16 (Bottleneck Residual Network 16).**

The modifications build upon techniques from the paper ["Bag of Tricks for Image Classification with Convolutional Neural Networks"](https://arxiv.org/abs/1812.01187), along with additional optimizations and personal refinements.  

Each variant has specific modifications tailored to its use case. Details about these improvements can be found in their respective repositories.  

The "D" in the variant names originates from ResNet-D of the referenced paper, reflecting the inspirations and architectural changes applied in these models.  

## Variants  
- [BResNet16-1DD](https://github.com/AliKHaliliT/BResNet16-1DD)  
- [BResNet16-2DD](https://github.com/AliKHaliliT/BResNet16-2DD)  
- [BResNet16-3DD](https://github.com/AliKHaliliT/BResNet16-3DD)  
- [BResNet16-2Plus1DD](https://github.com/AliKHaliliT/BResnet16-2Plus1DD)