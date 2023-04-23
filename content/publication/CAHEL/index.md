---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Implementing and Benchmarking Word-Wise Homomorphic Encryption Schemes on GPU"
authors: [Hao Yang, admin, Wangchen Dai, Lu Zhou, Zhe Liu, Yunlei Zhao]
date: 2023-01-14T11:01:16+08:00
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: 2023-01-14T11:01:16+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: |-
  Homomorphic encryption (HE) is one of the most promising techniques for privacy-preserving computations, especially the word-wise HE schemes that allow batched computations over ciphertexts. However, the high computational overhead hinders the deployment of HE in real-word applications. The GPUs are often used to accelerate the execution in such scenarios, while the performance of different HE schemes on the same GPU platform is still absent.
  
  In this work, we implement three word-wise HE schemes BGV, BFV, and CKKS on GPU, with both theoretical and engineering optimizations. We optimize the hybrid key-switching technique, reducing the computational and memory overhead of this procedure. We explore several kernel fusing strategies to reuse data, which reduces the memory access and IO latency, and improves the overall performance. By comparing with the state-of-the-art works, we demonstrate the effectiveness of our implementation.
  
  Meanwhile, we present a framework that finely integrates our implementation of the three schemes, covering almost all scheme functions and homomorphic operations. We optimize the management of pre-computation, RNS bases and memory in the framework, to provide efficient and low-latency data access and transfer. Based on this framework, we provide a thorough benchmark of the three schemes, which can serve as a reference for scheme selection and implementation in constructing privacy-preserving applications.

# Summary. An optional shortened abstract.
summary: ""

tags: [GPU, FHE]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- name: ePrint
  url: https://eprint.iacr.org/2023/049

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
