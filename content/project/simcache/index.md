---
title: simcache
summary: A simple golang implementation of groupCache
tags:
  - golang
date: '2023-02-27T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
#   caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
#   - icon: twitter
#     icon_pack: fab
#     name: Follow
#     url: https://twitter.com/georgecushen
  - icon: github
    icon_pack: fab
    name: github
    url: https://github.com/crazycth/simcache
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

# simcache

* LRU缓存淘汰策略
* 单机并发缓存
* HTTP服务端
* 一致性哈希与分布式节点
* 防止缓存击穿 & 缓存穿透
* protobuf通信



![avatar](featured.jpg)




待优化

* sync.mu性能不如sync.map，可将锁机制替换为sync.map，但存在缓存击穿问题，想想怎么省去一些锁
* simcache与httppool虽实现上解耦，但用接口实现关联的方式不太优雅
* 一致性哈希在各节点各自维护，添加节点时所有节点均需更新hash信息，思考能否抽象出hash层，所有节点共用一个hashmap
* 缓存击穿实现上用了太多锁，严格保证了串行化，思考是否能提高效率

