---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "OSKR/OKAI: Systematic Optimization of Key Encapsulation Mechanisms from Module Lattice"
authors: [admin, Feng He, Zhichuang Liang, Yang Wang, Yunlei Zhao]
date: 2021-09-07T22:26:06+08:00
doi: "10.48550/arXiv.2109.02893"

# Schedule page publish date (NOT publication's date).
publishDate: 2021-09-07T22:26:06+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: |-
  In this work, we make *systematic* optimizations of key encapsulation mechanisms (KEM) based on module learning-with-errors (MLWE), covering algorithmic design, fundamental operation of number-theoretic transform (NTT), approaches to expanding encapsulated key size, and optimized implementation coding. We focus on Kyber (now in the Round-3 finalist of NIST PQC standardization) and Aigis (a variant of Kyber proposed at PKC 2020). 
  By careful analysis, we first observe that the algorithmic design of Kyber and Aigis can be optimized by the mechanism of asymmetric key consensus with noise (AKCN) proposed in \cite{JZ16,JZ19}. Specifically, the decryption process can be simplified with AKCN, leading to a both faster and less error-prone decryption process. Moreover, the AKCN-based optimized version has perfect compatibility with the deployment of Kyber/Aigis in reality, as they can run on the same parameters, the same public key, and the same encryption process. 
  We make a systematic study of the variants of NTT proposed in recent years for extending its applicability scope, make concrete analysis of their exact computational complexity, and in particular show their equivalence. We then present a new variant named hybrid-NTT (H-NTT), combining the advantages of existing NTT methods, and derive its optimality in computational complexity. The H-NTT technique not only has larger applicability scope but also allows for modular and unified implementation codes of NTT operations even with varying module dimensions. 
  We analyze and compare the different approaches to expand the size of key to be encapsulated (specifically, 512-bit key for dimension of 1024), and conclude with the most economic approach. To mitigate the compatibility issue in implementations we adopt the proposed H-NTT method.

# Summary. An optional shortened abstract.
summary: ""

tags: [PQC]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- name: arXiv
  url: https://arxiv.org/abs/2109.02893
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
