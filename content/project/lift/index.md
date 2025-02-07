---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Lift"
summary: ""
authors: [admin,MichelSteuwer,LuLi,ThibautLutz,ToomasRemmelg,LarisaStoltzfus,FedericoPizzuti,NaumsMogers,AdamHarries]
tags: []
categories: []
date: 2014-09-04T15:40:33Z

# Optional external URL for project (replaces project detail page).
external_link: "http://www.lift-project.org"

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

Computing systems have become increasingly complex with the emergence of heterogeneous hardware combining multicore CPUs and GPUs.
These parallel systems exhibit tremendous computational power at the cost of increased programming effort. This results in a tension between performance and code portability.
This project investigates a novel approach aiming to combine high-level programming, code portability, and high-performance.
Starting from a high-level functional expression we apply a simple set of rewrite rules to transform it into a low-level functional representation close to the OpenCL programming model and from which OpenCL code is generated.
Our rewrite rules define a space of possible implementations which we automatically explore to generate hardware-specific OpenCL implementations.

#Supported by {{< figure src="Huawei.png" title="Oracle Labs" lightbox="true" >}}