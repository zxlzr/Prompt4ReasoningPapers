# Reasoning with Language Model Prompting Papers

![](https://img.shields.io/github/last-commit/zjunlp/Prompt4ReasoningPapers?color=green) 
![](https://img.shields.io/badge/PaperNumber-49-brightgreen)

## 🔔 News

- **2022-12-19  We have released a new survey paper:"[Reasoning with Language Model Prompting: A Survey](https://arxiv.org/abs/2212.09597)" based on this repository! We are looking forward to any comments or discussions on this topic :)**

---

## 🔍 Contents

- [🌟 Introduction](#-introduction)
- [📜 Papers](#-papers)
  - [Methods](#methods)
    - [Strategy Enhanced Reasoning](#strategy-enhanced-reasoning)
      - [Prompt Engineering](#prompt-engineering)
        - [Single-Stage](#single-stage)
        - [Multi-Stage](#multi-stage)
      - [Process Optimization](#process-Optimization)
        - [Self-Optimization](#self-optimization)
        - [Ensemble-Optimization](#ensemble-optimization)
        - [Iterative-Optimization](#iterative-optimization)
      - [External Engine](#external-engine)
        - [Physical Simulator](#physical-simulator)
        - [Code Interpreter](#code-interpreter)
    - [Knowledge Enhanced Reasoning](#knowledge-enhanced-reasoning)
      - [Implicit Knowledge](#implicit-knowledge)
      - [Explicit Knowledge](#explicit-knowledge)
  - [Analysis](#analysis)
- [🧰 Resources](#-resources)
    - [Benchmarks and Tasks](#benchmarks-and-tasks)
    - [Tools](#tools)

---

## 🌟 Introduction

Reasoning, as an essential ability for complex problem-solving, can provide back-end support for various real-world applications, such as medical diagnosis, negotiation, etc. This paper provides a comprehensive survey of cutting-edge research on reasoning with language model prompting. We introduce research works with comparisons and summaries and provide systematic resources to help beginners. We also discuss the potential reasons for emerging such reasoning abilities and highlight future research directions. 

---

## 📜 Papers

### Methods

#### Strategy Enhanced Reasoning

##### Prompt Engineering

###### Single-Stage

1. **Prompting Contrastive Explanations for Commonsense Reasoning Tasks.**

   *Bhargavi Paranjape, Julian Michael, Marjan Ghazvininejad, Luke Zettlemoyer, Hannaneh Hajishirzi.* [[abs](https://arxiv.org/abs/2106.06823)], 2021.6

2. **Template Filling for Controllable Commonsense Reasoning.**

   *Dheeraj Rajagopal, Vivek Khetan, Bogdan Sacaleanu, Anatole Gershman, Andrew Fano, Eduard Hovy.* [[abs](https://arxiv.org/abs/2111.00539)], 2021.11

3. **Chain of Thought Prompting Elicits Reasoning in Large Language Models.**

   *Jason Wei, Xuezhi Wang, Dale Schuurmans, Maarten Bosma, Brian Ichter, Fei Xia, Ed H. Chi, Quoc V. Le, Denny Zhou.* [[abs](https://arxiv.org/abs/2201.11903)], 2022.1

4. **Large Language Models are Zero-Shot Reasoners.**

   *Takeshi Kojima, Shixiang Shane Gu, Machel Reid, Yutaka Matsuo, Yusuke Iwasawa.* [[abs](https://arxiv.org/abs/2205.11916)], 2022.5
   
5. **Complexity-based Prompting for Multi-step Reasoning.**

   *Yao Fu, Hao Peng, Ashish Sabharwal, Peter Clark, Tushar Khot.* [[abs](https://arxiv.org/abs/2210.00720)], 2022.10
   
6. **Language Models are Multilingual Chain-of-thought Reasoners.**

   *Freda Shi, Mirac Suzgun, Markus Freitag, Xuezhi Wang, Suraj Srivats, Soroush Vosoughi, Hyung Won Chung, Yi Tay, Sebastian Ruder, Denny Zhou, Dipanjan Das, Jason Wei.* [[abs](https://arxiv.org/abs/2210.03057)], 2022.10
   
7. **Automatic Chain of Thought Prompting in Large Language Models.**

    *Zhuosheng Zhang, Aston Zhang, Mu Li, Alex Smola.* [[abs](https://arxiv.org/abs/2210.03493)], 2022.10
    
8. **Large Language Models are few(1)-shot Table Reasoners.**

    *Wenhu Chen.* [[abs](https://arxiv.org/abs/2210.06710)], 2022.10

9. **Teaching Algorithmic Reasoning via In-context Learning.**

   *Hattie Zhou, Azade Nova, Hugo Larochelle, Aaron Courville, Behnam Neyshabur, Hanie Sedghi.* [[abs](https://arxiv.org/abs/2211.09066)], 2022.11

###### Multi-Stage

1. **Iteratively Prompt Pre-trained Language Models for Chain of Thought.**

   *Boshi Wang, Xiang Deng, Huan Sun.* [[abs](https://arxiv.org/abs/2203.08383)], 2022.3

2. **Selection-Inference: Exploiting Large Language Models for Interpretable Logical Reasoning.**

   *Antonia Creswell, Murray Shanahan, Irina Higgins.* [[abs](https://arxiv.org/abs/2205.09712)], 2022.5
   
3. **Least-to-Most Prompting Enables Complex Reasoning in Large Language Models.**

   *Denny Zhou, Nathanael Schärli, Le Hou, Jason Wei, Nathan Scales, Xuezhi Wang, Dale Schuurmans, Olivier Bousquet, Quoc Le, Ed Chi.* [[abs](https://arxiv.org/abs/2205.10625)], 2022.5
   
4. **Maieutic Prompting: Logically Consistent Reasoning with Recursive Explanations.**

   *Jaehun Jung, Lianhui Qin, Sean Welleck, Faeze Brahman, Chandra Bhagavatula, Ronan Le Bras, Yejin Choi.* [[abs](https://arxiv.org/abs/2205.11822)], 2022.5
   
5. **Faithful Reasoning Using Large Language Models.**

   *Antonia Creswell, Murray Shanahan.* [[abs](https://arxiv.org/abs/2208.14271)], 2022.8
   
6. **Decomposed Prompting: A Modular Approach for Solving Complex Tasks.**

   *Tushar Khot, Harsh Trivedi, Matthew Finlayson, Yao Fu, Kyle Richardson, Peter Clark, Ashish Sabharwal.* [[abs](https://arxiv.org/abs/2210.02406)], 2022.10
   
7. **Measuring and Narrowing the Compositionality Gap in Language Models.**

   *Ofir Press, Muru Zhang, Sewon Min, Ludwig Schmidt, Noah A. Smith, Mike Lewis.* [[abs](https://arxiv.org/abs/2210.03350)], 2022.10

##### Process Optimization

###### Self-Optimization

1. **Reframing Human-AI Collaboration for Generating Free-Text Explanations.**

   *Sarah Wiegreffe, Jack Hessel, Swabha Swayamdipta, Mark Riedl, Yejin Choi.* [[abs](https://arxiv.org/abs/2112.08674)], 2021.12

2. **The Unreliability of Explanations in Few-Shot In-Context Learning.**

   *Xi Ye, Greg Durrett.* [[abs](https://arxiv.org/abs/2205.03401)], 2022.5

###### Ensemble-Optimization

1. **Self-Consistency Improves Chain of Thought Reasoning in Language Models.**

   *Xuezhi Wang, Jason Wei, Dale Schuurmans, Quoc Le, Ed H. Chi, Sharan Narang, Aakanksha Chowdhery, Denny Zhou.* [[abs](https://arxiv.org/abs/2203.11171)], 2022.3

2. **On the Advance of Making Language Models Better Reasoners.**

   *Yifei Li, Zeqi Lin, Shizhuo Zhang, Qiang Fu, Bei Chen, Jian-Guang Lou, Weizhu Chen.* [[abs](https://arxiv.org/abs/2206.02336)], 2022.6
   
3. **Complexity-based Prompting for Multi-step Reasoning.**

   *Yao Fu, Hao Peng, Ashish Sabharwal, Peter Clark, Tushar Khot.* [[abs](https://arxiv.org/abs/2210.00720)], 2022.10

###### Iterative-Optimization

1. **STaR: Bootstrapping Reasoning With Reasoning.**

   *Eric Zelikman, Yuhuai Wu, Noah D. Goodman.* [[abs](https://arxiv.org/abs/2203.14465)], 2022.3
   
2. **Large Language Models Can Self-Improve.**

   *Jiaxin Huang, Shixiang Shane Gu, Le Hou, Yuexin Wu, Xuezhi Wang, Hongkun Yu, Jiawei Han.* [[abs](https://arxiv.org/abs/2210.11610)], 2022.10

##### External Engine

###### Physical Simulator

1. **Mind's Eye: Grounded Language Model Reasoning through Simulation.**

   *Ruibo Liu, Jason Wei, Shixiang Shane Gu, Te-Yen Wu, Soroush Vosoughi, Claire Cui, Denny Zhou, Andrew M. Dai*. [[abs](https://arxiv.org/abs/2210.05359)], 2022.10

###### Code Interpreter

1. **Language Models of Code are Few-Shot Commonsense Learners.**

   *Aman Madaan, Shuyan Zhou, Uri Alon, Yiming Yang, Graham Neubig.* [[abs](https://arxiv.org/abs/2210.07128)], 2022.10

2. **PAL: Program-aided Language Models.**

   *Luyu Gao, Aman Madaan, Shuyan Zhou, Uri Alon, Pengfei Liu, Yiming Yang, Jamie Callan, Graham Neubig.* [[abs](https://arxiv.org/abs/2211.10435)], 2022.11
   
3. **Program of Thoughts Prompting: Disentangling Computation from Reasoning for Numerical Reasoning Tasks.**

   *Wenhu Chen, Xueguang Ma, Xinyi Wang, William W. Cohen.* [[abs](https://arxiv.org/abs/2211.12588)], 2022.11

#### Knowledge Enhanced Reasoning

##### Implicit Knowledge

1. **Generated Knowledge Prompting for Commonsense Reasoning.**

    *Jiacheng Liu, Alisa Liu, Ximing Lu, Sean Welleck, Peter West, Ronan Le Bras, Yejin Choi, Hannaneh Hajishirzi.* [[abs](https://arxiv.org/abs/2110.08387)], 2021.10

2. **Rainier: Reinforced Knowledge Introspector for Commonsense Question Answering.**

    *Jiacheng Liu, Skyler Hallinan, Ximing Lu, Pengfei He, Sean Welleck, Hannaneh Hajishirzi, Yejin Choi.* [[abs](https://arxiv.org/abs/2210.03078)], 2022.10

3. **Explanations from Large Language Models Make Small Reasoners Better.**

    *Shiyang Li, Jianshu Chen, Yelong Shen, Zhiyu Chen, Xinlu Zhang, Zekun Li, Hong Wang, Jing Qian, Baolin Peng, Yi Mao, Wenhu Chen, Xifeng Yan.* [[abs](https://arxiv.org/abs/2210.06726)], 2022.10

4. **PINTO: Faithful Language Reasoning Using Prompt-Generated Rationales.**

    *Peifeng Wang, Aaron Chan, Filip Ilievski, Muhao Chen, Xiang Ren.* [[abs](https://arxiv.org/abs/2211.01562)], 2022.11

5. **TSGP: Two-Stage Generative Prompting for Unsupervised Commonsense Question Answering.**

    *Yueqing Sun, Yu Zhang, Le Qi, Qi Shi.* [[abs](https://arxiv.org/abs/2211.13515)], 2022.11

##### Explicit Knowledge

1. **LogicSolver: Towards Interpretable Math Word Problem Solving with Logical Prompt-enhanced Learning.**

   *Zhicheng Yang, Jinghui Qin, Jiaqi Chen, Liang Lin, Xiaodan Liang.* [[abs](https://arxiv.org/abs/2205.08232)], 2022.5

2. **Selective Annotation Makes Language Models Better Few-Shot Learners.**

   *Hongjin Su, Jungo Kasai, Chen Henry Wu, Weijia Shi, Tianlu Wang, Jiayi Xin, Rui Zhang, Mari Ostendorf, Luke Zettlemoyer, Noah A. Smith, Tao Yu.* [[abs](https://arxiv.org/abs/2209.01975)], 2022.9

3. **Dynamic Prompt Learning via Policy Gradient for Semi-structured Mathematical Reasoning.**

   *Pan Lu, Liang Qiu, Kai-Wei Chang, Ying Nian Wu, Song-Chun Zhu, Tanmay Rajpurohit, Peter Clark, Ashwin Kalyan.* [[abs](https://arxiv.org/abs/2209.14610)], 2022.9

#### Others

1. **Language Model Cascades.**

   *David Dohan, Winnie Xu, Aitor Lewkowycz, Jacob Austin, David Bieber, Raphael Gontijo Lopes, Yuhuai Wu, Henryk Michalewski, Rif A. Saurous, Jascha Sohl-dickstein, Kevin Murphy, Charles Sutton*. [[abs](https://arxiv.org/abs/2207.10342)], 2022.7
   
2. **Rationale-Augmented Ensembles in Language Models.**

   *Xuezhi Wang, Jason Wei, Dale Schuurmans, Quoc Le, Ed Chi, Denny Zhou.* [[abs](https://arxiv.org/abs/2207.00747)], 2022.7
   
3. **Psychologically-informed chain-of-thought prompts for metaphor understanding in large language models.**

   *Ben Prystawski, Paul Thibodeau, Noah Goodman.* [[abs](https://arxiv.org/abs/2209.08141)], 2022.9
   
4. **Learn to Explain: Multimodal Reasoning via Thought Chains for Science Question Answering.**

   *Pan Lu, Swaroop Mishra, Tony Xia, Liang Qiu, Kai-Wei Chang, Song-Chun Zhu, Oyvind Tafjord, Peter Clark, Ashwin Kalyan.* [[abs](https://arxiv.org/abs/2209.09513)], 2022.9
   
5. **The Impact of Symbolic Representations on In-context Learning for Few-shot Reasoning.**

   *Hanlin Zhang, Yi-Fan Zhang, Li Erran Li, Eric Xing.* [[abs](https://arxiv.org/abs/2212.08686)], 2022.12

6. **Large Language Models are reasoners with Self-Verification.**

   *Yixuan Weng, Minjun Zhu, Shizhu He, Kang Liu, Jun Zhao.* [[abs](https://arxiv.org/abs/2212.09561)]

### Analysis

1. **Can language models learn from explanations in context?**

   *Andrew K. Lampinen, Ishita Dasgupta, Stephanie C. Y. Chan, Kory Matthewson, Michael Henry Tessler, Antonia Creswell, James L. McClelland, Jane X. Wang, Felix Hill.* [[abs](https://arxiv.org/abs/2204.02329)], 2022.4
   
2. **Emergent Abilities of Large Language Models.**
   
   *Jason Wei, Yi Tay, Rishi Bommasani, Colin Raffel, Barret Zoph, Sebastian Borgeaud, Dani Yogatama, Maarten Bosma, Denny Zhou, Donald Metzler, Ed H. Chi, Tatsunori Hashimoto, Oriol Vinyals, Percy Liang, Jeff Dean, William Fedus.* [[abs](https://arxiv.org/abs/2206.07682)], 2022.6
   
3. **Language models show human-like content effects on reasoning.**
   
   *Ishita Dasgupta, Andrew K. Lampinen, Stephanie C. Y. Chan, Antonia Creswell, Dharshan Kumaran, James L. McClelland, Felix Hill.* [[abs](https://arxiv.org/abs/2207.07051)], 2022.7
   
4. **Can Large Language Models Truly Understand Prompts? A Case Study with Negated Prompts.**
   
   *Joel Jang, Seongheyon Ye, Minjoon Seo.* [[abs](https://arxiv.org/abs/2209.12711)], 2022.9
   
5. **Challenging BIG-Bench Tasks and Whether Chain-of-Thought Can Solve Them.**

   *Mirac Suzgun, Nathan Scales, Nathanael Schärli, Sebastian Gehrmann, Yi Tay, Hyung Won Chung, Aakanksha Chowdhery, Quoc V. Le, Ed H. Chi, Denny Zhou, Jason Wei.* [[abs](https://arxiv.org/abs/2210.09261)], 2022.10
   
6. **Language Models are Greedy Reasoners: A Systematic Formal Analysis of Chain-of-thought.**

   *Abulhair Saparov, He He.* [[abs](https://arxiv.org/abs/2210.01240)], 2022.10
   
7. **Knowledge Unlearning for Mitigating Privacy Risks in Language Models.**

   *Joel Jang, Dongkeun Yoon, Sohee Yang, Sungmin Cha, Moontae Lee, Lajanugen Logeswaran, Minjoon Seo.* [[abs](https://arxiv.org/abs/2210.01504)], 2022.10
   
8. **Emergent Analogical Reasoning in Large Language Models.**

   *Taylor Webb, Keith J. Holyoak, Hongjing Lu.* [[abs](https://arxiv.org/abs/2212.09196)], 2022.12

---

## 🧰 Resources

### Benchmarks and Tasks

|     Reasoning Skills      | Benchmarks                                                   |
| :-----------------------: | ------------------------------------------------------------ |
| **Arithmetic Reasoning**  | [GSM8K](https://arxiv.org/abs/2110.14168), [SVAMP](https://aclanthology.org/2021.naacl-main.168), [ASDiv](https://aclanthology.org/2020.acl-main.92/), [AQuA-RAT](https://aclanthology.org/P17-1015/), [MAWPS](https://aclanthology.org/N16-1136/), [AddSub](https://aclanthology.org/D14-1058/), [MultiArith](https://aclanthology.org/D15-1202/), [SingleEq](https://aclanthology.org/Q15-1042/), [SingleOp]( https://doi.org/10.1162/tacl_a_00118) |
| **Commonsense Reasoning** | [CommonsenseQA](https://aclanthology.org/N19-1421/), [StrategyQA](https://direct.mit.edu/tacl/article/doi/10.1162/tacl_a_00370/100680/Did-Aristotle-Use-a-Laptop-A-Question-Answering), [ARC](https://arxiv.org/abs/1803.05457), [SayCan](https://arxiv.org/abs/2204.01691), [BoolQA](https://aclanthology.org/N19-1300/), [HotpotQA](https://aclanthology.org/D18-1259/), [OpenBookQA](https://aclanthology.org/D18-1260/), [PIQA](https://yonatanbisk.com/piqa/) |
|  **Symbolic Reasoning**   | [Last Letter Concatenation](https://arxiv.org/abs/2201.11903), [Coin Flip](https://arxiv.org/abs/2201.11903), Reverse List |
|   **Logical Reasoning**   | [ProofWriter](https://arxiv.org/abs/2012.13048), [EntailmentBank](https://arxiv.org/abs/2104.08661), [RuleTaker](https://www.ijcai.org/proceedings/2020/537), [CLUTRR](https://aclanthology.org/D19-1458/) |
| **Multimodal Reasoning**  | [SCIENCEQA](https://scienceqa.github.io/)                    |
|        **Others**         | [BIG-bench](https://doi.org/10.48550/arXiv.2206.04615), [SCAN](http://proceedings.mlr.press/v80/lake18a.html) |

### Tools

- **[ThoughtSource](https://github.com/OpenBioLink/ThoughtSource)**: a central, open resource for data and tools related to chain-of-thought reasoning in LLMs. 
- **[LangChain](https://github.com/hwchase17/langchain)**: a library designed to help developers build applications using LLMs combined with other sources of computation or knowledge.
- **[LogiTorch](https://github.com/LogiTorch/logitorch)**: a PyTorch-based library for logical reasoning on natural language.

---

## 🚩Citation 
If you find this survey useful for your research, please consider citing

```
@misc{https://doi.org/10.48550/arxiv.2212.09597,
  doi = {10.48550/ARXIV.2212.09597},
  
  url = {https://arxiv.org/abs/2212.09597},
  
  author = {Qiao, Shuofei and Ou, Yixin and Zhang, Ningyu and Chen, Xiang and Yao, Yunzhi and Deng, Shumin and Tan, Chuanqi and Huang, Fei and Chen, Huajun},
  
  keywords = {Computation and Language (cs.CL), Artificial Intelligence (cs.AI), Computer Vision and Pattern Recognition (cs.CV), Information Retrieval (cs.IR), Machine Learning (cs.LG), FOS: Computer and information sciences, FOS: Computer and information sciences},
  
  title = {Reasoning with Language Model Prompting: A Survey},
  
  publisher = {arXiv},
  
  year = {2022},
  
  copyright = {arXiv.org perpetual, non-exclusive license}
}
```

