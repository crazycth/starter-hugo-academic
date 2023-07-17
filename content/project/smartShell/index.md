---
title: smartShell
summary: SmartShell is used to help you easily write very complex shell commands within the shell, and requires support from OpenAI-ChatGPT.
tags:
  - chatGPT
date: '2023-05-27T00:00:00Z'

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
    url: https://github.com/crazycth/smartShell
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
# SmartShell💊

SmartShell is used to help you easily write very complex shell commands within the shell, and requires support from OpenAI-ChatGPT.

develop with [@uni-zhuan](https://github.com/uni-zhuan)

1. set your environmental variable : OPENAI_API_KEY (export OPENAI_API_KEY=XXX)
2. git clone https://github.com/crazycth/smartShell.git
3. cd smartShell && bash install.sh (install with pip3)

```
(base) ➜ [/Users/richard] help 查找当前目录下所有以.py结尾的文件，提取到当前目录的上一层
find . -name '*.py' -exec mv {} .. \;
```

Note : The shell command has been pasted into the clipboard, just use command+v to paste it