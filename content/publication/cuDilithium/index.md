---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "High-Throughput GPU Implementation of Dilithium Post-Quantum Digital Signature"
authors: [admin, Hao Yang, Wangchen Dai, Zhe Liu, Yunlei Zhao]
date: 2023-04-22T11:01:24+08:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2023-04-22T11:01:24+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: In this work, we present a well-optimized GPU implementation of Dilithium, one of the NIST post-quantum standard digital signature algorithms. We focus on warp-level design and exploit several strategies to improve performance, including memory pool, kernel fusing, batching, streaming, etc. All the above efforts lead to an efficient and high-throughput solution. We profile on both desktop and server-grade GPUs, and achieve up to 57.7$\times$, 93.0$\times$, and 63.1$\times$ higher throughput on RTX 3090Ti for key generation, signing, and verification, respectively, compared to single-thread CPU. Additionally, we study the performance in real-world applications to demonstrate the effectiveness and applicability of our solution.

# Summary. An optional shortened abstract.
summary: ""

tags: [GPU, PQC]
categories: []
featured: true

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- name: arXiv
  url: https://arxiv.org/abs/2211.12265
  # icon_pack: fab
  # icon: twitter

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
