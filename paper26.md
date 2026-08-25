
#  Topics, papers, and supervisors

## Topic 1: AI Safety 

- **Supervisor** Gert
- **Paper ** XXXXX

  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - **Link :** 
  - **Brief description :** 
  - **How to reproduce :**
  - **How to extend :** 

- **Supervisor** Summer
- **Paper ** XXXXX

  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - **Link :** 
  - **Brief description :** 
  - **How to reproduce :**
  - **How to extend :**
 
- **Supervisor** Abel
- **Paper ** Guard

  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - **Link :** 
  - **Brief description :** 
  - **How to reproduce :**
  - **How to extend :** 

## Topic 2 : Agentic Systems

- **Supervisor** Giulio

- **Paper** Think Twice Before You Act: Protecting LLM Agents Against Tool Description Poisoning via Isolated Planning

  * 👨‍🏫: ⭐

  * 🖥️: ⭐⭐⭐

  * **Link:** [Think Twice Before You Act: Protecting LLM Agents Against Tool Description Poisoning via Isolated Planning](https://openreview.net/forum?id=jiNw5AgBbw)

  * **Brief description:** LLM-based agents can interact with their environment through tools. These tools are supplied in context through their function definitions, argument schemas, return values, and natural-language descriptions. Because tools, skills, and MCP servers may be downloaded from or exposed by untrusted sources, an attacker can embed instructions in these descriptions. One class of attack subtly steers an agent’s trajectory towards different tool choices, making it less conspicuous than direct malicious-instruction injection. This work addresses tool-description poisoning attacks that steer an agent towards invoking otherwise benign tools. Tool-Guard classifies tool calls along two binary dimensions: aligned versus misaligned, and normal versus suspicious. Tools associated with calls classified as misaligned or suspicious are moved to an influenced list, over which planning is performed separately from the normal tool list.

  * **How to reproduce:** The code for this paper is fully available. You will reproduce **Experiment 1** or **Experiment 3** using two LLMs of your choice. One model must be self-hosted, while the other must be accessed through an inference provider. I can direct you towards suitable options depending on your available hardware and budget; free or low-cost options are also available. 

  * **How to extend:** Separated-planning defenses against prompt injection, tool or skill poisoning, and malicious MCP servers incur additional inference overhead. This overhead may itself be amplified by attacks such as the one proposed in [this paper](https://arxiv.org/pdf/2602.14798). As an extension, you should implement a small set of overthinking-inducing tools and evaluate whether Tool-Guard identifies them as suspicious or misaligned. If time permits, an extension of Tool-Guard that mitigates overthinking-inducing tools can also be explored.


-- **Supervisor** Zhiwen
- **Paper ** XXXXX

  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - **Link :** 
  - **Brief description :** 
  - **How to reproduce :**
  - **How to extend :** 


-- **Supervisor** Roberto
- **Paper ** XXXXX

  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - **Link :** 
  - **Brief description :** 
  - **How to reproduce :**
  - **How to extend :** 



## Topic : Structured Data Generation
- **Supervisor** Aditya
- **Paper** WaveStitch: Flexible and Fast Conditional Time Series Generation with Diffusion Models

  - 👨‍🏫: ⭐⭐
  - 🖥️: ⭐⭐
  
  - **Link :** https://dl.acm.org/doi/10.1145/3769842
  - **Brief description :** Traditional imputation and forecasting methods often require retraining or adapting separate models for different missingness ratios, observation positions, or forecasting scenarios. Another limitation is generating long time series sequences: conventional methods divide sequences into smaller windows and generate them sequentially, making inference increasingly slow as the horizon grows. WaveStitch overcomes the first limitation by training one universal model once and then guiding it at inference to handle arbitrary observation patterns and missing-value ratios, without scenario-specific retraining. High generation speed for long sequences is achieved via "stitching". Instead of generating windows sequentially, it generates multiple windows in parallel and progressively propagates synchronisation information through a pipelined process, ensuring global temporal coherence. The result is a scalable, flexible, and efficient framework that transforms time-series generation: one model, any missingness pattern, and fast generation of arbitrarily long sequences.
  - **How to reproduce :** Please follow the code repository of the paper: https://github.com/adis98/WaveStitch
  - **How to extend :** While The original paper focuses on time series generation, it would be interesting to see how well the concept of "stitching" generalises to generating other sequential data, specifically, languages. The goal would be to first understand and reproduce the original time series version, then experiment with language diffusion models, including masked diffusion, multinomial, or pure continuous architectures and adapt the stitching mechanism to these scenarios.

-- **Supervisor** Jeroen
- **General description :** 
- **Paper ** XXXXX

  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - **Link :** 
  - **Brief description :** 
  - **How to reproduce :**
  - **How to extend :** 




