# Knowledge Incorporation Frameworks Using LLMs
[![Awesome](https://awesome.re/badge.svg)](https://github.com/Glasgow-AI4BioMed/Knowledge-Incorporation-Frameworks-Using-LLMs) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/Glasgow-AI4BioMed/Knowledge-Incorporation-Frameworks-Using-LLMs/blob/main/LICENSE)

>How can knowledge be incorporated into Large Language Models (LLMs)?

🙌 This repository collects papers on integration techniques for incorporating **Knowledge Graphs (KG)** into **Large Language Modelling (LLM)**.

😎 Welcome to recommend missing papers through **`Adding Issues`** or **`Pull Requests`**. 

## 🔔 News

## Content
  
- [📚 Backbone Models](#backbone-models)
  - **Single-Modal Models**
  - **Multi-Modal Models**
- [🔐 Encoder Methods](#encoder-methods)
  - **Bi-encoder**
  - **Cross-encoder**
- [🔗 Integration Techniques](#integration-techniques)
  - **Full Fine-Tuning (FT)**
  - **Parameter-Efficient Fine-Tuning (PEFT)**
    - **Adapter**
    - **LoRA (Low-Rank Adaptation)**
    - **Prefix-Tuning**
- [🔄 Task Setups](#task-setups)
  - **Single-Instance Tasks**
  - **Multi-Instance Tasks**
- [🧠 Knowledge Graphs (KG)](#kg)
  - **Homogeneous**
  - **Heterogeneous**
  - **Large Scale KG Integration**
---

## Backbone Models
- The backbone models in this framework focus on handling either single-modal or multi-modal inputs to integrate KG knowledge into LLMs. The models can vary from simpler structures like bi-encoders to more sophisticated cross-encoders, depending on the specific task requirements.

## Encoder Methods
- **Bi-encoder**: This method encodes two inputs separately (e.g., two drugs or drug-protein pairs), making it ideal for tasks where individual entity-level embeddings are needed. Bi-encoders are efficient for tasks like pairwise similarity or interaction prediction, as they handle separate representations and later calculate their interactions.
  
- **Cross-encoder**: In contrast to bi-encoders, cross-encoders jointly encode multiple inputs in a unified context. This approach captures richer interactions between the entities by concatenating them before feeding into the model, making it more suitable for capturing complex relationships in drug-drug or drug-protein interactions.

## Integration Techniques
- **Full Fine-Tuning (FT)**: This technique involves updating all parameters of the model. It is useful when large amounts of task-specific data are available and when deep integration of KG knowledge with LLMs is necessary.
  
- **Parameter-Efficient Fine-Tuning (PEFT)**: PEFT is a collection of techniques designed to fine-tune models efficiently by only modifying a small number of parameters. These methods include:
  - **Adapter**: Trainable modules inserted between layers of a pre-trained model, allowing task-specific adjustments without updating the main model.
  - **LoRA (Low-Rank Adaptation)**: LoRA introduces low-rank decompositions into pre-trained models to efficiently learn task-specific representations with minimal parameter updates.
  - **Prefix-Tuning**: This method optimizes specific task-related prefixes while freezing most of the main model's parameters, allowing efficient adaptation to new tasks.

## Task Setups
- **Single-Instance Tasks**: These tasks focus on using a single entity (e.g., a drug or a protein) as input for tasks such as classification or side-effect prediction.
  
- **Multi-Instance Tasks**: Multi-instance tasks require processing multiple entities (e.g., drug pairs, drug-protein pairs) simultaneously, making them suitable for tasks like interaction prediction.

## Knowledge Graphs (KG)
- **Homogeneous KGs**: Homogeneous KGs consist of single-type nodes and edges (e.g., drug-drug interactions). These are simpler to model but may lack the complexity needed for diverse biological tasks.
  
- **Heterogeneous KGs**: Heterogeneous KGs contain multiple types of nodes and edges (e.g., drug-protein interactions, protein-protein interactions). This structure allows for richer representations of biomedical data.
  
- **Large Scale KG Integration**: Efficiently integrating large-scale KGs into LLM frameworks is essential for handling complex datasets in the biomedical domain. Scalability is key when dealing with KGs containing millions of nodes and edges.

- ##  Papers
