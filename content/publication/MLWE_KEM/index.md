---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "基于模格的密钥封装方案的比较分析与优化"
authors: [Yang Wang, admin, Yunlei Zhao, Mingqiang Wang]
date: 2020-10-01T22:30:27+08:00
doi: "10.7544/issn1000-1239.2020.20200452"

# Schedule page publish date (NOT publication's date).
publishDate: 2020-10-01T22:30:27+08:00

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: "计算机研究与发展"
publication_short: ""

abstract: |-
  到目前为止, 不使用复杂纠错码的基于模 LWE LWR 问题设计的高效密钥封装方案主要有 2 类: 1) 如 Kyber, Aigis 和 Saber 直接基于 (对称或非对称) 模 LWE LWR 问题设计; 2) 如 AKCN-MLWE 和 AKCN-MLWR 基于密钥共识机制结合模 LWE LWR 问题设计. 一般来说, 在满足一定安全性和实现效率的基础上, 实际应用中构造的密钥封装方案会通过压缩一些通信比特来达到节省通信带宽的目的. 据作者所知, 现存文献的关注点一般集中在详细分析对应某具体参数条件下密码体制的安全性, 还没有文献系统地分析上述 2 类构造方式的异同以及采用相同 (或不同) 压缩函数情况下不同参数选择与错误率的关系. 从理论上系统地比较了直接基于 LWE LWR 构造的密钥封装方案和基于密钥共识机制结合模 LWE LWR 问题设计的密钥封装方案的异同, 并从理论分析和实际测试 2 方面证明了当采用相同的压缩函数和相同的参数设置时, AKCN-MLWE 采用的构造方式要优于 Kyber 采用的构造方式, 而 Saber 采用的构造方式本质上与 AKCN-MLWR 是相同的. 针对 Kyber-1024 这一组参数对应的安全强度, 还详细分析了 3 种封装 512 b 密钥长度的方法. 根据理论分析和大量的实验测试, 给出了 AKCN-MLWE 和 AKCN-MLWR 的新的优化建议和参数推荐, 也给出了对于 Aigis 和 Kyber 的优化方案 (对应的命名为 AKCN-Aigis 和 AKCN-Kyber) 和新的参数推荐.

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
