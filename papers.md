
#  Topics, papers, and supervisors

## Topic 1: GenAI 

- **Supervisor** Gert Lek
- **General description :** AI-generated images are increasingly hard to distinguish by eye, and the political and safety consequences pose significant risks to trust in digital media, elections, and public discourse. This topic studies training-free detection of AI-generated images using vision foundation models to improve our ability to detect synthetic content.

- **Paper 1.1** Further improving training-free AI-generated image detection.

  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - **Link :** [Understanding and Improving Training-Free AI-Generated Image Detections with Vision Foundation Models](https://arxiv.org/abs/2411.19117)
  - **Brief description :** This work examines training-free detection of AI-generated images by analyzing how robust different their vision foundation model embeddings are to perturbations. It shows that fake images tend to be more sensitive to perturbations (e.g. Gaussian noise) than their real counterpart. It then designs an approach to use this sensitivity to detect fake images. The authors evaluate several pre-trained foundation models and perturbations. The authors then propose two improvements to make this insight competitive in detection with trained methods. 
  - **How to reproduce :** You will be given a set of 1000 image pairs (real vs. fake). Reproduce the key experiments as follows:
    1. Implement the baseline detector (RIGID) by extracting and computing the embedding similarity.
    2. Recreate the Gaussian noise and Gaussian blur perturbation experiment.
    3. Implement the MINDER approach from the paper by taking the minimum of similarities.
       
  - **How to extend :** More recent, powerful foundation models such as DINOv3 and I-JEPA have been released since the publication. An extension would be to evaluate these using the same framework on more powerful foundation models. You can also explore alternative aggregation schemes on the similarities instead of the mean, to use more structural information to improve performance. If we can find a new perturbation, this would be interesting, but the obvious choices for this have already been exhausted. Self-proposed extensions are also appreciated.

- **Paper 1.2** : Loss-landscape analysis of AI-generated vs. real images.

  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - **Link :** [Computational Safety for Generative AI:
A Signal Processing Perspective](https://arxiv.org/pdf/2502.12445) Section 5A
  - **Brief description :** Section V-A of this survey studies training-free detection of AI-generated images. It uses the above approach but visualises the loss-landscape in the vision foundation model embedding space. This visual is compared with its real counterpart. The insight here is that the synthetic images have a very specific and distinct loss-landscape vs. real images. 
  - **How to reproduce :** You will be given a set of 1000 image pairs (real vs. fake). Reproduce the key experiments:
    Select a subset of the real and generated images from several diffusion models and recreate their 2d loss-landscape visual. This is achieved by computing cosine similarities over different noise intensities. Create multiple graphs with varying settings of noise in each graph. 
  - **How to extend :** We conjecture that increased realism in more recent and powerful diffusion models has reduced the sensitivity difference. Thus the loss landscape of fake images should converge to that of the real images. You can investigate if this is indeed the case. This conjecture has important consequences: If true, images would become increasingly harder to detect. But if false, synthetic images look more realistic but carry the same artifacts that tell them apart from real images. Therefore, you will get data sets from more and less modern diffusion models and compare their loss-landscapes. A follow-up is to see when the conjecture is true, if more powerful foundation models restore the difference in the loss landscape. Self-proposed extensions are also appreciated.

## Topic 2 : XXXX

- **Supervisor:** Giulio




## Topic 3: GenAI

- **Supervisor:** Basile

- **General description:**
  This topic proposes considering different approaches to increase efficiency in the inference of generative models. The first subject addresses the problem of model selection under budget constraints, which has received a lot of traction lately. The second one concerns the challenge of accelerating Text-to-Image generation using alternative computer arithmetic. These subjects also contributes to AI trustworthiness by ensuring that generative models can deliver consistent results under limited computational budgets and by making the trade-offs between cost, speed, and output quality more explicit and measurable. The students will be able to use the most recent models to work on some very concrete issues of the current state of the art. They should be prepared to work on dense codebases and have a good understanding of the systems used in machine learning inference
  
- **Paper 3.1**
  - 👨‍🏫: ⭐⭐
  - 🖥️: ⭐⭐ 
  
  - Link: [PromptWise: Online Learning for Cost-Aware Prompt Assignment in Generative Models](https://arxiv.org/abs/2505.18901)
    
  - How to reproduce:
    
    Students should reproduce the proposed algorithm, focusing on the simpler task. The algorithm should run locally on publicly available models, using the inference time as cost input. They can rely on previous works' codebase for easier implementation.
    
  - How to extend:
    
    The students should consider one or several of the following extension path :   
      - Considering other modalities for the selected models, notably Text to Image generation. This requires using other models as well as considering new metrics for evaluation.
      - Using active learning to improve the prediction accuracy. Thanks to a measure of uncertainty, we can predict when to query ground truth results in order to refine the prediction of our selector.

- **Paper 3.2**
  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐⭐
  
  - Link: [MixDQ: Memory-Efficient Few-Step Text-to-Image Diffusion Models with Metric-Decoupled Mixed Precision Quantization](https://arxiv.org/abs/2405.17873)
    
  - How to reproduce:
    
    Reproduce the experimental results using the provided code. Specifically the students should ensure their results align with the value reported in the paper for SDXL.
  
  - How to extend:
    
    You can investigate one or several of the following points. Students are also welcomed to propose their ideas.  
      - Adapt the framework for undistilled models. This opens the way to state-of-the-art models but requires to design a quantization error correcting scheme more robust than the one currently proposed.  
      - Implement a caching policy to further increase sampling speed. Several caching methods already exist for diffusion models, it is yet to determine which one is the most suited to this case. 




## Topic 4: XXXX 

- **Supervisor:** Zhiwen


## Topic 5: XXX

- **Supervisor: Roberto
  


## Topic 6: GenAI (Sampling in graph synthesizers)
- **Supervisor:** Abele Malan

- **General description:**
  Investigate output controllability and process optimization in the sampling of iterative denoising (e.g., diffusion) deep learning models for synthetic graph generation.
  Ensuring that one can control a trained model on demand with specific rules is a key prerequisite to ensuring the trustworthiness of its output.
  Similarly, tweaking the sample generation process to optimize for desirable properties helps maximize confidence in the ability of models to generate reliable data.
  Data modeled by the graph generators encompasses structural (adjacency matrix) and, optionally, auxiliary (e.g., molecular atom and bond types) information.
  The reproducibility tasks focus on either exploring the sampling capabilities of a state-of-the-art model or techniques for conditioning sampling based on desirable properties across multiple models.
  Consequently, extensions tackle areas like generation speed/quality improvements or further increasing the complexity of targeted conditions.
  Since the work mainly concerns sampling, the longer and more resource-intensive part of training denoising models is not generally required.
  However, experiments involving new datasets or smaller auxiliary models could be an exception.
  For extensions, students should tackle at least one task.
  Working on alternative tasks is also possible, subject to approval from the teaching team.

- **Paper 6.1:** DeFoG: Discrete Flow Matching for Graph Generation
  - 👨‍🏫: ⭐
  - 🖥️: ⭐⭐
  - **Link:**
    [https://openreview.net/pdf?id=KPRIwWhqAZ](https://openreview.net/pdf?id=KPRIwWhqAZ)
  - **How to reproduce:**
    Use the provided codebase (and model checkpoints) to run the DeFoG model proposed in the paper (without the other baseline models).
    Specifically, recreate Table 1 (with 10% and 100% steps), Figure 2 (a), and all Figure 3 subfigures.
  - **How to extend:**
    - additional sample distortion functions, with the target of further boosting generation quality (MMD or validity), for (specific) test scenarios;
    - graph editing (e.g., given a graph, use the model trained on planar data to edit it into a planar version) or augmentation (e.g., given a graph structure, add the node types) instead of generation from scratch;
    - dynamic optimization of sampling parameters (distortion, target guidance, stochasticity) during generation.


- **Paper 6.2:** Diffuse, Sample, Project: Plug-And-Play Controllable Graph Generation
  - 👨‍🏫: ⭐⭐
  - 🖥️: ⭐⭐⭐
  - **Link:**
    [https://openreview.net/pdf?id=ia0Z8d1DbY](https://openreview.net/pdf?id=ia0Z8d1DbY)
  - **How to reproduce:**
    Use the codebase provided by the PRODIGY framework authors and checkpoints from the authors of the underlying tested models to replicate PRODIGY's main results.
    Specifically, recreate Table 5 (only the entries with PRODIGY and without the EDP-GNN model), Table 10 (which is Table 6, with additional hyperparameter information), and Table 11 (which is Table 7 with more hyperparameter information; only the QM9 dataset and again without the EDP-GNN model).
    Note that the model referred to as DruM by PRODIGY authors has since been renamed to GruM by its authors.
  - **How to extend:**
    - optimizing for more than one condition at once (the method supports such a use case, but the paper does not test it);
    - additional constraint types (e.g., control the count of other graphlets, like squares instead of triangles);
    - new partial step $\gamma_t$ formulations (possibly based on an auxiliary neural network).

*Bonus extension:* Harness classifier-free guidance in DeFoG's classifier-free guidance to dynamically steer graphs towards the closest counterpart satisfying one of the hard constraints covered in PRODIGY and analyze the obtained performance.
