# Single GPU Passthrough (for Nvidia GPUs) Arch Linux

Passing through your primary GPU from your host OS to a Windows 10 VM

## Contents:

1. Introduction
2. Credits
2. Hardware and Software
3. Preparation
4. Hooks
5. Setting up a VM
6. GPU Passthrough Settings and Setup
7. Starting VM with GPU passthrough
11. Tips and Tricks

## Introduction

This tutorial walks you through how to passthrough your boot GPU to a guest machine on Arch Linux, this tutorial will work on other distros, I'm just using Arch for this tutorial.

## Credits

<b>[Chirjonit] for inspiring me to create a VM when I was still running Pop! OS. [Single-GPU-Passthrough](https://github.com/chironjit/single-gpu-passthrough/blame/master/README.md)</b>

## Hardware and Software

This is my hardware setup:

```
  CPU: i5-4570
  MB: HP Generic
  RAM: 16GB
  Main Storage: 240GB SSD
  Secondary Storage: 500GB HDD
  Game Storage: 2TB HDD
  GPU: NVIDIA GTX 1650
```

Monitor:

```
  MSI Optix G27C2 attached to NVIDIA GPU
```

Software: <br />

Install of Arch Linux updated using `sudo pacman -Syu`<br />
Downloaded Windows 10 Version (21H2) ISO

## Preparation

### Enable Virtualization in Bios

The first and most important step is to make sure that virtualization is enabled in your bios.
