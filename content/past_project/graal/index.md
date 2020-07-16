---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "GPU-Acceleration for the Graal VM"
summary: ""
authors: [ChristopheDubach, MichelSteuwer, JuanFumero]
tags: []
categories: []
date: 2019-11-04T15:43:15Z

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

This project aims at automatically accelerating applications running on top of the Graal VM, an Open source Java VM.
To achieve this goal we first define a high-level API inspired by functional programming and data-flow programming concepts.
At runtime, our system recognises the calls to our API and automatically generate OpenCL kernels.
The runtime then manages the execution of this OpenCL kernel on multiple devices (e.g. GPU) which results in the application being transparently accelerated.

Supported by {{< figure src="o_labs_clr2.jpg" title="Oracle Labs" lightbox="true" >}}