---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Aigis密钥封装算法多平台高效实现与优化"
authors: [admin, Feng He, Yunlei Zhao]
date: 2021-10-01T22:14:49+08:00
doi: "10.7544/issn1000-1239.2021.20210617"

# Schedule page publish date (NOT publication's date).
publishDate: 2021-10-01T22:14:49+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "计算机研究与发展"
publication_short: ""

abstract: 量子计算技术快速发展带来的新挑战使得后量子密码(post-quantum cryptography, PQC)成为当前密码学界研究热点.基于格的密码方案因其安全高效的特性,已经成为后量子公钥密码的主流之一.Aigis密钥封装算法(Aigis-enc)是我国学者自主设计的基于模格上非对称错误学习(A-MLWE)问题的后量子密码算法,是中国密码学会举办的全国密码算法设计竞赛公钥密码算法一等奖获奖算法之一.为了应对量子攻击,维护国家网络空间的长远安全,为未来国家后量子密码算法标准的制定和实际部署贡献力量,对我国自行研发的优秀后量子密码算法进行优化具有重要意义.工作重点关注Aigis-enc算法在不同平台的实现优化,包含高性能平台的快速并行实现与嵌入式低功耗平台的紧凑实现.具体而言,运用单指令多数据流(single instruction multiple data, SIMD)指令,充分优化了Aigis-enc现有AVX2实现,并提供了其首个ARM Cortex-M4平台的轻量级紧凑实现.实现包含4个关键优化点:降低Montgomery约减与Barrett约减汇编指令数目,提升了约减效率;使用裁剪层数的数论变换并优化指令流水调度,加速多项式乘法运算并减少了预计算表存储需求;提供了多项式序列化与反序列化的并行汇编指令实现,加快了编码解码与加解密过程;结合on-the-fly计算与空间复用优化算法存储空间.实验结果表明:提出的优化技术在8核Intel Core i7处理器上可将Aigis-enc算法原始AVX2实现提升25%,且大幅减少了其在ARM Cortex-M4平台的预计算表存储、代码尺寸与运行堆栈占用,对算法的实际应用有重要现实意义.

# Summary. An optional shortened abstract.
summary: ""

tags: [PQC]
categories: []
featured: false

# Custom links (optional).
#   Uncomment and edit lines below to show custom links.
# links:
# - name: Follow
#   url: https://twitter.com
#   icon_pack: fab
#   icon: twitter

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
