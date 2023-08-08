# 👨‍💻 Awesome-Code-LLM [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![PR](https://img.shields.io/badge/PRs-Welcome-red)](https://img.shields.io/badge/PRs-Welcome-red) [![COMMIT](https://img.shields.io/github/last-commit/huybery/Awesome-Code-LLM?color=green)](https://img.shields.io/github/last-commit/huybery/Awesome-Code-LLM?color=green)

![](code-banner.png)

## 🧵 Table of Contents

- [👨‍💻 Awesome-Code-LLM   ](#-awesome-code-llm---)
  - [🧵 Table of Contents](#-table-of-contents)
  - [🚀 Leaderboard](#-leaderboard)
  - [📚 Paper](#-paper)
    - [▶️ Pre-Training](#️-pre-training)
    - [▶️ Instruction Tuning](#️-instruction-tuning)
    - [▶️ Alignment with Feedback](#️-alignment-with-feedback)
    - [▶️ Prompting](#️-prompting)
    - [▶️ Evaluation \& Benchmark](#️-evaluation--benchmark)
  - [🙌 Contributors](#-contributors)
  - [Cite as](#cite-as)
  - [Acknowledgement](#acknowledgement)
  - [Star History](#star-history)

## 🚀 Leaderboard

<p align="center"> <b>Leaderboard</b> (Sort by HumanEval Pass@1) </p>

| Rank | Model                    | Params | HumanEval | MBPP | HF                                                  | Paper                                     |
|------|--------------------------|--------|-----------|------|-----------------------------------------------------|-------------------------------------------|
| 1    | GPT-4 + Relexion         | ?      | 91.0      | 77.1 |                                                     | [paper](https://arxiv.org/abs/2303.11366) |
| 2    | GPT-4                    | ?      | 67.0      |      |                                                     | [paper](https://arxiv.org/abs/2303.08774) |
| 3    | Pangu-Coder2             | 15B    | 61.6      |      |                                                     | [paper](https://arxiv.org/abs/2307.14936) |
| 4    | WizardCoder-15B          | 15B    | 57.3      | 51.8 | [ckpt](https://hf.co/WizardLM/WizardCoder-15B-V1.0) | [paper](https://arxiv.org/abs/2306.08568) |
| 5    | GPT-3.5                  | ?      | 48.1      |      |                                                     | [paper](https://arxiv.org/abs/2303.08774) |
| 6    | Code-Davinci-002         | ?      | 47.0      |      |                                                     | [paper](https://arxiv.org/abs/2107.03374) |
| 7    | StarCoder-15B (Prompted) | 15B    | 40.8      | 49.5 | [ckpt](https://hf.co/bigcode/starcoder)             | [paper](https://arxiv.org/abs/2305.06161) |
| 8    | PaLM 2-S                 | ?      | 37.6      | 50.0 |                                                     | [paper](https://arxiv.org/abs/2204.02311) |
| 9    | PaLM-Coder-540B          | 540B   | 36.0      | 47.0 |                                                     | [paper](https://arxiv.org/abs/2204.02311) |
| 10   | InstructCodeT5+          | 16B    | 35.0      |      |                                                     | [paper](https://arxiv.org/abs/2305.07922) |
| 11   | StarCoder-15B            | 15B    | 33.6      | 52.7 | [ckpt](https://hf.co/bigcode/starcoder)             | [paper](https://arxiv.org/abs/2305.06161) |
| 12   | Code-Cushman-001         | ?      | 33.5      | 45.9 |                                                     | [paper](https://arxiv.org/abs/2107.03374) |
| 13   | CodeT5+                  | 16B    | 30.9      |      |                                                     | [paper](https://arxiv.org/abs/2305.07922) |
| 14   | LLaMA2-70B               | 70B    | 29.9      |      | [ckpt](https://hf.co/meta-llama/Llama-2-70b-hf)     | [paper](https://arxiv.org/abs/2307.09288) |
| 15   | CodeGen-16B-Mono         | 16B    | 29.3      | 35.3 |                                                     | [paper](https://arxiv.org/abs/2203.13474) |
| 16   | PaLM-540B                | 540B   | 26.2      | 36.8 |                                                     | [paper](https://arxiv.org/abs/2204.02311) |
| 17   | LLaMA-65B                | 65B    | 23.7      | 37.7 |                                                     | [paper](https://arxiv.org/abs/2302.13971) |
| 18   | CodeGeeX                 | 13B    | 22.9      | 24.4 |                                                     | [paper](https://arxiv.org/abs/2303.17568) |
| 19   | LLaMA-33B                | 33B    | 21.7      | 30.2 |                                                     | [paper](https://arxiv.org/abs/2302.13971) |
| 20   | CodeGen-16B-Multi        | 16B    | 18.3      | 20.9 |                                                     | [paper](https://arxiv.org/abs/2203.13474) |
| 21   | AlphaCode                | 1.1B   | 17.1      |      |                                                     | [paper](https://arxiv.org/abs/2203.07814) |


💡 Toolkit:
- [bigcode-evaluation-harness](https://github.com/bigcode-project/bigcode-evaluation-harness): A framework for the evaluation of autoregressive code generation language models.
- [multilingual-code-evals](https://huggingface.co/spaces/bigcode/multilingual-code-evals): Multilingual Code Models Evaluation.

## 📚 Paper

### ▶️ Pre-Training

1. **Evaluating Large Language Models Trained on Code** `Preprint`
  
    [[Paper](https://arxiv.org/abs/2107.03374)] *Mark Chen, Jerry Tworek, Heewoo Jun, Qiming Yuan, Henrique Ponde de Oliveira Pinto. et al.* 2021.07

2. **CodeGen: An Open Large Language Model for Code with Multi-Turn Program Synthesis** `ICLR23`
  
    [[Paper](https://arxiv.org/abs/2203.13474)] *Erik Nijkamp, Bo Pang, Hiroaki Hayashi, Lifu Tu, Huan Wang, Yingbo Zhou, Silvio Savarese, Caiming Xiong.* 2022.03

3. **CodeGen2: Lessons for Training LLMs on Programming and Natural Languages** `ICLR23`
  
    [[Paper](https://arxiv.org/abs/2305.02309)] *Erik Nijkamp, Hiroaki Hayashi, Caiming Xiong, Silvio Savarese, Yingbo Zhou.* 2023.05

4. **SantaCoder: don't reach for the stars!** `Preprint`
  
    [[Paper](https://arxiv.org/abs/2301.03988)] *Loubna Ben Allal, Raymond Li, Denis Kocetkov, Chenghao Mou, Christopher Akiki, Carlos Munoz Ferrandis, Niklas Muennighoff. et al.* 2023.01

5. **StarCoder: may the source be with you!** `Preprint`
  
    [[Paper](https://arxiv.org/abs/2305.06161)] *Raymond Li, Loubna Ben Allal, Yangtian Zi, Niklas Muennighoff, Denis Kocetkov, Chenghao Mou. et al.* 2023.05

6. **Textbooks Are All You Need** `Preprint`
  
    [[Paper](https://arxiv.org/abs/2306.11644)] *Suriya Gunasekar, Yi Zhang, Jyoti Aneja, Caio César Teodoro Mendes, Allie Del Giorno, Sivakanth Gopi. et al.* 2023.06


### ▶️ Instruction Tuning

1. **WizardCoder: Empowering Code Large Language Models with Evol-Instruct** `Preprint`
  
    [[Paper](https://arxiv.org/abs/2306.08568)] *Ziyang Luo, Can Xu, Pu Zhao, Qingfeng Sun, Xiubo Geng, Wenxiang Hu, Chongyang Tao, Jing Ma, Qingwei Lin, Daxin Jiang.* 2023.07

### ▶️ Alignment with Feedback

1. **PanGu-Coder2: Boosting Large Language Models for Code with Ranking Feedback** `Preprint`
  
    [[Paper](https://arxiv.org/abs/2307.14936)] *Bo Shen, Jiaxin Zhang, Taihong Chen, Daoguang Zan, Bing Geng, An Fu, Muhan Zeng, Ailun Yu, Jichuan Ji, Jingyang Zhao, Yuenan Guo, Qianxiang Wang.* 2023.07 

### ▶️ Prompting

1. **CodeT: Code Generation with Generated Tests** `ICLR23`
  
    [[Paper](https://arxiv.org/abs/2207.10397)] *Bei Chen, Fengji Zhang, Anh Nguyen, Daoguang Zan, Zeqi Lin, Jian-Guang Lou, Weizhu Chen.* 2022.07

2. **Coder Reviewer Reranking for Code Generation** `ICML23`
  
    [[Paper](https://arxiv.org/abs/2211.16490)] *Tianyi Zhang, Tao Yu, Tatsunori B Hashimoto, Mike Lewis, Wen-tau Yih, Daniel Fried, Sida I Wang.* 2022.11

3. **Teaching Large Language Models to Self-Debug** `Preprint`
  
    [[Paper](https://arxiv.org/abs/2304.05128)] *Xinyun Chen, Maxwell Lin, Nathanael Schärli, Denny Zhou.* 2023.06


4. **Demystifying GPT Self-Repair for Code Generation** `Preprint`
  
    [[Paper](https://arxiv.org/abs/2306.09896)] *Theo X. Olausson, Jeevana Priya Inala, Chenglong Wang, Jianfeng Gao, Armando Solar-Lezama.* 2023.06


### ▶️ Evaluation & Benchmark

1. **Measuring Coding Challenge Competence With APPS** `NeurIPS21`

    > Named APPS
  
    [[Paper](https://arxiv.org/abs/2108.07732)][[Repo](https://github.com/hendrycks/apps)] *Dan Hendrycks, Steven Basart, Saurav Kadavath, Mantas Mazeika, Akul Arora, Ethan Guo, Collin Burns, Samir Puranik, Horace He, Dawn Song, Jacob Steinhardt.* 2021.05 


2. **Program Synthesis with Large Language Models** `Preprint`

    > Named MBPP
  
    [[Paper](https://arxiv.org/abs/2108.07732)] *Jacob Austin, Augustus Odena, Maxwell Nye, Maarten Bosma, Henryk Michalewski, David Dohan, Ellen Jiang, Carrie Cai, Michael Terry, Quoc Le, Charles Sutton.* 2021.08 






## 🙌 Contributors

<a href="https://github.com/huybery"><img src="https://avatars.githubusercontent.com/u/13436140?v=4"  width="50" /></a>
<a href="https://github.com/Yangjiaxi"><img src="https://avatars.githubusercontent.com/u/6203054?v=4"  width="50" /></a>
<a href="https://github.com/GanjinZero"><img src="https://avatars.githubusercontent.com/u/19466330?v=4"  width="50" /></a>

This is an active repository and your contributions are always welcome! If you have any question about this opinionated list, do not hesitate to contact me `huybery@gmail.com`.

## Cite as

```
@software{awesome-code-llm,
  author = {Binyuan Hui},
  title = {An awesome and curated list of best code-LLM for research},
  howpublished = {\url{https://github.com/huybery/Awesome-Code-LLM}},
  year = 2023,
}
```

## Acknowledgement

This project is inspired by [Awesome-LLM](https://github.com/Hannibal046/Awesome-LLM).

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=huybery/Awesome-Code-LLM&type=Date)](https://star-history.com/#huybery/Awesome-Code-LLM&Date)


**[⬆ Back to ToC](#table-of-contents)**
