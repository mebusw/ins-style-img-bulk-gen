---
name: ins-style-img-bulk-gen
description: bulk generate instagram style images by combining elements
allowed-tools: Read, Bash
---


## Task

1. 理解元素清单 `./references/ins-style-elements.md`
2. 搭配新的提示词文案。如果用户没有指定数量，则默认搭配5套文案。默认每个文案从元素清单中随机选12个元素，每一类1-2个。
3. 遍历上述提示词队列，并发地调用其他可用的image generation Skill 进行生图。注意生图是整个流程的一部分，你必须在 image generation Skill 执行完成后，返回本流程，并执行后续步骤
4. 将生成的图片保存到 `~/Download/ins-image-{timestamp}/`