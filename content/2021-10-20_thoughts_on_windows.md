---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
author: David Marx
date: '2021-10-20'
---

# Some thoughts on Windows

> {sub-ref}`today` | {sub-ref}`wordcount-words` words | {sub-ref}`wordcount-minutes` min read

Microsoft is making a big effort to position themselves as an ML driven company. But somehow, windows remaines basically incompatible with ML.

## The Machine

For a long time I've been resisting investing in a computer I could use for serious ML. A few weeks ago I gave in and treated myself to [high-end pre-built gaming PC](https://www.newegg.com/abs-ali511/p/N82E16883360111?Item=N82E16883360111&utm_medium=TraEmail&utm_source=TEMC-Shipping-New-Tracking-Notification-Responsive-US&cm_mmc=TEMC-Shipping-New-Tracking-Notification-Responsive-US-_-N82E16883360111), 
complete with an RTX 3090 graphics card -- undoubtedly the highest-end consumer grade GPU currently on the market boasting NVIDIA's new Ampere architecture and a 
whopping 24GB VRAM. Here are a few key specs on this beast:

| Type | Part | Notes |
|:---|:---|:---|
| CPU | Intel i9 10850K | With a respectable 10 cores and 20 threads, this processor is nothing to shake a stick at. Released mid 2020, it was [raved](https://www.techradar.com/news/intel-core-i9-10850k-is-unleashed-but-10-core-comet-lake-cpu-might-not-be-as-affordable-as-you-hoped) as a "beast" and one of the fastest gaming processors available. Suffice it to say, it is powerful and the technology is current. |
| Storage | 1 TB SSD (M.2 NVMe)| Much faster data transfer than conventional HDD with a spinning magnetic platter |
| RAM | 2x 32 GB cards (64GB total) | Lots of RAM so I can work with large datasets |
| GPU | RTX 3090 | undoubtedly the highest-end consumer grade GPU currently on the market boasting NVIDIA new Ampere architecture |
| VRAM | 24 GB | The main reason I got the 3090. Need lots of VRAM to accomodate large models like transformers |

Yes, this machine was designed to be a gaming PC, bit those specs position it to be a fairly powerful ML workstation as well. It would be nice if it had multiple GPUs, 
but you gotta pick your battles so I went with the one monster GPU and I think I made the right choice. 

The computer came with windows pre-installed, and I decided to give it a chance. After all, I worked at Microsoft when I bought the thing, I should be "dogfooding" our 
products. Microsoft had been boasting about the windows ML runtime and WSL integration so I figured it was worth giving windows a chance. 

## Problem 1: WSL

- No CUDA-enabled containers.
- No JAX.
- No RAPIDS.

## Problem 2: Windows Update

- No long running jobs.
- Don't feel like I'm in control of my own machine

## Problem 3: Unnecessary limitations

- E.g. No RDP.
