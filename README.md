# Knowledge Incorporation Frameworks Using LLMs  
[![Awesome](https://awesome.re/badge.svg)](https://github.com/Glasgow-AI4BioMed/Knowledge-Incorporation-Frameworks-Using-LLMs)  
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/Glasgow-AI4BioMed/Knowledge-Incorporation-Frameworks-Using-LLMs/blob/main/LICENSE)  

> **How can knowledge be incorporated into Large Language Models (LLMs)?**

🙌 This repository collects papers on integration techniques and frameworks for incorporating Knowledge Graphs (KG) into Large Language Modelling (LLM).

---

## 🌟 Why Incorporate KGs into LLMs?  

### 📚 Enhanced Knowledge Representation  
Integrating KGs with LLMs enables structured knowledge representation, improving reasoning and contextual understanding.

### 🧐 Improved Explainability, Reasoning, and Inference  
KGs provide a logical foundation for tasks requiring interpretable and inference-driven outputs.

### 🎯 Increased Accuracy and Reduced Hallucination  
LLMs benefit from the factual and structured knowledge in KGs, minimising hallucination and enhancing performance.

---

## 🚀 How to Incorporate KGs Effectively?  

### **Key Components**  

- **Backbone Models**: Support for protein, molecular, text, and visual modalities.  
- **Encoder Methods**: Bi-encoder and Cross-encoder.
- **Integration Stages**: Pretraining, post-training, fine-tuning, and inference pipelines.  
- **Integration Techniques**: Includes Adapters, LoRA, In-Context Learning (ICL), Retrieval-Augmented Generation (RAG), and LLM Agent.

---

## 📰 Latest Updates  

Stay tuned for news, newly added papers, and feature updates!

---

## 📖 Table of Contents  

- [Backbone Models](#backbone-models)  
- [Encoder Methods](#encoder-methods)  
- [Integration Stages](#integration-stages)  
- [Integration Techniques](#integration-techniques)  
- [Task Setups](#task-setups)  
- [Knowledge Graphs (KG)](#knowledge-graphs)  

---

## 📚 Backbone Models  

Backbone models form the foundation for integrating KG knowledge into LLMs. These models are tailored for either single-modal or multi-modal inputs:  

- **Protein Models**  
- **Molecular Models**  
- **Text Models**  
- **Visual Models**  

---

## 🔐 Encoder Methods  

### **Bi-Encoder**  
- Encodes two inputs separately (e.g., drugs or drug-protein pairs).  
- Efficient for entity-level embedding tasks such as pairwise similarity or interaction prediction.  

### **Cross-Encoder**  
- Jointly encodes multiple inputs in a unified context, capturing richer interactions.  
- Ideal for complex relationship modelling, such as drug-drug or drug-protein interactions.  

---

## 🛠 Integration Stages  

1. **Pretraining**: Incorporating KG knowledge during the initial training phase of LLMs.  
2. **Post-Training**: Updating LLMs with additional KG-based tasks after the initial training.  
3. **Fine-Tuning**: Adjusting specific parameters for task-specific objectives.  
4. **Inference**: Leveraging KG knowledge during real-time prediction or generation.

---

## 🔗 Integration Techniques  

### **Full Fine-Tuning (FT)**  
- Updates all model parameters for deep integration of KG knowledge.  
- Requires substantial task-specific data.  

### **Parameter-Efficient Fine-Tuning (PEFT)**  
Efficient fine-tuning strategies that modify only a small subset of parameters:  

- **Adapter**: Inserted between model layers to enable task-specific adjustments.  
- **LoRA (Low-Rank Adaptation)**: Uses low-rank decompositions for task-specific learning.  
- **Prefix-Tuning**: Optimises task-related prefixes, freezing most model parameters.  
- **ICL (In-Context Learning)**: Dynamically adapts to tasks without parameter updates.  
- **RAG (Retrieval-Augmented Generation)**: Combines LLM generation with external knowledge retrieval.  
- **LLM Agent**: Deploys LLMs as reasoning agents, integrating KG knowledge dynamically.

---

## 🔄 Task Setups  

### **Single-Instance Tasks**  
- Use a single entity (e.g., drug or protein) as input for reaction or property prediction tasks.  

### **Multi-Instance Tasks**  
- Process multiple entities (e.g., drug pairs, drug-protein pairs) simultaneously.  

---

## 🧠 Knowledge Graphs  

### **Homogeneous KGs**  
- Single-type nodes and edges (e.g., drug-drug interactions).  
- Simpler to model but less versatile for complex tasks.  

### **Heterogeneous KGs**  
- Multiple types of nodes and edges (e.g., drug-protein interactions).  
- Richer representations for biomedical tasks.  

### **Large-Scale KG Integration**  
Efficiently incorporating massive KGs into LLMs is crucial for scalability and performance.  

Key considerations:  
- **Scalability**: Graph sampling, indexing, and efficient representations.  
- **Multi-Modal Data**: Integration of textual, numerical, and structural information.  
- **Dynamic Updates**: Adapting to continuously evolving KGs.  
- **Sparse Connectivity**: Addressing sparsity through link prediction and knowledge completion.  
- **Knowledge Distillation**: Extracting essential knowledge for task-specific fine-tuning.  

---

## 🙌 Contributing  

We welcome your contributions!  

- **Add Missing Papers**: Submit suggestions via [Issues](https://github.com/Glasgow-AI4BioMed/Knowledge-Incorporation-Frameworks-Using-LLMs/issues) or [Pull Requests](https://github.com/Glasgow-AI4BioMed/Knowledge-Incorporation-Frameworks-Using-LLMs/pulls).  
- **Share Your Ideas**: Let us know how we can improve or expand this repository.  

---

## 📜 Licence  

This project is licensed under the [MIT Licence](https://github.com/Glasgow-AI4BioMed/Knowledge-Incorporation-Frameworks-Using-LLMs/blob/main/LICENSE).

---
