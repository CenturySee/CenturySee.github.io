---
title: "关于Claude，你应该知道的十件事"
date: 2023-04-15T13:08:40+08:00
draft: false
author: AK27
tags:
    - Claude
    - LLM
---

1. Claude是Anthropic公司开发的大语言模型(LLM)，主要特点是有用与可信（helpful and trustworthy）  

2. Anthropic成立于2021年，是一家人工智能安全和研究公司，致力于建立可靠的、可解释的、可操纵的人工智能系统，公司的创始团队来自于OpenAI  

3. Claude提供了两种访问方式，API和Slack机器人  

4. API访问方式需要申请并等待通过，通过后测试时的并发限制为1，用于[生产时需要与Anthropic协商具体限速](https://console.anthropic.com/docs/api/errors#rate-limits)  

5. Claude目前有两个版本，一个是**功能强大的版本Claude**，擅长于从复杂的对话和创造性的内容生成到详细的指令跟随的广泛任务；一个是**速度更快，价格更优的Claude Instant**，它也可以处理随意对话、文本分析、摘要和文档问答  

6. 两个版本的Claude[prompt与output分开计费](https://cdn2.assets-servd.host/anthropic-website/production/images/FINAL-PRICING.pdf)，能够处理内容的最长长度、收费标准具体如下：  

| 模型名称 | 最长长度（tokens） | prompt价格（美元/1000） | output价格（美元/1000） |
| --- | --- | --- | --- |
| Claude-Instant | 9000 | 0.00043 | 0.00145 |
| Claude | 9000 | 0.0029 | 0.0086 |
| ChatGPT | 4096 | 0.002 | 0.002 |

> 注：Claude的价格单位为character，ChatGPT的价格单位为token

7. 与ChatGPT类似，**Claude能够处理多语言、不能联网**；支持个性化finetune，但需要与Authropic联系  

8. Claude目前不支持embedding，Anthropic推荐使用SBERT生成句子embedding  

9. Claude in Slack目前是beta版本，不收费  

10. [Claude目前存在一些缺陷](https://www.anthropic.com/claude-in-slack)，包括以下几点：  

> Claude对之前的对话没有任何记忆  
> Claude经常在复杂的算术和推理中出错  
> Claude有时会产生幻觉或编造信息和细节  
> Claude没有联网  
> Claude的训练数据是两年前的

更多可能有帮助的内容，请关注**算法工程笔记**公众号。 
