---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "High-Level Synthesis of Neural Networks on FPGAs"
summary: ""
authors: [ChristopheDubach, ChristofSchlaak, AndrejIvanis]
tags: []
categories: []
date: 2019-11-04T15:50:41Z

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

Many modern applications that perform classification, prediction or clustering employ Neural Networks (NN) for these tasks. They are often used in datacenters or mobile devices, where high performance and energy-efficiency is crucial. Due to their parallelity, GPUs bring a big performance improvement (in comparison to CPUs) for these applications. Nevertheless, they still have a limitation in their fixed architecture. Especially, because the field is changing quickly and fast innovation must be made possible.

Field-Programmable Gate Arrays (FPGAs) offer more flexibility and can specialise the architecture design to the specific neural network application in order to archive the best performance. Furthermore they are highly energy-efficient and are therefore well suited for NNs in embedded systems or large scale server clusters.

However, deploying neural networks on FPGAs (like programming parallel accelerators in general), with focus on high performance, is a complex step. Due to their flexible architecture, FPGAs allow for so many options for tweaking the performance but in return require a lot of hardware specific expertise and take costly development time to be configured properly. Rather than manual development, automation should take place here to accelerate the development process and also drive down costs. Furthermore, developers do not want to manually adapt their implementations for various accelerators (e.g. CPU, GPU, FPGA). Instead, performance portability is desirable.

Lift addresses these challenges by offering a high-level functional, data-parallel language, which allows the user to efficiently develop an application independently of the target hardware platform. Then, rewrite rules in the Lift compiler open a vast design space of possible implementations for this abstract system specification. This design space is explored to find a suitable solution, which satisfies the performance and energy requirements. In order to exploit the parallel structure of NNs, the compiler employs pipelining mechanisms and allocates distributed on-chip memory on the FPGA. Timing behaviour and scheduling is introduced until finally a Hardware description language (HDL) code is emitted, that can be used to generate the bitstream for the FPGA.

Supported by {{< figure src="Microsoft_Research_logo.jpg" title="Microsoft Research" lightbox="true" >}}
