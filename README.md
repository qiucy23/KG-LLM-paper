# RAG-Paper-Reading

一个用于整理和学习检索增强生成（RAG）、大型语言模型（LLM）与知识图谱（KG）相关领域前沿论文的知识库。

## 介绍

这个仓库旨在记录和整理近年KG与LLM/RAG/Chain-of-Thought领域的前沿论文。

这并非一个纯粹的论文收集仓库，而是一个更偏向工业界应用方向的论文学习仓库。ToRead论文未经内容审核，可能在阅读后被删除。

## 目录 (Table of Contents)

* [ToRead](#toread)
  * Chain-of-Thought
      * [Graph of Thoughts: Solving Elaborate Problems with Large Language Models Authors - `AAAI-24`](https://ojs.aaai.org/index.php/AAAI/article/view/29720)
  * [CogMG: Collaborative Augmentation Between Large Language Model and Knowledge Graph - `ACL 2024 Demo`](https://aclanthology.org/2024.acl-demos.35/)
  * [Bi-Directional Multi-Granularity Generation Framework for Knowledge Graph-to-Text with Large Language Model - `ACL 2024 Short`](https://aclanthology.org/2024.acl-short.14/)
  * [HOLMES: Hyper-Relational Knowledge Graphs for Multi-hop Question Answering using LLMs - `ACL 2024`](https://aclanthology.org/2024.acl-long.717/)
  * [SAC-KG: Exploiting Large Language Models as Skilled Automatic Constructors for Domain Knowledge Graph - `ACL 2024`](https://aclanthology.org/2024.acl-long.238/)
  * [REANO: Optimising Retrieval-Augmented Reader Models through Knowledge Graph Generation - `ACL 2024`](https://aclanthology.org/2024.acl-long.115/)
  * [Direct Evaluation of Chain-of-Thought in Multi-hop Reasoning with Knowledge Graphs - `Findings of ACL 2024`](https://aclanthology.org/2024.findings-acl.168/)
  * [LLM as Prompter: Low-resource Inductive Reasoning on Arbitrary Knowledge Graphs - `Findings of ACL 2024`](https://aclanthology.org/2024.findings-acl.224/)
  * [Knowledge Graph-Enhanced Large Language Models via Path Selection - `Findings of ACL 2024`](https://aclanthology.org/2024.findings-acl.376/)
  * [Leveraging Graph Structures to Detect Hallucinations in Large Language Models - `textgraphs-17`](https://aclanthology.org/2024.textgraphs-1.7/)
  * [NLPeople at TextGraphs-17 Shared Task: Chain of Thought Questioning to Elicit Decompositional Reasoning - `textgraphs-17`](https://aclanthology.org/2024.textgraphs-1.13/)
* [HasRead](#hasread)
  * Chain-of-Thought
      * [Graph Chain-of-Thought: Augmenting Large Language Models by Reasoning on Graphs - `Findings of ACL 2024`](#graph-chain-of-thought-augmenting-large-language-models-by-reasoning-on-graphs-findings-of-acl-2024)

---


### 
已读论文

---

### [Graph Chain-of-Thought: Augmenting Large Language Models by Reasoning on Graphs (Findings of ACL 2024)](https://aclanthology.org/2024.findings-acl.11/)
* 提出了一种图结构的思维链范式，在每次迭代中包含三个子步骤：大模型推理、大模型-图谱交互以及图函数查询。图函数包含以下四种：
  * `RetrieveNode(Text): Identify related nodes in
  the graph with semantic search.`
  * `NodeFeature(NodeID, FeatureName): Extract
  the textual feature information from the graph
  for a specific node.`
  * `NeighborCheck(NodeID, NeighborType): Return the neighboring information in the graph
  for a specific node.`
  * ` NodeDegree(NodeID, NeighborType): Return
  the degree of a specific neighbor type for a
  specific node in the graph.`
  
* 提出了一种包含多个领域内的复杂图问答benchmark
* 在复杂图问答上超越 w/o-RAG LLM, naive RAG, GraphRAG