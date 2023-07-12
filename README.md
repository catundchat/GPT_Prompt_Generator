# GPT_Prompt_Generator

To generate gpt prompt automatically and a ranking is given based on the scores.

微信小程序：AI爱家 | ELO评分 | Prompt自动化生成

## 概述

Prompt的本质是调整任务格式去迎合我们的LLM(Large Language Model), Prompt 采取类似完形填空的策略，这要求模型具备一些序列语义信息。而对于Prompt Tuning往往需要人工撰写大量prompt，测试过程耗时费力且不好评估。这里提出了一种基于ELO评分的prompt自动化生成方法，本质上是使用`gpt-4`或`gpt-3.5-turbo`模型能力，我们只需输入任务描述(description)和一些测试用例(test_case)，系统就会生成、测试和排序大量提示，以找到表现最好的提示。

## 配置

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/catundchat/gpt_prompt_generator/blob/main/gpt_prompt_generator.ipynb)

参数表如下:
```
config={
      "K": K,
      "system_gen_system_prompt": system_gen_system_prompt,
      "ranking_system_prompt": ranking_system_prompt,
      "candiate_model": CANDIDATE_MODEL,
      "candidate_model_temperature": CANDIDATE_MODEL_TEMPERATURE,
      "generation_model": GENERATION_MODEL,
      "generation_model_temperature": GENERATION_MODEL_TEMPERATURE,
      "generation_model_max_tokens": GENERATION_MODEL_MAX_TOKENS,
      "n_retries": N_RETRIES,
      "ranking_model": RANKING_MODEL,
      "ranking_model_temperature": RANKING_MODEL_TEMPERATURE,
      "number_of_prompts": NUMBER_OF_PROMPTS
      }
```
文件地址：`code/gpt_prompt_generator.ipynb` 和 `code/gpt_prompt_generator.py`

## 使用过程



