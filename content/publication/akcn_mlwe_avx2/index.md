---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "AKCN-MLWE算法AVX2高效实现"
authors: [Hao Yang, Zhe Liu, Junhao Huang, admin, Yunlei Zhao]
date: 2021-12-01T16:38:56+08:00
doi: "10.11897/SP.J.1016.2021.02560"

# Schedule page publish date (NOT publication's date).
publishDate: 2021-12-01T16:38:56+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "计算机学报"
publication_short: ""

abstract: "随着量子计算机的快速发展,经典密码系统面临巨大的威胁.Shor算法可以在量子计算机上多项式时间内分解大整数和求解离散对数,而这两类问题分别对应经典公钥密码系统中的RSA和椭圆曲线密码(ECC)所依赖的困难问题,因此可以抵御量子计算攻击的后量子密码近年来受到广泛的研究.格密码是后量子密码中最为高效且拓展性强的一类密码算法,在未来会逐步替代传统公钥密码算法(RSA、ECC等).256位高级向量扩展(AVX2)指令集是英特尔64位处理器中普遍支持的一类单指令多数据(SIMD)指令集,可用于并行计算.但是,由于格密码结构复杂,在支持AVX2指令集的英特尔64位处理器上难以对格密码方案进行高适配的深度优化.AKCN-MLWE算法是我国自主设计的基于模格上容错学习(MLWE)问题的格密码密钥封装(KEM)方案,是中国密码学会举办的公钥密码算法竞赛第二轮的获奖算法.本文基于256位高级向量扩展(AVX2)指令集设计了针对AKCN-MLWE算法的高效实现方案,包括以下几个关键优化点:针对多项式乘法,本文结合最优的数论变换(NTT)算法,将NTT的最后一层转换为线性多项式并使用Karatsuba算法进行加速计算,大幅提升计算效率的同时减少了预计算表的空间占用;针对取模运算,本文结合了Barrett约减算法和蒙哥马利约减算法的优势,同时采用延迟约减技术降低取模次数;本文针对所有多项式运算均实现了高度并行化,设计了针对多项式压缩与解压缩的并行算法,进一步提升了实现效率.本文设计的AKCN-MLWE算法AVX2高效实现方案在八核Intel Core i9-9880H处理器上仅需不到0.04毫秒即可完成一次完整的KEM(包括密钥生成、密钥封装和密钥解封装),相比于参考实现提升8.84倍,其中密钥生成提升7.07倍,密钥封装提升7.90倍,密钥解封装算法提升11.78倍.本文提出的AKCN-MLWE算法AVX2实现方案在相近经典经典安全强度下性能优于美国国家标准技术研究所(NIST)后量子密码标准化进程第二轮中众多格密码方案(Kyber、NewHope和Saber等).同时,本文设计的部分优化方案可用于提升Kyber、NewHope等格密码方案的性能."

# Summary. An optional shortened abstract.
summary: ""

tags: [PQC, AVX2]
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
