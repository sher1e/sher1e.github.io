---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "cuXCMP: CUDA-Accelerated Private Comparison Based on Homomorphic Encryption"
authors: [Hao Yang, admin, Zhe Liu, Yunlei Zhao]
date: 2023-04-11T10:56:33+08:00
doi: "10.1109/TIFS.2023.3267677"

# Schedule page publish date (NOT publication's date).
publishDate: 2023-04-11T10:56:33+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "IEEE Transactions on Information Forensics and Security"
publication_short: "TIFS"

abstract: Private comparison schemes constructed on homomorphic encryption offer the noninteractive, output expressive and parallelizable features, and have advantages in communication bandwidth and performance. In this paper, we propose cuXCMP, which allows negative and ﬂoat inputs, offers fully output expressive feature, and is more extensible and practical compared to XCMP (AsiaCCS 2018). Meanwhile, we introduce several memory-centric optimizations of the constant term extraction kernel tailored for CUDA-enabled GPUs. Firstly, we fully utilize the shared memory and present compact GPU implementations of NTT and INTT using a single block; Secondly, we fuse multiple kernels into one AKS kernel, which conducts the automorphism and key switching operation, and reduce the grid dimension for better resource usage, data access rate and synchronization. Thirdly, we precisely measure the IO latency and choose an appropriate number of CUDA streams to enable concurrent execution of independent operations, yielding a constant term extraction kernel with perfect latency hide, i.e., CTX. Combining these approaches, we boost the overall execution time to optimum level and the speedup ratio increases with the comparison scales. For one comparison, we speedup the AKS by 23.71$\times$, CTX by 15.58$\times$, and scheme by 1.83$\times$ (resp., 18.29$\times$, 11.75$\times$, and 1.42$\times$) compared to C (resp., AVX512) baselines, respectively. For 32 comparisons, our CTX and scheme implementations outperform the C (resp., AVX512) baselines by 112.00$\times$ and 1.99$\times$ (resp., 81.53$\times$ and 1.51$\times$).

# Summary. An optional shortened abstract.
summary: ""

tags: [GPU, FHE]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
links:
- name: ePrint
  url: https://eprint.iacr.org/2022/1621
- name: IEEE Xplore
  url: https://ieeexplore.ieee.org/document/10121630

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
