# GPT_Prompt_Generator
To generate gpt prompt automatically and a ranking is given based on the scores.

微信小程序：AI爱家 | ELO score | Prompt 自动化生成

## 概述

Prompt的本质是调整任务格式去迎合我们的LLM(Large Language Model), Prompt 采取类似完形填空的策略，这要求模型具备一些序列语义信息。而对于Prompt Tuning往往需要人工撰写大量prompt，测试过程耗时费力且不好评估。这里提出了一种基于ELO评分的prompt自动化生成方法，本质上是调用`gpt-4`或`gpt-3.5-turbo`模型


[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/catundchat/gpt_prompt_generator/blob/main/gpt_prompt_generator.ipynb)
