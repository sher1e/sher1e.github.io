---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Parallel Small Polynomial Multiplication for Dilithium: A Faster Design and Implementation"
authors: [Jieyu Zheng, Feng He, admin, Chenxi Xue, Yunlei Zhao]
date: 2022-12-05T11:01:16+08:00
doi: "10.1145/3564625.3564629"

# Schedule page publish date (NOT publication's date).
publishDate: 2022-12-05T11:01:16+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: "ACSAC '22: Proceedings of the 38th Annual Computer Security Applications Conference"
publication_short: "ACSAC '22"

abstract: |-
  The lattice-based signature scheme CRYSTALS-Dilithium is one of the two signature finalists in the third round NIST post-quantum cryptography (PQC) standardization project. For applications of low-power Internet-of-Things (IoT) devices, recent research efforts have been focusing on the performance optimization of PQC algorithms on embedded systems. In particular, performance optimization is more demanding for PQC signature algorithms that are usually significantly more time-consuming than PQC public-key encryption counterparts. For most cryptographic algorithms based on algebraic lattices including Dilithium, the fundamental and most time-consuming operation is polynomial multiplication over rings. For this computational task, number theoretic transform (NTT) is the most efficient multiplication method for NTT-friendly rings, and is now the typical technique for performing fast polynomial multiplications when implementing lattice-based PQC algorithms.
  
  The key observation of this work is that, besides multiplications of polynomials of standard forms, Dilithium involves a list of multiplications for polynomials of very small coefficients. Can we have more efficient methods for multiplying such polynomials of small coefficients? Under this motivation, we present in this work a parallel small polynomial multiplication algorithm to speed up the implementations of Dilithium. We complete both C reference implementation and ARM Neon implementation. Moreover, we conducted some speed tests in combination with Becker’s Neon NTT [4]. The results show that, in comparison with the C reference implementation of Dilithium submitted to the third round of the NIST PQC competition, our reference implementation with the proposed parallel small polynomial multiplication is faster: specifically, our Sign and Verify speed up 18% and 19% respectively for Dilithium-2 (30% and 7% for Dilithium-3, 27% and 3% for Dilithium-5, respectively). As for the Arm Neon implementation, we achieved a performance improvement of about 64% in Sign and 50% in Verify for Dilithium-2 (60% and 32% for Dilithium-3) compared with the C reference implementation of Dilithium submitted to the third round of the NIST PQC competition. We aslo compared our work with the state-of-the-art Arm Neon implementation of Dilithium [4], the results show our speed of Sign is 13.4% faster for Dilithium-2 and 8.0% faster for Dilithium-3, achieving a new record of fast Dilithium implementation.

# Summary. An optional shortened abstract.
summary: ""

tags: [PQC]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- name: ACM DL
  url: https://dl.acm.org/doi/10.1145/3564625.3564629

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
