---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "CUDA-Accelerated RNS Multiplication in Word-Wise Homomorphic Encryption Schemes"
authors: [admin, Hao Yang, Yu Liu, Zhe Liu, Yunlei Zhao]
date: 2022-05-23T11:01:16+08:00
doi: "10.1109/TC.2022.3227874"

# Schedule page publish date (NOT publication's date).
publishDate: 2022-05-23T11:01:16+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "IEEE Transactions on Computers"
publication_short: "TC"

abstract: Homomorphic encryption (HE), which allows computation over encrypted data, has often been used to preserve privacy. However, the computationally heavy nature and complexity of network topologies make the deployment of HE schemes in the Internet of Things (IoT) scenario difficult. In this work, we propose CARM, the first optimized GPU implementation that covers BGV, BFV and CKKS, targeting for accelerating homomorphic multiplication using GPU in heterogeneous IoT systems. We offer constant-time low-level arithmetic with minimum instructions and memory usage, as well as performance- and memory-prior configurations, and exploit a parametric and generic design, and offer various trade-offs between resource and efficiency, yielding a solution suitable for accelerating RNS homomorphic multiplication on both high-performance and embedded GPUs. Through this, we can offer more real-time evaluation results and relieve the computational pressure on cloud devices. We deploy our implementations on two GPUs and achieve up to 378.4$\times$, 234.5$\times$, and 287.2$\times$ speedup for homomorphic multiplication of BGV, BFV, and CKKS on Tesla V100S, and 8.8$\times$, 9.2$\times$, and 10.3$\times$ on Jetson AGX Xavier, respectively.

# Summary. An optional shortened abstract.
summary: ""

tags: [GPU, FHE]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- name: ePrint
  url: https://eprint.iacr.org/2022/633
- name: IEEE Xplore
  url: https://ieeexplore.ieee.org/document/9976229

url_pdf:
url_code:
url_dataset:
url_poster:
url_project:
url_slides:
url_source:
url_video:

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
