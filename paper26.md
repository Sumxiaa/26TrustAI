
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

* **Supervisor:** Summer
* **Paper:** HulluEdit — Trustworthy Hallucination Mitigation in Large Vision-Language Models

  * 👨‍🏫: ⭐

  * 🖥️: ⭐⭐⭐

  * **Link:** [HulluEdit Paper](https://arxiv.org/abs/2602.22727)

  * **Brief description:** HulluEdit is a training-free, single-pass method for mitigating object hallucinations in large vision-language models. It decomposes hidden representations into orthogonal subspaces corresponding to visual evidence, conflicting language priors, and residual uncertainty, and selectively suppresses the latter components while preserving visual evidence.

  * **How to reproduce:** Reproduce the main hallucination-reduction results on POPE and CHAIR using one selected open-source LVLM, verify general capability on MME, and visualize how the visual-evidence, language-prior, and residual components change across layers and prompt conditions. Since HulluEdit requires neither model training nor an additional reference model, the main experiments can be conducted on a single H100 or 4090-class GPU.

  * **How to extend:** There are three promising directions. First, move from geometric orthogonality to causal identifiability by using paired image and prompt counterfactuals to separate visual effects, language-prior effects, and their harmful interactions, then editing only causally verified hallucination components. Second, study binding-aware compositional hallucination by asking whether attribute, relation, and counting errors arise from incorrect entity–concept bindings rather than isolated hallucination directions, and develop editing methods at the binding or operator level. Third, inspired by [ISO](https://arxiv.org/abs/2607.19331), replace destructive suppression with isospectral evidence realignment: preserve activation singular values and token geometry while rotating harmful prior or interaction subspaces away from hallucination-sensitive readout directions. Medical or other safety-critical domains can serve as external validation for image–text conflicts and insufficient visual evidence, but domain transfer alone should not be treated as the main novelty. Self-proposed extensions are also appreciated.

 
- **Supervisor** Abel
- **Paper ** Guard

  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - **Link :** 
  - **Brief description :** 
  - **How to reproduce :**
  - **How to extend :** 

## Topic 2 : Agentic Systems

- **Supervisor** Guilio
- **Paper ** XXXXX

  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - **Link :** 
  - **Brief description :** 
  - **How to reproduce :**
  - **How to extend :** 

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



## Topic : Structure Data Generation
- **Supervisor** Aditya
- **Paper ** XXXXX

  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - **Link :** 
  - **Brief description :** 
  - **How to reproduce :**
  - **How to extend :** 

-- **Supervisor** Jeroen
- **General description :** 
- **Paper ** XXXXX

  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - **Link :** 
  - **Brief description :** 
  - **How to reproduce :**
  - **How to extend :** 





