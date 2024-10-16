---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: resume-biography
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text:
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: tom-ritson-syGe7e2gKG0-unsplash.jpg
          filters:
            brightness: 0.4
          size: cover
          position: center
          parallax: false
  - block: stats
    content:
      items:
        - statistic: "16"
          description: |
            Publications
        - statistic: "64"
          description: |
            Citations
        - statistic: "5"
          description: |
            h-index
    design:
      # Section background color (CSS class)
      css_class: "bg-gray-100 dark:bg-gray-900"
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: markdown
    content:
      title: 'Welcome 👋'
      subtitle: ''
      text: |
        I am **Shiyu Shen** (**沈诗羽**). I received my PhD degree from Fudan University, supervised by Prof. Yunlei Zhao. My research interests include post-quantum cryptography, homomorphic encryption, and cryptographic engineering. I have published in journals and conferences including _IEEE Transactions on Computers_ (TC), _IEEE Transactions on Information Forensics and Security_ (TIFS), _IEEE Transactions on Dependable and Secure Computing_ (TDSC), _IEEE Transactions on Information Theory_ (TIT), and _the Annual Computer Security Applications Conference_ (ACSAC). I also serve as reviewer for publications including _IEEE Transactions on Information Forensics and Security_ (TIFS), _Nature Scientific Reports_, _Designs, Codes and Cryptography_ (DCC), _IEEE Internet of Things Journal_ (IoTJ), and _Journal of Cryptographic Engineering_ (JCE).
    design:
      columns: '1'
  # - block: collection
  #   content:
  #     title: Recent News
  #     subtitle: ''
  #     text: ''
  #     # Page type to display. E.g. post, talk, publication...
  #     page_type: post
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: date-title-summary
  #     # Reduce spacing
  #     spacing:
  #       padding: [0, 0, 0, 0]
---
