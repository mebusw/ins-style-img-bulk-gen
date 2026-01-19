---
name: ins-style-img-bulk-gen
description: bulk generate instagram style images by combining elements
allowed-tools: Read, Bash
---


## Task

1. 理解元素清单 `./references/ins-style-elements.md`
2. 搭配新的提示词文案。如果用户没有指定数量，则默认搭配5套文案。每个文案从元素清单中随机选5个元素，每一类最多1个。
3. 遍历上述提示词队列，并发地调用其他可用的image generation Skill 进行生图
4. 下载所有生成的图片，保存到 `~/Download/ins-image-{timestamp}/`