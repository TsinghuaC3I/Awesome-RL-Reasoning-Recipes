# Awesome RL Reasoning Recipes ("Triple R")

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated collection covering models, datasets, reward designs, optimization methods, hyperparameters, empirical findings, theoretical insights, and everything about reasoning with reinforcement learning.

## News
- **[2025-05-06]:** **🔥Releasing a survey on Efficient Diffusion Models — this survey provides resources and updates related to our research including **RL for Image Generation**. Check it out: [Github](https://github.com/TsinghuaC3I/Efficient-Diffusion-Models) and [Paper](https://arxiv.org/abs/2504.16084).**
- **[2025-04-23]:** **🔥Introducing TTRL — an open-source solution for online RL on data without ground-truth labels, especially test data. Check it out: [Github](https://github.com/PRIME-RL/TTRL) and [Paper](https://arxiv.org/abs/2504.16084).**

## Contents

> ⚠️⚠️⚠️ The following table of contents highlight only a selection of projects, which provide detailed configurations. For the most recent updates, please scroll to the bottom of the table:
> - [Jump to Latest LLM Projects 🚀🚀🚀](#llm_latest)
> - [Jump to Latest Multimodal Projects 🚀🚀🚀](#vlm_latest)
> - [Jump to Latest Agent Projects 🚀🚀🚀](#agent_latest)


- [Awesome RL Reasoning Recipes ("Triple R")](#awesome-rl-reasoning-recipes-triple-r)
  - [News](#news)
  - [Contents](#contents)
  - [Overview](#overview)
    - [Large Language Models](#large-language-models)
    - [Multimodal Models](#multimodal-models)
    - [Agentic Applications](#agentic-applications)
  - [Projects](#projects)
    - [Large Language Models](#large-language-models-1)
      - [2025.0102, PRIME-RL](#20250102-prime-rl)
      - [2025.0122, DeepSeek-R1](#20250122-deepseek-r1)
      - [2025.0122, Kimi k1.5](#20250122-kimi-k15)
      - [2025.0124, TinyZero](#20250124-tinyzero)
      - [2025.0125, SimpleRL](#20250125-simplerl)
      - [2025.0206, Demysitify-long-CoT](#20250206-demysitify-long-cot)
      - [2025.0210, DeepScaler](#20250210-deepscaler)
      - [2025.0210, Logic-RL](#20250210-logic-rl)
      - [2025.0210, OREAL](#20250210-oreal)
      - [2025.0217, LIMR](#20250217-limr)
      - [2025.0217, Open-Reasoner-Zero](#20250217-open-reasoner-zero)
      - [ 2025.0225, SWE-RL](#-20250225-swe-rl)
      - [2025.0303, VC-PPO ](#20250303-vc-ppo-)
      - [2025.0306, LCPO-L1 ](#20250306-lcpo-l1-)
      - [2025.0310, MetaRL ](#20250310-metarl-)
      - [2025.0318, TOPR ](#20250318-topr-)
      - [2025.0318, DAPO](#20250318-dapo)
      - [2025.0320, Open RS](#20250320-open-rs)
      - [2025.0321, Oat-Zero](#20250321-oat-zero)
      - [2025.0328, ARGO](#20250328-argo)
      - [2025.0407, VAPO](#20250407-vapo)
      - [2025.0410, Seed-Thinking-v1.5](#20250410-seed-thinking-v15)
      - [2025.0413, Skywork-OR1](#20250413-skywork-or1)
      - [2025.0416, d1 \& diffu-GRPO](#20250416-d1--diffu-grpo)
    - [Multimodal Models](#multimodal-models-1)
      - [2025.0128, open-r1-multimodal](#20250128-open-r1-multimodal)
      - [2025.0202, R1-V](#20250202-r1-v)
      - [2025.0215, VLM-R1](#20250215-vlm-r1)
      - [2025.0303, Visual-RFT](#20250303-visual-rft)
      - [2025.0306, r1-vlm](#20250306-r1-vlm)
      - [2025.0310, VisualThinker-R1-Zero](#20250310-visualthinker-r1-zero)
      - [2025.0310, MM-Eureka](#20250310-mm-eureka)
      - [2025.0310, Curr\_ReFT](#20250310-curr_reft)
      - [2025.0311, MMR1](#20250311-mmr1)
      - [2025.0315, MetaSpatial](#20250315-metaspatial)
      - [2025.0327, Reason-RFT](#20250327-reason-rft)
      - [2025.0409, Kimi-VL-Thinking](#20250409-kimi-vl-thinking)
      - [2025.0409, VideoChat-R1](#20250409-videochat-r1)
      - [2025.0410, VL-Rethinker](#20250410-vl-rethinker)
    - [Agentic Applications](#agentic-applications-1)
      - [2025.0307, R1-Searcher](#20250307-r1-searcher)
      - [2025.0309, AutoCoA](#20250309-autocoa)
      - [2024.0312, Search-R1](#20240312-search-r1)
      - [2025.0404, DeepResearcher](#20250404-deepresearcher)
      - [2025.0407, SWiRL](#20250407-swirl)
  - [Contributing](#contributing)
      - [202x.0x0x, Template](#202x0x0x-template)
  - [Citation](#citation)



## Overview

**This collection covers recent progress in reinforcement learning for large language model reasoning, starting from 2025 in the timeline.**


### Large Language Models

| Date      | Project            | Org                                | Intro                                                        | HF Model                                                     | HF Dataset                                                   | Takeaway Messages                                                 |
| --------- | ------------------ | ---------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 2025.0102 | PRIME-RL           | THU & UIUC <br /> Shanghai AI Lab      | [Paper](https://arxiv.org/abs/2502.01456)<br />[GitHub](https://github.com/PRIME-RL/PRIME)<br /> [More](#primerl) | [Eurus-2-7B-PRIME](https://huggingface.co/PRIME-RL/Eurus-2-7B-PRIME) <br />[Eurus-2-7B-PRIME-Zero](https://huggingface.co/PRIME-RL/Eurus-2-7B-PRIME-Zero) | [Eurus-2-RL-Data](https://huggingface.co/datasets/PRIME-RL/Eurus-2-RL-Data) | <details><summary>Click</summary>PRIME offers scalable Reinforcement Learning by using dense, token-level implicit rewards derived only from final outcomes. This bypasses costly step-by-step annotations, providing fine-grained feedback to improve sample efficiency and reasoning.</details> |
| 2025.0122 | DeepSeek-R1        | DeepSeek                           | [Paper](https://arxiv.org/abs/2501.12948)<br />[GitHub](https://github.com/deepseek-ai/DeepSeek-R1/tree/main)<br />[More](#deepseek-r1) | [DeepSeek-R1](https://huggingface.co/deepseek-ai/DeepSeek-R1) <br />[DeepSeek-R1-Zero](https://huggingface.co/deepseek-ai/DeepSeek-R1-Zero) | ——                                                           | <details><summary>Click</summary>DeepSeek-R1's core contribution is demonstrating large-scale RL from scratch (600B+) without SFT, achieving emergent "aha moments" (self-reflective reasoning) and matching OpenAI o1's performance at 1/30 cost</details> |
| 2025.0122 | Kimi k1.5          | Kimi                               | [Paper](https://arxiv.org/abs/2501.12599)<br />[GitHub](https://github.com/MoonshotAI/Kimi-k1.5)<br />[More](#kimi-k1.5) | ——                                                           | ——                                                           | <details><summary>Click</summary>Kimi 1.5 introduces a simplified RL framework that leverages long-context scaling (128k tokens) and improved policy optimization (e.g., online mirror descent) to enhance reasoning and multimodal performance.</details> |
| 2025.0124 | TinyZero           | Berkeley                           | [Twitter](https://x.com/jiayi_pirate/status/1882839370505621655)<br />[GitHub](https://github.com/Jiayi-Pan/TinyZero)<br />[More](#tinyzero) | ——                                                           | [Countdown-Tasks-3to4](https://huggingface.co/datasets/Jiayi-Pan/Countdown-Tasks-3to4) | <details><summary>Click</summary>TinyZero's core contribution is demonstrating that smaller language models (e.g., 1.5B-3B parameters) can develop complex reasoning, search, and self-verification abilities through Reinforcement Learning, replicating capabilities of larger models like DeepSeek R1-Zero at extremely low cost (<$30).</details> |
| 2025.0124 | Open-R1            | Huggingface                        | [GitHub](https://github.com/huggingface/open-r1)             | [OpenR1-Qwen-7B](https://huggingface.co/open-r1/OpenR1-Qwen-7B)<br />[OlympicCoder-7B](https://huggingface.co/open-r1/OlympicCoder-7B)<br />[OlympicCoder-32B](https://huggingface.co/open-r1/OlympicCoder-32B) | [OpenR1-Math-220k](https://huggingface.co/datasets/open-r1/OpenR1-Math-220k)<br />[codeforces](https://huggingface.co/datasets/open-r1/codeforces) | <details><summary>Click</summary>Open-R1's core contribution is providing the first fully open-source replication and release of the DeepSeek R1-Zero Reinforcement Learning training pipeline. Its main insight or goal is to democratize access to these advanced RL techniques for enhancing LLM reasoning and planning.</details> |
| 2025.0125 | simpleRL-reason    | HKUST                              | [Paper](https://hkust-nlp.notion.site/simplerl-reason)<br />[GitHub](https://github.com/hkust-nlp/simpleRL-reason)<br />[More](#simplerl) | [Qwen-2.5-Math-7B-SimpleRL-Zero](https://huggingface.co/hkust-nlp/Qwen-2.5-Math-7B-SimpleRL-Zero)<br />[Qwen-2.5-Math-7B-SimpleRL](https://huggingface.co/hkust-nlp/Qwen-2.5-Math-7B-SimpleRL) | [MATH](https://huggingface.co/datasets/EleutherAI/hendrycks_math) | <details><summary>Click</summary>Researchers replicated the DeepSeek-R1-Zero and DeepSeek-R1 training using a 7B model with only 8K MATH examples, achieving strong results on complex mathematical reasoning.</details> |
| 2025.0205 | Demystify-long-cot | CMU                                | [Paper](https://arxiv.org/abs/2502.03373)<br />[GitHub](https://github.com/eddycmu/demystify-long-cot)<br />[More](#demystify) | ——                                                           | ——                                                           | <details><summary>Click</summary>The paper elucidates the role of RL in stabilizing and enhancing long CoT reasoning in LLMs, highlighting the necessity of reward shaping and verifiable reward signals for complex reasoning tasks.</details> |
| 2025.0210 | DeepScaler         | Agentica-Org                       | [Blog](https://pretty-radio-b75.notion.site/DeepScaleR-Surpassing-O1-Preview-with-a-1-5B-Model-by-Scaling-RL-19681902c1468005bed8ca303013a4e2)<br />[GitHub](https://github.com/agentica-project/deepscaler)<br />[More](#deepscaler) | [DeepScaleR-1.5B-Preview](https://huggingface.co/agentica-org/DeepScaleR-1.5B-Preview) | [DeepScaleR-Preview-Dataset](https://huggingface.co/datasets/agentica-org/DeepScaleR-Preview-Dataset) | <details><summary>Click</summary>DeepScaleR's core contribution is demonstrating that a small 1.5B parameter model, fine-tuned using scaled Reinforcement Learning (RL) and an iterative context lengthening scheme, can surpass the reasoning performance of larger, state-of-the-art models like OpenAI's O1-Preview on complex benchmarks (e.g., AIME math problems).</details> |
| 2025.0210 | Logic-RL           | MSRA & Ubiquant                    | [Paper](https://arxiv.org/pdf/2502.14768)<br />[GitHub](https://github.com/Unakar/Logic-RL)<br />[More](#logicrl) | ——                                                           | [knights-and-knaves](https://huggingface.co/datasets/K-and-K/knights-and-knaves)   [knights-and-knaves-ZH](https://huggingface.co/datasets/Trae1ounG/knights-and-knaves-ZH)  | <details><summary>Click</summary>The paper introduces Logic-RL, a rule-based reinforcement learning framework that enables large language models to develop o3-mini-level reasoning skills through training on logic puzzles. The reasoning capabilities can also be transferred to other domains like math.</details> |
| 2025.0210 | OREAL              | Shanghai AI Lab <br /> SJTU & CUHK | [Paper](https://arxiv.org/abs/2502.06781)<br /> [GitHub](https://github.com/InternLM/OREAL)<br /> [More](#oreal) | [OREAL-32B](https://huggingface.co/internlm/OREAL-32B)  [OREAL-7B](https://huggingface.co/internlm/OREAL-7B)<br />[OREAL-DeepSeek-R1-Distill-Qwen-7B](https://huggingface.co/internlm/OREAL-DeepSeek-R1-Distill-Qwen-7B)<br />[OREAL-32B-SFT](https://huggingface.co/internlm/OREAL-32B-SFT)<br />[OREAL-7B-SFT](https://huggingface.co/internlm/OREAL-7B-SFT) | [OREAL-RL-Prompts](https://huggingface.co/datasets/internlm/OREAL-RL-Prompts) | <details><summary>Click</summary>The paper introduces OREAL, a reinforcement learning framework for mathematical reasoning with binary feedback. It proves that behavior cloning on positive samples is sufficient for optimal learning and proposes reward reshaping for negative samples. A token-level reward model addresses sparse rewards in long reasoning chains. OREAL achieves state-of-the-art results on math benchmarks.</details> |
| 2025.0217 | LIMR               | SJTU                               | [Paper](https://arxiv.org/pdf/2502.11886)<br />[GitHub](https://github.com/GAIR-NLP/LIMR)<br /> [More](#limr) | [LIMR](https://huggingface.co/GAIR/LIMR)                     | [LIMR](https://huggingface.co/datasets/GAIR/LIMR)            | <details><summary>Click</summary>The paper challenges the assumption that scaling up RL training data inherently improves performance in language models, instead finding that a strategically selected subset of 1,389 samples can outperform a full 8,523-sample dataset.</details> |
| 2025.0218 | Open-Reasoner-Zero | StepFun & THU                      | [Paper](https://github.com/Open-Reasoner-Zero/Open-Reasoner-Zero/blob/main/ORZ_paper.pdf) <br />[GitHub](https://github.com/Open-Reasoner-Zero/Open-Reasoner-Zero/)<br />   [More](#openreaon-zero) | [Open-Reasoner-Zero-7B](https://huggingface.co/Open-Reasoner-Zero/Open-Reasoner-Zero-7B)<br />[Open-Reasoner-Zero-32B](https://huggingface.co/Open-Reasoner-Zero/Open-Reasoner-Zero-32B) | [ORZ-Math-57k](https://github.com/Open-Reasoner-Zero/Open-Reasoner-Zero/tree/main/data) | <details><summary>Click</summary>The Open-Reasoner-Zero model has achieved notable performance, with Open-Reasoner-Zero-32B outperforming DeepSeek-R1-Zero-Qwen-32B on the GPQA Diamond benchmark while requiring significantly fewer training steps.</details> |
| 2025.0225 | SWE-RL             | FAIR at Meta                       | [Paper](https://arxiv.org/abs/2502.18449)<br />[GitHub](https://github.com/facebookresearch/swe-rl)<br />[More](#swerl) | ——                                                           | ——                                                           | <details><summary>Click</summary>SWE-RL enhances LLMs' code reasoning through RL using open-source software evolution data, achieving state-of-the-art results in software engineering tasks and demonstrating generalized reasoning capabilities beyond coding.</details> |
| 2025.0227 | Med-RLVR              | Microsoft Research | [Paper](https://arxiv.org/pdf/2502.19655)<br />[More](#medrlvr) | ——                                                           | ——                                                           | <details><summary>Click</summary>The Med-RLVR framework demonstrates emergent medical reasoning via RL, achieving performance parity with SFT on in-distribution tasks and improving out-of-distribution generalization, all without explicit reasoning supervision, showcasing RL's potential in medicine.</details> |
| 2025.0303 | VC-PPO             | Bytedance                          | [Paper](https://arxiv.org/abs/2503.01491)<br />[More](#vcppo) | ——                                                           | ——                                                           | <details><summary>Click</summary>VC-PPO (Value-Calibrated PPO) diagnoses PPO's collapse in long CoT tasks as stemming from value function inaccuracies (initialization bias and reward signal decay in long sequences). Its core contribution is modifying PPO with value pretraining and decoupled GAE for actor and critic.</details> |
| 2025.0306 | LCPO-L1            | CMU                                | [Paper](https://arxiv.org/abs/2503.04697)<br />[GitHub](https://github.com/cmu-l3/l1)<br />[More](#lcpol1) | [L1-Qwen-1.5B-Max](https://huggingface.co/l3lab/L1-Qwen-1.5B-Max)<br /> [L1-Qwen-1.5B-Exact](https://huggingface.co/l3lab/L1-Qwen-1.5B-Exact) | ——                                                           | <details><summary>Click</summary>L1 introduces Length Controlled Policy Optimization (LCPO), a RL method enabling precise control over a reasoning model's thinking time (output length) via prompt instructions. It shows that RL effectively controls reasoning duration and unexpectedly enhances even short-chain reasoning capabilities.</details> |
| 2025.0310 | MRT                | CMU                                | [Paper](https://arxiv.org/pdf/2503.07572)<br />[Project](https://cohenqu.github.io/mrt.github.io/)<br />[GitHub](https://github.com/CMU-AIRe/MRT) | ——                                                           | ——                                                           | <details><summary>Click</summary>MRT (Mixed-Reality Trajectory Preferences) introduces a novel method for fine-tuning cooperative LLM agents. It effectively blends human preferences on real interaction trajectories with AI preferences on synthetic variations, improving data efficiency. This mixed-reality approach surpasses purely AI-driven feedback (RLAIF), especially for complex, multi-turn collaborative tasks.</details> |
| 2025.0318 | TOPR               | Mila & Reliant AI                  | [Paper](https://arxiv.org/abs/2503.14286v2)<br />[More](#topr) | ——                                                           | ——                                                           | <details><summary>Click</summary>TOPR (Tapered Off-Policy REINFORCE) introduces a novel RL algorithm for fine-tuning LLMs. Its core contribution is using asymmetric, tapered importance sampling to modify REINFORCE, enabling stable and efficient off-policy learning. This allows reusing past data effectively without the instability often seen in other methods and without needing explicit KL regularization.</details> |
| 2025.0318 | DAPO               | Bytedance <br /> THU               | [Paper](https://arxiv.org/pdf/2503.14476)<br />[GitHub](https://github.com/BytedTsinghua-SIA/DAPO)<br />[More](#dapo) | ——                                                           | [DAPO-Math-17k](https://huggingface.co/datasets/BytedTsinghua-SIA/DAPO-Math-17k) | <details><summary>Click</summary>DAPO algorithm introduces four key techniques (Clip-Higher, Dynamic Sampling, Token-Level Loss, Overlong Shaping) for stable and efficient long-chain-of-thought RL training, surpassing previous SoTA results efficiently.</details> |
| 2025.0320 | Open RS          | VNU University of Science & Knovel Engineering Lab                            | [Paper](https://arxiv.org/pdf/2503.16219)<br />[GitHub](https://github.com/knoveleng/open-rs)<br />[More](#open-rs) | [Open-RS1](https://huggingface.co/knoveleng/Open-RS1)<br />[Open-RS2](knoveleng/Open-RS2)<br />[Open-RS3](https://huggingface.co/knoveleng/Open-RS3) | [open-s1](https://huggingface.co/datasets/knoveleng/open-s1)<br />[open-deepscaler](https://huggingface.co/datasets/knoveleng/open-deepscaler)<br />[open-rs](https://huggingface.co/datasets/knoveleng/open-rs) | <details><summary>Click</summary>The study investigates the potential of RL to improve reasoning in small LLMs. The results demonstrate rapid reasoning gains, with accuracy improvements on mathematical reasoning benchmarks, and highlight the efficacy of RL-based fine-tuning for small LLMs as a cost-effective alternative to large-scale approaches, using high-quality training data.</details> |
| 2025.0321 | Oat-Zero           | Sail-Sg                            | [Paper](https://arxiv.org/abs/2503.20783)<br />[GitHub](https://github.com/sail-sg/understand-r1-zero)<br />[More](#oat-zero) | [Qwen2.5-Math-7B-Oat-Zero](https://huggingface.co/sail/Qwen2.5-Math-7B-Oat-Zero)<br />[Qwen2.5-Math-1.5B-Oat-Zero](https://huggingface.co/sail/Qwen2.5-Math-1.5B-Oat-Zero)<br />[Llama-3.2-3B-Oat-Zero](https://huggingface.co/sail/Llama-3.2-3B-Oat-Zero) | [MATH](https://huggingface.co/datasets/EleutherAI/hendrycks_math) | <details><summary>Click</summary>This work critically analyzes R1-Zero-like RL training. It reveals base model properties and GRPO algorithm biases (e.g., length bias) significantly impact outcomes. It contributes the efficient, unbiased Dr. GRPO algorithm and an open-source recipe/codebase for better understanding and reproduction.</details> |
| 2025.0321 | FastCuRL           | Tencent Hunyuan                    | [Paper](https://arxiv.org/abs/2503.17287)<br />[GitHub](https://github.com/nick7nlp/FastCuRL) | [FastCuRL-1.5B-Preview](https://huggingface.co/Nickyang/FastCuRL-1.5B-Preview) | [FastCuRL](https://huggingface.co/datasets/Nickyang/FastCuRL) | <details><summary>Click</summary>FastCuRL introduces a simple, efficient Curriculum RL method for LLMs. Its core contribution uses target perplexity to dynamically scale the standard RL loss (like PPO), creating an effective curriculum without complex reward models or auxiliary components, enabling faster, more stable training.</details> |
| 2025.0328 | ARGO           | Meta                    | [Paper](https://arxiv.org/abs/2503.19612)<br /> | —— | —— | <details><summary>Click</summary>This paper derived the Any-Generation Reward Optimization (AGRO) frim the consistency condition across any possible generation of the model. AGRO achieves a better convergence than KL-regularized policy gradient method.</details> |
| 2025.0401 | Z1           | THU                    | [Paper](https://arxiv.org/abs/2504.00810)<br />[GitHub](https://github.com/efficientscaling/Z1) | [Z1-7B](https://huggingface.co/efficientscaling/Z1-7B) | [Z1-Code-Reasoning-107K](https://huggingface.co/datasets/efficientscaling/Z1-Code-Reasoning-107K) | <details><summary>Click</summary>This paper proposes training LLMs on code-related reasoning trajectories using a curated dataset and a "Shifted Thinking Window" technique. This allows models to reduce excessive thinking tokens, achieving efficient test-time scaling and generalizing reasoning abilities.</details> |
| 2025.0401 | VAPO           | ByteDance Seed                    | [Paper](https://arxiv.org/pdf/2504.05118)<br /> | —— | —— | <details><summary>Click</summary>VAPO offers an integrated solution that effectively alleviates value model bias, the presence of heterogeneous sequence lengths, and the sparsity of reward signal.</details> |
|2025.0407 |  ConciseRL  |   Wand AI   | [Paper](https://arxiv.org/pdf/2504.05185) | —— | —— | <details><summary>Click</summary>This work challenges the idea that longer reasoning chains in LLMs inherently mean better accuracy. It uses mathematical analysis of RL principles, particularly PPO, to show that lengthier responses often arise from the optimization process itself, not necessarily improved reasoning.</details> |
| 2025.0409 | AdaRFT           | USC LIME Lab                    | [Paper](https://arxiv.org/abs/2504.05520)<br />[GitHub](https://github.com/uscnlp-lime/verl) | —— | [DeepScaleR_Difficulty](https://huggingface.co/datasets/lime-nlp/DeepScaleR_Difficulty) | <details><summary>Click</summary>AdaRFT proposes Adaptive Curriculum Reinforcement Finetuning to improve LLM reasoning training efficiency. It dynamically adjusts task difficulty based on recent reward signals, accelerating learning by keeping challenges optimally balanced. Experiments on competition math benchmarks show up to 2x fewer steps and improved accuracy, using standard PPO with minimal changes.</details> |
| 2025.0410 | Seed-Thinking-v1.5 | ByteDance Seed                         | [Paper, GitHub](https://github.com/ByteDance-Seed/Seed-Thinking-v1.5) | —— | —— | <details><summary>Click</summary>Seed-Thinking-v1.5 is a high-performing reasoning model that combines curated chain-of-thought data, stable reinforcement learning, and advanced infrastructure to achieve strong results across math, coding, and logic tasks.</details> |
| 2025.0410 | d1 & diffu-GRPO | UCLA & Meta| [Paper](https://arxiv.org/pdf/2504.12216)<br />[GitHub](https://github.com/dllm-reasoning/d1)<br />[Project](https://dllm-reasoning.github.io)  | —— | —— | <details><summary>Click</summary> This paper propose d1 to adapt pre-trained masked dLLMs into reasoning via a combination of SFT and RL. The RL method used is named diffu-GRPO. </details> |
| 2025.0413 | Skywork-OR1 | Skywork AI| [Blog](https://capricious-hydrogen-41c.notion.site/Skywork-Open-Reasoner-Series-1d0bc9ae823a80459b46c149e4f51680)<br />[GitHub](https://github.com/SkyworkAI/Skywork-OR1)  | [Skywork-OR1-32B-Preview](https://huggingface.co/Skywork/Skywork-OR1-32B-Preview)<br />[Skywork-OR1-7B-Preview](https://huggingface.co/Skywork/Skywork-OR1-7B-Preview)<br />[Skywork-OR1-Math-7B](https://huggingface.co/Skywork/Skywork-OR1-Math-7B) | [Skywork-OR1-RL-Data](https://huggingface.co/datasets/Skywork/Skywork-OR1-RL-Data) | <details><summary>Click</summary> Skywork-OR1 is a series of robust open-source models trained on carefully curated math and code data. The training process incorporates several modifications to the original GRPO, including offline and online data filtering, multi-stage training, and adaptive entropy control. </details> |
| 2025.0423 | TTRL | THU&Shanghai AI Lab | [Paper](https://arxiv.org/abs/2504.16084)<br />[GitHub](https://github.com/PRIME-RL/TTRL) | —— | —— | <details><summary>Click</summary>This paper investigates Reinforcement Learning (RL) on data without explicit labels for reasoning tasks in Large Language Models (LLMs).</details> |
| <div id="llm_latest">2025.0x0x</div> |             |                      | [Paper]()<br />[GitHub]() | [hf models]() | [hf datasets]() | <details><summary>Click</summary>insights and contributions about RL for reasoning within 30 words.</details> |

### Multimodal Models
| Date      | Project               | Org                | Intro                                                        | HF Model                                                     | HF Dataset                                                   | Takeaway Messages                                                 |
| --------- | --------------------- | ------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 2025.0128 | Open-R1-MultiModal    | LLMs Lab           | [GitHub](https://github.com/EvolvingLMMs-Lab/open-r1-multimodal)<br />[More](#open-r1-mm) | [Qwen2-VL-2B-GRPO-8k](https://huggingface.co/lmms-lab/Qwen2-VL-2B-GRPO-8k)<br />[Qwen2-VL-7B-GRPO-8k](https://huggingface.co/lmms-lab/Qwen2-VL-7B-GRPO-8k) | [multimodal-open-r1-8k-verified](https://huggingface.co/datasets/lmms-lab/multimodal-open-r1-8k-verified) | <details><summary>Click</summary>Open-R1-MultiModal provides an open-source replication of R1-Zero-like RL for Multimodal LLMs, aiming to enhance complex visual reasoning. It demonstrates the effectiveness of these RL techniques for boosting multimodal performance and promotes reproducibility in the field.</details> |
| 2025.0202 | R1-V                  | Deep Agent         | [Blog](https://deepagent.notion.site/rlvr-in-vlms)<br />[GitHub](https://github.com/Deep-Agent/R1-V)<br />[More](#r1v) | ——                                                           | [Clevr_CoGenT_TrainA_R1](https://huggingface.co/datasets/MMInstruction/Clevr_CoGenT_TrainA_R1) | <details><summary>Click</summary>R1-V applies RL, specifically RLV-Instruct, to fine-tune VLMs. It enhances complex visual reasoning and instruction-following capabilities in VLMs beyond standard supervised fine-tuning.</details> |
| 2025.0215 | VLM-R1                | OmAI Lab           | [Blog](https://om-ai-lab.github.io/index.html) <br />[GitHub](https://github.com/om-ai-lab/VLM-R1)<br />[More](#vlmr1) | [OVD](https://huggingface.co/omlab/VLM-R1-Qwen2.5VL-3B-OVD-0321)<br />[Math](https://huggingface.co/omlab/VLM-R1-Qwen2.5VL-3B-Math-0305) <br />[REC](https://huggingface.co/omlab/Qwen2.5VL-3B-VLM-R1-REC-500steps) | ——                                                           | <details><summary>Click</summary>VLM-R1 applies R1-style RL to VLMs, improving stability and generalization on visual reasoning tasks. It shows that RL enhances VLM generalization beyond standard fine-tuning, achieving SOTA results, particularly on complex or out-of-domain benchmarks.</details> |
| 2025.0303 | Visual-RFT                | SJTU & Shanghai AI Lab & CUHK        | [Paper](https://arxiv.org/pdf/2503.01785)<br />[GitHub](https://github.com/Liuziyu77/Visual-RFT)<br />[More](#research) | [Reasoning Grounding](https://huggingface.co/Zery/Qwen2-VL-7B_visual_rft_lisa_IoU_reward) | [COCO_base65](https://huggingface.co/datasets/laolao77/ViRFT_COCO_base65)<br />[COCO](https://huggingface.co/datasets/laolao77/ViRFT_COCO)<br />[COCO_8_classes_4_shot](https://huggingface.co/datasets/laolao77/ViRFT_COCO_8_cate_4_shot)<br />[LVIS_few_shot](https://huggingface.co/datasets/laolao77/ViRFT_LVIS_few_shot)<br />[Flower_4_shot](https://huggingface.co/datasets/laolao77/ViRFT_CLS_flower_4_shot)<br />[FGVC_Aircraft_4_shot](https://huggingface.co/datasets/laolao77/ViRFT_CLS_fgvc_aircraft_4_shot)<br />[Car196_4_shot](https://huggingface.co/datasets/laolao77/ViRFT_CLS_car196_4shot)<br />[Pets37_4_shot](https://huggingface.co/datasets/laolao77/ViRFT_CLS_pets37_4shot)                                                           | <details><summary>Click</summary>Visual-RFT introduces Visual Reinforcement Fine-tuning, which extends reinforcement learning with verified rewards on visual perception tasks that are effective with limited data for fine-tuning.</details> |
| 2025.0306 | R1-VLM                | GroundLight        | [Blog](https://www.groundlight.ai/blog/visual-reasoning-models)<br />[GitHub](https://github.com/groundlight/r1_vlm)<br />[More](#r1-vlm) | ——                                                           | ——                                                           | <details><summary>Click</summary>R1-VLM enhances VLMs using RL, contributing significantly improved performance on complex visual reasoning tasks (spatial, counting, logic) where standard models falter. It shows that RL effectively unlocks advanced, multi-step reasoning capabilities specifically for vision-language understanding.</details> |
| 2025.0310 | VisualThinker-R1-Zero | TurningPoint       | [Paper](https://arxiv.org/pdf/2503.05132) <br />[GitHub](https://github.com/turningpoint-ai/VisualThinker-R1-Zero)<br />[More](#visual-r1-zero) | [VisualThinker-R1-Zero](https://huggingface.co/turningpoint-ai/VisualThinker-R1-Zero) | ——                                                           | <details><summary>Click</summary>VisualThinker-R1-Zero adapts the R1-Zero RL paradigm (no supervised fine-tuning) to VLMs, achieving SoTa visual reasoning. It shows that complex visual reasoning can be effectively cultivated directly via RL on a base VLM, bypassing supervised data needs.</details> |
| 2025.0310 | MM-EUREKA | USTC & ZTE & NEU      | [Paper](https://arxiv.org/pdf/2503.07365) <br />[Github](https://github.com/ModalMinds/MM-EUREKA) <br /> [More](#mm-eureka) | [MM-Eureka-Qwen-7B](https://huggingface.co/FanqingM/MM-Eureka-Qwen-7B) | [MM-Eureka-Dataset](https://huggingface.co/datasets/FanqingM/MM-Eureka-Dataset)       | <details><summary>Click</summary>MM-EUREKA reproduces key characteristics of text-based RL systems like DeepSeek-R1 in the multimodal space, which demonstrates that both instruction-tuned and pre-trained models can develop strong multimodal reasoning capabilities through rule-based RL without supervised fine-tuning, showing superior data efficiency compared to alternative approaches. </details> |
| 2025.0310 | Curr-ReFT | Shanghai AI Lab & SJTU & HKU       | [Paper](https://arxiv.org/pdf/2503.07065)<br />[GitHub](https://github.com/ding523/Curr_REFT)<br />[More](#curr-reft) | [3B-Curr-ReFT](https://huggingface.co/ZTE-AIM/3B-Curr-ReFT)<br />[7B-Curr-ReFT](https://huggingface.co/ZTE-AIM/7B-Curr-ReFT) | [Curr-ReFT-data](https://huggingface.co/datasets/ZTE-AIM/Curr-ReFT-data)       | <details><summary>Click</summary>Curr-ReFT proposes a Curriculum Reinforcement Finetuning strategy to enhance the out-of-distribution generalization and reasoning abilities. The curriculum paradim ensures steady progression. Moreover, a rejected sampling-based self-improvement is proposed to maintain the fundamental capabilities of VLMs through selective learning from high-quality multimodal and language examples. </details> |
| 2025.0311 | LLM-R1                | CUHK & Ant Group   | [Paper](https://arxiv.org/pdf/2503.07536)<br />[GitHub](https://github.com/TideDra/lmm-r1) | ——                                                           | ——                                                           | <details><summary>Click</summary>LLM-R1 contributes the RMAVO algorithm to stably enhance LLM reasoning using RL, preventing reward hacking and achieving SOTA results with smaller models via an open-source implementation. It shows that reward model assistance in value optimization is key for stable RL.</details> |
| 2025.0311 | Vision-R1             | ECNU & Xiaohongshu | [Paper](https://arxiv.org/abs/2503.06749)<br />[GitHub](https://github.com/Osilly/Vision-R1) | ——                                                           | [Vision-R1-cold](https://huggingface.co/datasets/Osilly/Vision-R1-cold) | <details><summary>Click</summary>Vision-R1 adapts the R1-Zero RL paradigm for VLMs, training them on visual reasoning chains. Its contribution is significantly boosting complex multimodal reasoning performance. It shows that RL applied to explicit reasoning steps effectively enhances VLM capabilities.</details> |
| 2025.0311 | MMR1             | NTU & SUTD & LASA | [GitHub](https://github.com/LengSicong/MMR1) | [MMR1-Math-v0-7B](https://huggingface.co/MMR1/MMR1-Math-v0-7B)    | [MMR1-Math-RL-Data-v0](https://huggingface.co/datasets/MMR1/MMR1-Math-RL-Data-v0) | <details><summary>Click</summary>MMR1-Math-v0 achieves state-of-the-art performance among open-source 7B multimodal models, competing effectively even against proprietary models with significantly larger parameter sizes—all trained using only 6k carefully curated data instances.</details> |
| 2025.0315 | MetaSpatial                | Northwestern University                                | [Paper](https://arxiv.org/abs/2503.18470)<br />[Project](https://github.com/PzySeere/MetaSpatial)<br />[GitHub](https://github.com/PzySeere/MetaSpatial) | ——                                                           | [3D_Reasoning](https://huggingface.co/datasets/zhenyupan/3d_layout_reasoning)                                                          | <details><summary>Click</summary>MetaSpatial leverages reinforcement learning to enhance 3D spatial reasoning in vision-language models (VLMs), enabling more structured, realistic, and adaptive scene generation for applications in the metaverse, AR/VR, and game development.</details> |
| 2025.0327 | Reason-RFT             | PKU & BAAI & CASIA & School of Artificial Intelligence, University of Chinese Academy of Sciences | [Paper](https://arxiv.org/pdf/2503.20752)<br />[GitHub](https://github.com/tanhuajie/Reason-RFT)<br />[Project](https://tanhuajie.github.io/ReasonRFT/) | ——                                                           | [tanhuajie2001/Reason-RFT-CoT-Dataset](https://huggingface.co/datasets/tanhuajie2001/Reason-RFT-CoT-Dataset/) | <details><summary>Click</summary>Reason-RFT introduces a two-phase training paradim: (1) SFT with CoT data to activate reasoning potential, followed by (2) GRPO-based reinforcement learning to enhance generalization, which further has potential applications in Emobodied AI.</details> |
| 2025.0404 | MAYE           | SJTU & GAIR                | [Paper](https://arxiv.org/pdf/2504.02587)<br />[GitHub](https://github.com/GAIR-NLP/MAYE) |——  | [ManTle/MAYE](https://huggingface.co/datasets/ManTle/MAYE) | <details><summary>Click</summary>MAYE is a transparent, reproducible framework and a comprehensive evaluation scheme for applying reinforcement learning (RL) to vision-language models (VLMs). Its codebase is developed entirely from scratch without relying on any existing RL toolkits.</details> |
| 2025.0408 | Step-R1-V-Mini           | StepFun               | [Website](https://platform.stepfun.com) |——  | —— | <details><summary>Click</summary>Step-R1-V-Mini excels in the domain of visual reasoning, while also demonstrating top-tier performance in mathematical, code, and textual reasoning tasks. It supports a context length of 100k.</details> |
| 2025.0409 | Kimi-VL-Thinking           | Kimi Team               | [Technical Report](https://github.com/MoonshotAI/Kimi-VL/blob/main/Kimi-VL.pdf)<br />[GitHub](https://github.com/MoonshotAI/Kimi-VL) |[moonshotai/Kimi-VL-A3B-Thinking](https://huggingface.co/moonshotai/Kimi-VL-A3B-Thinking)  | —— | <details><summary>Click</summary>Kimi-VL-Thinking is designed to enhance long-horizon reasoning capabilities in vision-language tasks.  Built on a foundation of long CoT SFT and RL, with only 2.8 parameters,  Kimi-VL-Thinking achieves strong performance across a range of tasks requiring long-term reasoning. It excels in domains such as MMMU, MathVision, and MathVista, achieving impressive scores of 61.7, 36.8, and 71.3, respectively.</details> |
| 2025.0409 | VideoChat-R1           | Shanghai AI Lab & NJU & ZJU & USTC & Shanghai Innovation Institute & SIAT               | [Paper](https://arxiv.org/pdf/2504.06958)<br />[GitHub](https://github.com/OpenGVLab/VideoChat-R1)  | —— | —— | <details><summary>Click</summary>VideoChat-R1 provides a systematic exploration of Reinforcement Fine-Tuning (RFT) with GRPO for video MLLMs, which exhibiting remarkable performance on spatio-temporal perception tasks without sacrificing chat ability, while exhibiting emerging spatio-temporal reasoning abilities. </details> |
| 2025.0410 | Perception-R1           | HUST & BUPT & StepFun & JHU & Tsinghua University        | [Paper](https://arxiv.org/pdf/2504.07954)<br />[GitHub](https://github.com/linkangheng/PR1)  | [Perception-R1](https://huggingface.co/collections/Kangheng/perception-r1-67f6b14f89d307a0ece985af) | [Perception-R1](https://huggingface.co/collections/Kangheng/perception-r1-67f6b14f89d307a0ece985af) | <details><summary>Click</summary>Perception-R1 explores the effects of RL on different perception tasks, the researchers observe that the percep- tual perplexity is a major factor in determining the effectiveness of RL. The scalable Perception-R1 achieves remarkable performance on the perception tasks.  </details> |
| 2025.0410 | VL-Rethinker           | TIGER-Lab        | [Paper](https://arxiv.org/pdf/2504.08837)<br />[GitHub](https://github.com/TIGER-AI-Lab/VL-Rethinker)  | [TIGER-Lab/VL-Rethinker-7B](https://huggingface.co/TIGER-Lab/VL-Rethinker-7B)<br />[TIGER-Lab/VL-Rethinker-72B](https://huggingface.co/TIGER-Lab/VL-Rethinker-72B) | —— | <details><summary>Click</summary>VL-Rethinker proposes Selective Sample Replay (SSR) and Forced Rethinking to enhance fast-thinking models.The model achieves remarkable performance on multi-disciplinary benchmarks.  </details> |
| <div id="vlm_latest">2025.0x0x</div> |             |                      | [Paper]()<br />[GitHub]() | [hf models]() | [hf datasets]() | <details><summary>Click</summary>insights and contributions about RL for reasoning within 30 words.</details> |


### Agentic Applications
| Date      | Project               | Org                | Intro                                                        | HF Model                                                     | HF Dataset                                                   | Takeaway Messages                                                 |
| --------- | --------------------- | ------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 2025.0126 | RAGEN              | RAGEN-AI                           | [Paper](https://arxiv.org/abs/2504.20073) <br /> [GitHub](https://github.com/RAGEN-AI/RAGEN)                  | ——                                                           | ——                                                           | <details><summary>Click</summary>RAGEN introduces a RL framework to train reasoning-capable LLM agents for interactive, stochastic environments. Its core contribution is the Reasoning-Interaction Chain Optimization (RICO) algorithm, which jointly optimizes reasoning and action strategies by reinforcing entire trajectories.</details> |
| 2025.0203 | Verifiers          | Independent                        | [GitHub](https://github.com/willccbb/verifiers) | ——                                                           | ——                                                           | <details><summary>Click</summary>This repository contains a set of tools for reinforcement learning with LLMs in verifiable environments. It can be used for LLM Agent RL in verifable environments.</details> |
| 2025.0303 | ReSearch              | Agent-RL           | [GitHub](https://github.com/Agent-RL/ReSearch)<br />[More](#research) | ——                                                           | ——                                                           | <details><summary>Click</summary>The project train LLMs from scratch, utilizing RL with GRPO to learn to reason via search operations, without reliance on pre-existing reasoning frameworks or supervised data.</details> |
| 2025.0312 | Search-R1             | UIUC & UMass Amherst | [Paper](https://arxiv.org/abs/2503.09516)<br />[GitHub](https://github.com/PeterGriffinJin/Search-R1)<br />[More](#search-r1) | [Search-R1](https://huggingface.co/collections/PeterJinGo/search-r1-67d1a021202731cb065740f5)   | [2018 Wikipedia](https://huggingface.co/datasets/PeterJinGo/wiki-18-corpus) | <details><summary>Click</summary>The paper introduces Search-R1, a novel RL framework that enables LLMs to interact with search engines in an interleaved manner with their own reasoning. The framework is shown to be effective, with experiments demonstrating average relative improvements of 41% and 20% over RAG baselines, and providing insights into RL optimization methods, LLM choices, and response length dynamics in retrieval-augmented reasoning.</details> |
| 2025.0318 | R1-Searcher           | RUC                | [Paper](https://arxiv.org/pdf/2503.05592)<br />[GitHub](https://github.com/RUCAIBox/R1-Searcher) | [Llama-3.1-8B-instruct-RAG-RL](https://huggingface.co/XXsongLALA/Llama-3.1-8B-instruct-RAG-RL) <br />[Qwen-2.5-7B-base-RAG-RL](https://huggingface.co/XXsongLALA/Qwen-2.5-7B-base-RAG-RL) | [RAG-RL-Hotpotqa](https://huggingface.co/datasets/XXsongLALA/RAG-RL-Hotpotqa-with-2wiki) | <details><summary>Click</summary>R1-Searcher enhances LLM reasoning via RL by training the model to perform adaptive model-based search during generation. This integration enables flexible thinking depth, improving reasoning efficiency and performance compared to fixed-step methods like R1-Zero.</details> |
| 2025.0319 | SWEET-RL           | Meta AI                            | [Paper](https://arxiv.org/abs/2503.15478)<br />[GitHub](https://github.com/facebookresearch/sweet_rl/tree/main) | ——                                                           | [collaborative_agent_bench](https://huggingface.co/datasets/facebook/collaborative_agent_bench) | <details><summary>Click</summary>Sweet-RL introduces a novel RL algorithm for multi-turn collaborative reasoning LLM agents. Its core contribution is improving credit assignment across long interactions by using an asymmetric actor-critic structure where the critic leverages additional training-time information for step-wise evaluation.</details> |
| <div id="agent_latest">2025.0x0x</div> |             |                      | [Paper]()<br />[GitHub]() | [hf models]() | [hf datasets]() | <details><summary>Click</summary>insights and contributions about RL for reasoning within 30 words.</details> |

## Projects

### Large Language Models

#### <div id="primerl">2025.0102, PRIME-RL</div>

| Project or Paper      | [Process Reinforcement through Implicit Rewards](https://arxiv.org/abs/2502.01456) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [PRIME-RL/PRIME](https://github.com/PRIME-RL/PRIME)          |
| Backbone Model        | Qwen2.5-Math-7B-Base                                         |
| RL Algorithm          | PPO/REINFORCE++/RLOO/GRPO + Online PRM                       |
| Training Dataset      | [PRIME-RL/Eurus-2-RL-Data](https://huggingface.co/datasets/PRIME-RL/Eurus-2-RL-Data), 150K |
| Rollout Configuration | 256 prompts * 4 responses Online Prompt Filtering (Accuracy in [0.2,0.8]) |
| Reward Function       | Rule-based Rewards + Implicit Process Rewards                |
| Policy Optimization   | PPO loss, without KL loss                                    |
| Benchmark             | GPT-4o level on AIME 2024, AMC, MATH-500, Minerva Math, OlympiadBench, LeetCode, and LiveCodeBench |
| Core Insights         | Implicit PRM efficiently addresses reward sparsity, distribution shift, and scalability by directly learning token-level rewards within a language model framework, eliminating the need for separate value models or prior training. |
| Additional Notes      |                                                              |



#### <div id="deepseek-r1">2025.0122, DeepSeek-R1</div>

| Project or Paper      | [DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](https://arxiv.org/pdf/2501.12948) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [deepseek-ai/DeepSeek-R1](https://github.com/deepseek-ai/DeepSeek-R1) |
| Backbone Model        | DeepSeek-V3-Base                                             |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | Unclear                                                      |
| Rollout Configuration | 4~64 samples for each prompt, temperature = 0.6              |
| Reward Function       | Rule-based Rewards                                           |
| Policy Optimization   | vanilla GRPO Loss                                            |
| Benchmark             | OpenAI-o1 level on AIME 2024, Codeforces, GPQA Diamond, MATH-500, MMLU, SWE-bench Verified. |
| Core Insights         | RL can boost LLMs' reasoning. DeepSeek - R1 series models prove effective, and distilling reasoning to small models works, while highlighting challenges in other methods. |
| Additional Notes      |                                                              |



#### <div id="kimi-k1.5">2025.0122, Kimi k1.5</div>

| Project or Paper      | [Kimi k1.5: Scaling Reinforcement Learning with LLMs](https://arxiv.org/pdf/2501.12599) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [MoonshotAI/Kimi-k1.5](https://github.com/MoonshotAI/Kimi-k1.5) |
| Backbone Model        | Kimi k-series model (closed source)                          |
| RL Algorithm          | Online Policy Mirror Decent/Length Penalty Reward/Curriculum Sampling/Prioritized Sampling/Chain-of-Thought RM/Long2short RL |
| Training Dataset      | Code: 1000 contest problem; </br>Math: 800k in-context learning/800k chain-of-thought data; </br> Vision: unknown number of real-world/synthetic visual reasoning/text-rendered data |
| Rollout Configuration | None                                                         |
| Reward Function       | Outcome Reward+Length Penalty Reward                         |
| Policy Optimization   | Online Policy Mirror Decent                                  |
| Benchmark             | Matching OpenAI’s o1 on AIME/MATH500/Codeforces/MathVista    |
| Core Insights         | Effective long2short methods that use long-CoT techniques to improve short-CoT models, yielding state-of-the-art short-CoT reasoning results, outperforming existing short-CoT models. |
| Additional Notes      |                                                              |



#### <div id="tinyzero">2025.0124, TinyZero</div>

| Project or Paper      | not applicable                                               |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [Tiny-Zero](https://github.com/Jiayi-Pan/TinyZero) |
| Backbone Model        | QWen-2.5-3B                                                  |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | countdown                                                    |
| Rollout Configuration | 1024                                                         |
| Reward Function       | 0/1 reward                                                   |
| Policy Optimization   | vanilla GRPO: (KL Loss; Length Penalty; Token-level loss)    |
| Benchmark             | test set of countdown                                        |
| Core Insights         | Aha moment can be reproducible on puzzle-style data.         |
| Additional Notes      |                                                              |



#### <div id="simplerl">2025.0125, SimpleRL</div>

| Project or Paper      | [7B Model and 8K Examples: Emerging Reasoning with Reinforcement Learning is Both Effective and Efficient](https://hkust-nlp.notion.site/simplerl-reason) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [hkust-nlp/simpleRL-reason](https://github.com/hkust-nlp/simpleRL-reason) |
| Backbone Model        | Qwen2.5-Math-7B                                              |
| RL Algorithm          | PPO based on OpenRLHF                                        |
| Training Dataset      | [MATH](https://huggingface.co/datasets/EleutherAI/hendrycks_math), 8k Level3-Level5 |
| Rollout Configuration | 128 prompts * 8 responses; Temperature = 0.6                 |
| Reward Function       | Rule-based Rewards                                           |
| Policy Optimization   | PPO loss with 0.01 KL coefficient                            |
| Benchmark             | GPT-4o level on AIME2024, AMC2023, College Math, Gaokao2023en, GSM8k, MATH500, Minerva Math, and OlympiadBench. |
| Core Insights         | Long Chain-of-Thought (CoT) and self-reflection can emerge on a 7B model with only few high-quality examples with rule-based rewards only. |
| Additional Notes      |                                                              |



#### <div id="demystify">2025.0206, Demysitify-long-CoT</div> 

| Project or Paper      | [Demystifying Long Chain-of-Thought Reasoning in LLMs](https://arxiv.org/pdf/2502.03373) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [eddycmu/demystify-long-cot](https://github.com/eddycmu/demystify-long-cot) |
| Backbone Model        | Qwen2.5-Math-7B Llama-3.1-8B                                 |
| RL Algorithm          | PPO (OpenRLHF)                                               |
| Training Dataset      | 7500 training samples of MATH                                |
| Rollout Configuration | 512 prompts * 8 responses; temperature=0.7, top-p=0.95 Context Length Prompt=2048, Gen=14384 tokens |
| Reward Function       | Rule-based Reward + Cosine Length Reward + Repetition Penalty Reward |
| Policy Optimization   | KL coefficy=0.01, gamma=1, lambda=1                          |
| Benchmark             | MATH, AIME, TheoremQA, MMLU-Pro-1k                           |
| Core Insights         | Reward shaping can be used to stabilize and control CoT length while improving accuracy. Cosine reward can be tuned to incentivize various length scaling behaviors, length rewards will be hacked with enough compute. But this can be mitigated using a repetition penalty. |
| Additional Notes      |                                                              |





#### <div id="deepscaler">2025.0210, DeepScaler</div>

| Project or Paper      | [DeepScaleR: Surpassing O1-Preview with a 1.5B Model by Scaling RL](https://pretty-radio-b75.notion.site/DeepScaleR-Surpassing-O1-Preview-with-a-1-5B-Model-by-Scaling-RL-19681902c1468005bed8ca303013a4e2) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [deepscaler](https://github.com/agentica-project/deepscaler) |
| Backbone Model        | deepseek-ai/DeepSeek-R1-Distill-Qwen-1.5B                    |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | [Omni-MATH](https://omni-math.github.io/) and [Still](https://github.com/RUCAIBox/Slow_Thinking_with_LLMs) |
| Rollout Configuration | 128 * 16 (bs*n);temperature=0.6; Context Length:8K->16K->24K |
| Reward Function       | 0/1 reward                                                   |
| Policy Optimization   | vanilla GRPO: (KL Loss; Length Penalty; Token-level loss)    |
| Benchmark             | AIME 2024/ MATH 500 /AMC 2023 / Minerva Math/ OlympiadBench  |
| Core Insights         | 1. RL scaling can manifest in small models as well. 2. Iterative lengthening enables more effective length scaling. |
| Additional Notes      | Iteratively increasing the max context for RL training.      |



#### <div id="logicrl">2025.0210, Logic-RL</div> 

| Project or Paper      | [Logic-RL: Unleashing LLM Reasoning with Rule-Based Reinforcement Learning](https://arxiv.org/abs/2502.14768) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [Unakar/Logic-RL](https://github.com/Unakar/Logic-RL)        |
| Backbone Model        | Qwen2.5-Math-7B / Qwen2.5-7B-Instruct                        |
| RL Algorithm          | REINFORCE++                                                  |
| Training Dataset      | [Knights and Knaves (K&K) puzzles](https://huggingface.co/datasets/K-and-K/knights-and-knaves), 6.2k |
| Rollout Configuration | 8 prompts * 8 responses; Temperature = 0.7                   |
| Reward Function       | Rule-based Rewards                                           |
| Policy Optimization   | REINFORCE++ loss with 0.001 unbiased KL coefficient.         |
| Benchmark             | o3-mini-high level on K&K logic puzzle                       |
| Core Insights         | With simple REINFORCE++ with KL loss, 7B model develops advanced reasoning skills that are absent from the logic corpus and generates to other tasks like math. |
| Additional Notes      |  |


#### <div id="oreal">2025.0210, OREAL</div>

| Project or Paper      | [Exploring the Limit of Outcome Reward for Learning Mathematical Reasoning](https://arxiv.org/abs/2502.06781) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [InternLM/OREAL](https://github.com/InternLM/OREA)           |
| Backbone Model        | Qwen2.5-7B / Qwen2.5-32B                                     |
| RL Algorithm          |   |
| Training Dataset      | [OREAL-RL-Prompts](https://huggingface.co/datasets/internlm/OREAL-RL-Prompts), 4k |
| Rollout Configuration | 64 prompts * 16 responses; Temprature = 1.0; Online Accuracy Filtering; Retain only one correct and wrong solutions |
| Reward Function       | Outcome Reward Signal by rule-based verifier and Qwen2.5-72B-Instruct + Token level Reward |
| Policy Optimization   | OREAL loss with 0.01 KL coefficient                          |
| Benchmark             | R1-level on MATH500, AIME2024, AIME2025-I, LiveMath, Olympiad |
| Core Insights         | Behavior cloning on positive samples is sufficient for optimal learning and reward reshaping for negative samples is needed for consistent gradient estimation. A token-level reward model can be trained to addresses sparse rewards. |
| Additional Notes      | |



#### <div id="limr">2025.0217, LIMR</div>

| Project or Paper      | [LIMR: Less is More for RL Scaling](https://arxiv.org/abs/2502.11886) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [GAIR-NLP/LIMR](https://github.com/GAIR-NLP/LIMR)            |
| Backbone Model        | Qwen2.5-Math-7B                                              |
| RL Algorithm          | PPO based on OpenRLHF                                        |
| Training Dataset      | [LIMR](https://huggingface.co/datasets/GAIR/LIMR), 1.4k      |
| Rollout Configuration | 1024 prompts * 8 responses; Temperature = 1.2                |
| Reward Function       | Rule-based Rewards                                           |
| Policy Optimization   | PPO loss with 0.01 KL coefficient                            |
| Benchmark             | GPT-4o level on AIME2024, MATH500, AMC2023                   |
| Core Insights         | Precisely selected data may be the key to unlocking the enhanced reasoning capabilities of LLMs. |
| Additional Notes      | The author uses the trained model's average reward curve as a reference for measuring sample effectiveness. |



#### <div id="openreason-zero">2025.0217, Open-Reasoner-Zero</div>

| Project or Paper      | [Open-Reasoner-Zero: An Open Source Approach to Scaling Up Reinforcement Learning on the Base Model](https://github.com/Open-Reasoner-Zero/Open-Reasoner-Zero/blob/main/ORZ_paper.pdf) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [Open-Reasoner-Zero/Open-Reasoner-Zero](https://github.com/Open-Reasoner-Zero/Open-Reasoner-Zero) |
| Backbone Model        | Qwen2.5-7B, Qwen2.5-32B                                      |
| RL Algorithm          | PPO based on OpenRLHF                                        |
| Training Dataset      | [ORZ-MATH](https://github.com/Open-Reasoner-Zero/Open-Reasoner-Zero/tree/main/data), 57k |
| Rollout Configuration | 128 prompts * 64 responses; Temperature = 1.0                |
| Reward Function       | Rule-based Rewards                                           |
| Policy Optimization   | PPO loss without KL loss                                     |
| Benchmark             | GPT-4o level on GPQA-Diamond, MATH500, AIME2024              |
| Core Insights         | Vanilla PPO with GAE and rule-based rewards without KL loss is sufficient to sclae up response length and benchmark performance. |
| Additional Notes      |                                                              |



#### <div id="swerl"> 2025.0225, SWE-RL</div> 

| Project or Paper      | [SWE-RL: Advancing LLM Reasoning via Reinforcement Learning on Open Software Evolution](https://arxiv.org/abs/2502.18449) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [facebookresearch/swe-rl](https://github.com/facebookresearch/swe-rl) |
| Backbone Model        | Llama-3.3-70B-Instruct                                       |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | Publicly available repositories                              |
| Rollout Configuration | 32 prompts * 16 rollouts                                     |
| Reward Function       | Similarity Function (`difflib.SequenceMatcher`)              |
| Policy Optimization   | Normalized Rewards for Advantage Calculation                 |
| Benchmark             | GPT-4o level on SWE-bench Verified (41%)                     |
| Core Insights         | SWE-RL enhances LLMs' code reasoning through RL using open-source software evolution data, achieving state-of-the-art results in software engineering tasks and demonstrating generalized reasoning capabilities beyond coding. |
| Additional Notes      |                                                              |



#### <div id="vcppo">2025.0303, VC-PPO </div>

| Project or Paper      | [What’s Behind PPO’s Collapse in Long-CoT? Value Optimization Holds the Secret](https://arxiv.org/pdf/2503.01491) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | N/A                                                          |
| Backbone Model        | Qwen2.5-32B-Base                                             |
| RL Algorithm          | VC-PPO                                                       |
| Training Dataset      | A compilation of questions from all past AIME competitions (excluding the last two years), supplemented with artificially constructed challenging mathematical problems. |
| Rollout Configuration | N/A                                                          |
| Reward Function       | Rule-based Rewards                                           |
| Policy Optimization   | PPO loss, Value Estimate with Decoupled-GAE                  |
| Benchmark             | AIME 2024, GPQA, CodeForces                                  |
| Core Insights         | VC-PPO addresses PPO’s failure in long CoT tasks by pretraining the value model to correct initialization bias and decoupling GAE between the actor and critic to mitigate reward signal decay. |
| Additional Notes      |                                                              |



#### <div id="lcpol1">2025.0306, LCPO-L1 </div>


| Project or Paper      | [L1: Controlling How Long A Reasoning Model Thinks With Reinforcement Learning ](https://www.arxiv.org/pdf/2503.04697) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [cmu-l3/l1](https://github.com/cmu-l3/l1)                    |
| Backbone Model        | DeepScaleR-1.5B-Preview                                      |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | [DeepScaleR-Preview-Dataset](https://huggingface.co/datasets/agentica-org/DeepScaleR-Preview-Dataset), 40k |
| Rollout Configuration | 128 prompts                                                  |
| Reward Function       | correctness reward + length penalty                          |
| Policy Optimization   | GRPO loss + length penalty loss                              |
| Benchmark             | AIME 2025, MATH, AMC, Olympiad-Bench, GPQA, LSAT, MMLU       |
| Core Insights         | Address the uncontrolled reasoning length issue in language models. It uses reinforcement learning to optimize for both accuracy and adherence to user - specified length constraints. By training models with a reward function that combines correctness and length - related terms, LCPO enables precise length control, allowing for a better trade - off between computational cost and accuracy in various reasoning tasks. |
| Additional Notes      |                                                              |



#### <div id="metarl">2025.0310, MetaRL </div>

| Project or Paper      | [Optimizing Test-Time Compute via Meta Reinforcement Fine-Tuning](https://arxiv.org/pdf/2503.07572) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [CMU-AIRe/MRT](https://github.com/CMU-AIRe/MRT)              |
| Backbone Model        | DeepSeek-R1-Distill-Qwen-32B/7B/1.5B / DeepScaleR-1.5B-Preview /  Llama-3.1-8B/3B-Instruct |
| RL Algorithm          | MRT                                                          |
| Training Dataset      | None                                                         |
| Rollout Configuration | 256 prompts * 4 responses, temperature = 0.7                 |
| Reward Function       | 0/1 reward + dense reward                                    |
| Policy Optimization   | SFT Loss + Dense Reward Bonus Loss                           |
| Benchmark             | AIME 2024, AIME 2025, AMC 2023, MinervaMATH, MATH500         |
| Core Insights         | Treating test - time computation of LLMs as a meta - RL problem. It uses a progress - based reward function to guide the model, and optimizes the policy to balance exploration and exploitation, aiming to improve the efficiency and performance of LLMs at test time. |
| Additional Notes      |                                                              |



#### <div id="topr">2025.0318, TOPR </div>

| Project or Paper      | [Tapered Off-Policy REINFORCE Stable and efficient reinforcement learning for LLMs](https://arxiv.org/pdf/2503.14286v2) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [None](http://None)                                          |
| Backbone Model        | Llama 3 8B/70B                                               |
| RL Algorithm          | Tapered Off-Policy REINFORCE (TOPR)                          |
| Training Dataset      | GSM8K and MATH                                               |
| Rollout Configuration | 64/8 solutions each question for GSM8k/MATH, respectively    |
| Reward Function       | Implicit Reward as DPO (contrastive learning with preference data) |
| Policy Optimization   | Optimization with off-policy samples and without KL penalty  |
| Benchmark             | The performance of 8B language models can match with 70B-parameter model's on GSM8K and MATH |
| Core Insights         | Properly leveraging positive and negative examples alike in the off-policy regime simultaneously increases test-time accuracy and training data efficiency, all the while avoiding the “wasted inference” that comes with discarding negative examples. |
| Additional Notes      | This method may speed up learning while maintaining stable learning dynamics, without the use of KL regularization and online sampling. |



#### <div id="dapo">2025.0318, DAPO</div>

| Project or Paper      | [DAPO: An Open-Source LLM Reinforcement Learning System at Scale](https://arxiv.org/pdf/2503.14476) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [BytedTsinghua-SIA/DAPO](https://github.com/BytedTsinghua-SIA/DAPO) |
| Backbone Model        | Qwen2.5-32B-Base                                             |
| RL Algorithm          | DAPO                                                         |
| Training Dataset      | [BytedTsinghua-SIA/DAPO-Math-17k](https://huggingface.co/datasets/BytedTsinghua-SIA/DAPO-Math-17k), 17K |
| Rollout Configuration | 512 prompts * 16 responses Dynamic Sampling                  |
| Reward Function       | Rule-based Rewards + Length-Aware Penalty Reward (Overlong Filtering strategy)           |
| Policy Optimization   | DAPO loss, without KL loss                                   |
| Benchmark             | DeepSeek-R1-Zero-Qwen-32B level on AIME 2024                 |
| Core Insights         | DAPO introduces four key techniques: Clip-Higher to promote diversity and prevent entropy collapse; Dynamic Sampling to enhance training efficiency and stability; Token-Level Policy Gradient Loss to refine long-chain reasoning; and Overlong Reward Shaping to reduce reward noise and stabilize training. |
| Additional Notes      |                                                              |

#### <div id="open-rs">2025.0320, Open RS</div>

| Project or Paper      | [Reinforcement Learning for Reasoning in Small LLMs: What Works and What Doesn’t](https://arxiv.org/pdf/2503.16219) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [knoveleng/open-rs](https://github.com/knoveleng/open-rs) |
| Backbone Model        | DeepSeek-R1-Distill-Qwen-1.5B                                                 |
| RL Algorithm          | GRPO                 |
| Training Dataset      | [open-s1](https://huggingface.co/datasets/knoveleng/open-s1), 18.6k</br>[open-deepscalar](https://huggingface.co/datasets/knoveleng/open-deepscaler), 21k</br>[open-rs](https://huggingface.co/datasets/knoveleng/open-rs), 7k</br>                             |
| Rollout Configuration | 24 prompts * 6 responses, Temperature = 0.7                                                          |
| Reward Function       | Rule-based Rewards with Cosine Reward assigning higher rewards to shorter but correct response.                                           |
| Policy Optimization   | GRPO       |
| Benchmark             | AIME2024, AMC, MATH500, Minerva Math and OlympiadBench       |
| Core Insights         | 1. High-quality data can boost performance compared with large amount low-quality data. 2. The difficulty of training data influences the training results. 3. Consine rewards can stabilize completion lengths, improving training consistency, |
| Additional Notes      |                                                              |

#### <div id="oat-zero">2025.0321, Oat-Zero</div>

| Project or Paper      | [Understanding R1-Zero-Like Training: A Critical Perspective](https://github.com/sail-sg/understand-r1-zero/blob/main/understand-r1-zero.pdf) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [sail-sg/understand-r1-zero](https://github.com/sail-sg/understand-r1-zero) |
| Backbone Model        | Qwen2.5-1.5B                                                 |
| RL Algorithm          | Dr. GRPO (fixes GRPO’s bias in optimization)                 |
| Training Dataset      | Questions sampled from the MATH;                             |
| Rollout Configuration | N/A                                                          |
| Reward Function       | Rule-based Rewards                                           |
| Policy Optimization   | Dr. GRPO Loss (remove two normalization terms in GRPO)       |
| Benchmark             | AIME2024, AMC, MATH500, Minerva Math and OlympiadBench       |
| Core Insights         | 1. The DeepSeek-V3-Base model exhibits significant reasoning capabilities, termed an “aha moment,” even prior to reinforcement learning fine-tuning. 2. GRPO introduces an optimization bias that artificially increases response length during training, particularly affecting incorrect outputs. |
| Additional Notes      |                                                              |

#### <div id="argo">2025.0328, ARGO</div>

| Project or Paper      | [RL-finetuning LLMs from On- and Off-Policy Data with a Single Algorithm](https://arxiv.org/pdf/2503.19612) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | -- |
| Backbone Model        | Qwen2.5-1.5B                                                 |
| RL Algorithm          | ARGO |
| Training Dataset      | MATH;                             |
| Rollout Configuration | N/A                                                          |
| Reward Function       | Computed based on the similarity of sampled answer and ground truth answer |
| Policy Optimization   | ARGO       |
| Benchmark             | MATH500    |
| Core Insights         | Incorporating ground truth answer into RL training can achieve a better convergence of loss and reward. |
| Additional Notes      |                                                              |

#### <div id="vapo">2025.0407, VAPO</div>

| Project or Paper      | [VAPO: Efficient and Reliable Reinforcement Learning for Advanced Reasoning Tasks](https://arxiv.org/pdf/2504.05118) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | -- |
| Backbone Model        | Qwen-32B                                                 |
| RL Algorithm          | Value-based Augmented PPO              |
| Training Dataset      | N/A                             |
| Rollout Configuration | N/A                                                          |
| Reward Function       | Rule-based Rewards                                           |
| Policy Optimization   | PPO       |
| Benchmark             | AIME 2024       |
| Core Insights         | VAPO integrates clip-higher, token-level loss, value-pretraining, decoupled-GAE, self-imitation learning and group-sampling.  |
| Additional Notes      |       First value-based RL training framework to outperform value-free methods on long COT tasks significantly   |

#### <div id="seed-thinking-v1.5">2025.0410, Seed-Thinking-v1.5</div>

| Project or Paper | [Seed-Thinking-v1.5: Advancing Superb Reasoning Models with Reinforcement Learning](https://github.com/ByteDance-Seed/Seed-Thinking-v1.5/blob/main/seed-thinking-v1.5.pdf) |
| --------------------- | ------------------------------------------------------------ |
| GitHub | [ByteDance-Seed/Seed-Thinking-v1.5](https://github.com/ByteDance-Seed/Seed-Thinking-v1.5) |
| Backbone Model | Doubao series model |
| RL Algorithm | VAPO, DAPO |
| Training Dataset | RL (Verifiable: STEM, code, logical puzzle; Non-verifiable: non-reasoning tasks including creative writing, translation, knowledge QA, role-playing...); SFT (300k verifiable data from RL training set, 100k non-verifiable data from SFT data of Doubao-Pro 1.5) |
| Rollout Configuration | Streaming Rollout System |
| Reward Function | Seed-Verifier and Seed-Thinking-Verifier that generates YES or NO with or without reasoning for verifiable problems; Pairwise generative reward model with probability of YES or NO for non-verifiable problems |
| Policy Optimization | PPO |
| Benchmark | AIME 2024, AIME 2025, BeyondAIME, Codeforces, GPQA diamond, superGPQA, ARC-AGI, SimpleQA, Collie, IFEval, SWE-bench, MMLU_PRO, LiveCodeBench, Aider Polyglot |
| Core Insights | 1. Generative reward model improves training stability with mixed verifiable and non-verifiable data by minimizing conflicts; 2. Training RL techniques (Value-pretraining, Decoupled-GAE, Length-adaptive GAE, Dynamic Sampling, Clip-Higher, Token-level Loss, Positive Example LM Loss, Online Data Distribution Adaptation); 3. Heavy emphasis on chain-of-thought (CoT)-rich reasoning data; 4. Infrastructure (Streaming Rollout System and hybrid parallelism strategies) |
| Additional Notes | Seed-Thinking-v1.5 is a Mixture-of-Experts (MoE) model, featuring 20B activated and 200B total parameters. Two new benchmarks, BeyondAIME and Codeforces. |

#### <div id="skywork-or1">2025.0413, Skywork-OR1</div>

| Project or Paper      | [Skywork Open Reasoner Series](https://capricious-hydrogen-41c.notion.site/Skywork-Open-Reasoner-Series-1d0bc9ae823a80459b46c149e4f51680) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [SkyworkAI/Skywork-OR1](https://github.com/SkyworkAI/Skywork-OR1) |
| Backbone Model        | DeepSeek-R1-Distill-Qwen-32B and DeepSeek-R1-Distill-Qwen-7B |
| RL Algorithm          | Multi-stage GRPO with adaptive entropy control |
| Training Dataset      | [Skywork-OR1-RL-Data](https://huggingface.co/datasets/Skywork/Skywork-OR1-RL-Data) |
| Rollout Configuration | 256 prompts * 16 responses, with temperature = 1.0 and online filtering and rejection sampling |
| Reward Function       | Rule-based Rewards |
| Policy Optimization   | GRPO with adaptive entropy loss |
| Benchmark             | AIME 2024, AIME 2025, LiveCodeBench (8/1/24-2/1/25) |
| Core Insights         | 1. Multi-stage GRPO training with scaled-up context window improves training efficiency without sacrificing performance.<br/>2. Advantage masks of truncated samples, while seems intuitive, does not transfer to performance.<br/>3. Adaptive entropy control robustly prevents entropy collapse and allows diverse sampling and continuous learning and improvement. |
| Additional Notes      | |

#### <div id="d1 & diffu-GRPO">2025.0416, d1 & diffu-GRPO</div>

| Project or Paper      | [d1: Scaling Reasoning in Diffusion Large Language Models via Reinforcement Learning](https://arxiv.org/pdf/2504.12216) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [dllm-reasoning/d1](https://github.com/dllm-reasoning/d1) |
| Backbone Model        | LLaDA-8B-Instruct                                          |
| RL Algorithm          | diffu-GRPO |
| Training Dataset      | GSM8K, MATH, Countdown, Sudoku;                             |
| Rollout Configuration | N/A                                                          |
| Reward Function       | Rule-based Rewards |
| Policy Optimization   |  |
| Benchmark             | GSM8K, MATH500, Countdown, Sudoku|
| Core Insights         | Attemping to improve the reasoning of diffusion LMs based on RL Algorithms. |
| Additional Notes      |                                                              |

### Multimodal Models

#### <div id="open-r1-mm">2025.0128, open-r1-multimodal</div>

| Project or Paper      | [EvolvingLMMs-Lab/open-r1-multimodal](https://github.com/EvolvingLMMs-Lab/open-r1-multimodal) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [EvolvingLMMs-Lab/open-r1-multimodal](https://github.com/EvolvingLMMs-Lab/open-r1-multimodal) |
| Backbone Model        | Qwen2-VL 2B/7B                                               |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | [multimodal-open-r1-8k-verified](https://huggingface.co/datasets/lmms-lab/multimodal-open-r1-8k-verified), 7.69K; |
| Rollout Configuration | 1 (prompts + images) * 8 responses; Temperature=0.9;         |
| Reward Function       | Rule-based Rewards (Choice, Format)                          |
| Policy Optimization   | PPO Loss                                                     |
| Benchmark             | MMMU:  <br />2B: +4.02% vs w./ reasoning, -4.48% vs base; <br />7B: 7.5% vs w./ reasoning, -1.2% vs base;  <br />Mathvista-mini:  <br />2B: +0.8% vs w./ reasoning, -2.2% vs base; <br />7B: -0.3% vs w./ reasoning, +3.5% vs base; |
| Core Insights         |                                                              |
| Additional Notes      |                                                              |



#### <div id="r1v">2025.0202, R1-V</div>

| Project or Paper      | [RLVR in Vision Language Models: Findings, Questions and Directions](https://deepagent.notion.site/rlvr-in-vlms) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [Deep-Agent/R1-V](https://github.com/Deep-Agent/R1-V[)       |
| Backbone Model        | Visual Counting/Complex Visual Reasoning: Qwen2-VL-2B-Instruct; <br />Geometry Reasoning: Qwen2.5-VL-7B-Instruct; |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | Visual Counting: [Clevr CoGenT-A](https://huggingface.co/datasets/leonardPKU/clevr_cogen_a_train), 70K<br /> Geometry Reasoning: [GeoQA-Train](https://huggingface.co/datasets/leonardPKU/GEOQA_R1V_Train_8K), 8K<br /> Complex Visual Reasoning: [Clevr_CoGenT_TrainA_R1](https://huggingface.co/datasets/MMInstruction/Clevr_CoGenT_TrainA_R1), 37.8K |
| Rollout Configuration | 1 (prompts + images) * 8 responses; Temperature=1.0;         |
| Reward Function       | Rule-based Rewards (Accuracy: Number/bool, Format)           |
| Policy Optimization   | PPO Loss                                                     |
| Benchmark             | Visual Counting (Acc.): Clevr CoGenT-B: 46%, comparable vs base and CoT+SFT models; SuperClevr:  40%, 11% higher than base and CoT+SFT models;  <br />Geometry Reasoning (Acc., no CoT data): GeoQA-Test: 24%, 1% higher than base and SFT models;  <br />Complex Visual Reasoning: SuperClevr: 53.48%, 49.28% higher than base and CoT+SFT models; |
| Core Insights         |                                                              |
| Additional Notes      |                                                              |



#### <div id="vlm-r1">2025.0215, VLM-R1</div>

| Project or Paper      | [VLM-R1: A stable and generalizable R1-style Large Vision-Language Model](https://om-ai-lab.github.io/index.html) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [om-ai-lab/VLM-R1](https://github.com/om-ai-lab/VLM-R1)      |
| Backbone Model        | Qwen2.5-VL-3B                                                |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | [COCO](https://cocodataset.org/#download), 83K, no improvement for both STF and RL model<br /> [Description Detection Dataset](https://github.com/shikras/d-cube), 24K; |
| Rollout Configuration | 8 (prompts + images) * 8 responses; Temperature=0.9;         |
| Reward Function       | Rule-based Rewards (IoU, Format)                             |
| Policy Optimization   | PPO Loss + KL Loss (default 0.04)                            |
| Benchmark             | OVDEval: 6.55%, 4.51% higher than base and SFT models in NMS-AP; <br />COCO(filter out images with more than 10 bbox): 6.1%, 2.6% higher than base and SFT models in MAP; |
| Core Insights         |                                                              |
| Additional Notes      |                                                              |


#### <div id="vlm-r1">2025.0303, Visual-RFT</div>

| Project or Paper      | [Visual-RFT: Visual Reinforcement Fine-Tuning ](https://arxiv.org/pdf/2503.01785) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [Liuziyu77/Visual-RFT](https://github.com/Liuziyu77/Visual-RFT)      |
| Backbone Model        | Qwen2-VL-2/7B                                                |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | [ViRFT Datasets] (https://huggingface.co/collections/laolao77/virft-datasets-67bc271b6f2833eccc0651df)，6K/6k/32/408/400/784/148; |
| Rollout Configuration | 2 * 8 responses; Temperature=1.0;                            |
| Reward Function       | Rule-based Rewards (Accuracy, IoU, Format)；                  |
| Policy Optimization   | PPO Loss                         |
| Benchmark             | Qwen2-VL-2B:<br />Fine-grained classification, Avg. Acc.（Flower102, Pets37, FGVC-Aircraft, Car196）:<br />1-shot +24.3%, +28.6%, 2-shot +27.5%, +24.7, 4-shot +25.9% , +26.3%, 8-shot +29.1%, +24.8%, 16-shot +29.3%, +21.3%, compared to base and SFT;<br />Object Detection (COCO), mAP:<br />1-shot +14.0%, +14.1%, 2-shot +21.9%, +20.5%, 4-shot +21.0%, +15.4%, 8-shot +27.8%, 17.2%, 16-shot +27.2%, +15.5%,  compared to base and SFT;<br />Rare Object Detection (LVIS), mAP:<br />10-shot, +15.4%, +9.4%,  compared to base and SFT;<br />Open Vocabulary Object Detection, mAP:<br />COCO: +21.5%, +17.7%, compared to base and SFT;<br />LVIS: +18.0%, +13.1%, compared to base and SFT;<br />Reasoning Grounding (LISA), mIoU:<br />+10.7%, +9.3%,  compared to base and SFT;<br /><br />Qwen2-VL-7B:<br />Object Detection (COCO), mAP:<br />4-shot +11.3%, +10.2%,  compared to base and SFT;<br />Rare Object Detection (LVIS), mAP:<br />10-shot, +18.4%, +6.2%,  compared to base and SFT;<br />Open Vocabulary Object Detection, mAP:<br />COCO: +9.5%, +10.1%, compared to base and SFT;<br />LVIS: +14.7%, +6.4%, compared to base and SFT;<br />Reasoning Grounding (LISA), mIoU:<br />+3.5%, +4.8%,  compared to base and SFT; |
| Core Insights         |                                                              |
| Additional Notes      |                                                              |


#### <div id="r1-vlm">2025.0306, r1-vlm</div>

| Project or Paper      | [GRPO for vision - Teaching an LLM to reason about images](https://www.groundlight.ai/blog/visual-reasoning-models) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [groundlight/r1_vlm](https://github.com/groundlight/r1_vlm)  |
| Backbone Model        | Qwen2.5-VL-3B-Instruct                                       |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | Message Decoding: [message-decoding-words-and-sequences-r1](https://huggingface.co/datasets/sunildkumar/message-decoding-words-and-sequences-r1), 27K<br /> Message Decoding-Single Word [message-decoding-words-r1](https://huggingface.co/datasets/sunildkumar/message-decoding-words-r1), 10K<br />Digit Recognition: [digit-recognition-r1 ](https://huggingface.co/datasets/sunildkumar/digit-recognition-r1), 2K |
| Rollout Configuration | 1 (prompts + images) * 9 responses; Temperature=1.0;         |
| Reward Function       | Rule-based Rewards (Decoding, Correctness, Format)           |
| Policy Optimization   | PPO Loss + KL Loss (default 0.01)                            |
| Benchmark             | -                                                            |
| Core Insights         |                                                              |
| Additional Notes      |                                                              |



#### <div id="visual-r1-zero">2025.0310, VisualThinker-R1-Zero</div>

| Project or Paper      | [R1-Zero’s “Aha Moment” in Visual Reasoning on a 2B Non-SFT Model](https://arxiv.org/pdf/2503.05132) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [turningpoint-ai/VisualThinker-R1-Zero](https://github.com/turningpoint-ai/VisualThinker-R1-Zero) |
| Backbone Model        | Qwen2-VL-2B                                                  |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | [SAT](https://huggingface.co/datasets/array/SAT), 218K;      |
| Rollout Configuration | 4 (prompts + images) * 8 responses; Temperature=1.0;         |
| Reward Function       | Rule-based Rewards (Accuracy-String Match, Format);         |
| Policy Optimization   | PPO Loss + KL Loss (default 0.04)                            |
| Benchmark             | CV-Bench (Choice): +25% vs base, +10.83% vs SFT;<br /> BLINK: +46.44 vs base, +0.75% vs SFT; <br />VSR: +62.32% vs base, +26.53% vs SFT; |
| Core Insights         |                                                              |
| Additional Notes      |                                                              |


#### <div id="mm-eureka">2025.0310, MM-Eureka</div>

| Project or Paper      | [MM-EUREKA: EXPLORING VISUAL AHA MOMENT WITH RULE-BASED LARGE-SCALE REINFORCEMENT LEARNING](https://arxiv.org/pdf/2503.07365) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [ModalMinds/MM-EURRKA](https://github.com/ModalMinds/MM-EUREKA) |
| Backbone Model        | InternVL2.5-Pretrained-38B                                                 |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | [MM-Eureka-Dataset](https://huggingface.co/datasets/FanqingM/MM-Eureka-Dataset), 55K;      |
| Rollout Configuration | 128 (prompts + images) * 8 responses; Temperature=1.0;         |
| Reward Function       | Rule-based Rewards (Accuracy-String Match, Format);         |
| Policy Optimization   | PPO Loss                            |
| Benchmark             | +9.2%, +4.7% compared with base model on OlympicBench and L12 respectively; |
| Core Insights         |                                                              |
| Additional Notes      |      |

#### <div id="curr-reft">2025.0310, Curr_ReFT</div>

| Project or Paper      | [Boosting the Generalization and Reasoning of Vision Language Models with Curriculum Reinforcement Learning](https://arxiv.org/pdf/2503.07065) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [ding523/Curr_REFT](https://github.com/ding523/Curr_REFT) |
| Backbone Model        | Qwen2.5-VL-3/7B                                                 |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | [RefCOCO](https://github.com/lichengunc/refer), 3K for training;<br />[Math360K](https://huggingface.co/datasets/Zhiqiang007/MathV360K), [Geo170K](https://huggingface.co/datasets/Luckyjhg/Geo170K), 3K for training;     |
| Rollout Configuration | 1 * 4 responses; Temperature=1.0;         |
| Reward Function       | Difficulty-aware Rule-based Rewards (Accuracy, IoU, Format)；         |
| Policy Optimization   | PPO Loss                            |
| Benchmark             | ID (In-Distribution), compared to base and SFT:<br/>Math (Math360K+Geo170K, 1K for testing): -3B +11.0%, +8.8%, -7B +11.2%, +4.4%;<br/>Detection (RefCOCO, 1K for testing): -3B +58.0%, +14.6%, -7B +51.3%, +2.5%;<br/>Classification: (RefCOCO, 1K for testing) -3B +31.9%, +21.3%, -7B +44.6%, +4.2%;<br/><br/>OOD(Out-of-Distribution), compared to base and SFT: <br/>Math (CLEVER-70K, 0.5K for testing): -3B +55.9%, +42.9%, -7B +46.6%, +21.6%;<br/>Detection (Refgta, 1K for testing): -3B +43.3%, +13.3% -7B +41.7%, +28.3%;<br/>Classification: (Pascal-VOC, 1K for testing) -3B +15.4%, +18.0%, -7B +12.5%, +6.5%; |
| Core Insights         |                                                              |
| Additional Notes      |                                                              |


#### <div id="curr-reft">2025.0311, MMR1</div>

| Project or Paper      | [MMR1: Advancing the Frontiers of Multimodal Reasoning](https://github.com/LengSicong/MMR1) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [LengSicong/MMR1](https://github.com/LengSicong/MMR1) |
| Backbone Model        | Qwen2.5-VL-7B                                                 |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | 6K high-quality samples from public training datasets    |
| Rollout Configuration |          |
| Reward Function       |        |
| Policy Optimization   |                        |
| Benchmark             | Compared to base model: +3.5%, +4.6%, +4.0%, +2.6%, +2.9% on MathVista, MathVision, LogicVista, MathVerse, MathVerse_V;<br />Compared to sft-cot: +16.3%, +6.8%, +17.0%, +21.4%, +24.1% on MathVista, MathVision, LogicVista, MathVerse, MathVerse_V; |
| Core Insights         |                                                              |
| Additional Notes      |                                                              |


#### <div id="metaspatial">2025.0315, MetaSpatial</div>

| Project or Paper      | [MetaSpatial: Reinforcing 3D Spatial Reasoning in VLMs for the Metaverse](https://arxiv.org/abs/2503.18470) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [PzySeere/MetaSpatial](https://github.com/PzySeere/MetaSpatial) |
| Backbone Model        | Qwen2.5-VL-7B                                                 |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | [3D-Reasoning-Dataset](https://huggingface.co/datasets/zhenyupan/3d_layout_reasoning), 50;      |
| Rollout Configuration | 16 (prompts + images) * 4 responses; Temperature=1.0;         |
| Reward Function       | Rule-based Rewards (Format Reward, Physics Reward, Rendering-based Reward);         |
| Policy Optimization   | PPO Loss                            |
| Benchmark             | +74% compared with base model on test-set of 3d-reasoning dataset; |
| Core Insights         |   Injecting physics reward and gpt-4o-based rendering evaluation reward.                                                    |
| Additional Notes      |   


#### <div id="curr-reft">2025.0327, Reason-RFT</div>

| Project or Paper      | [Reason-RFT: Reinforcement Fine-Tuning for Visual Reasoning](https://arxiv.org/pdf/2503.20752) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [tanhuajie/Reason-RFT](https://github.com/tanhuajie/Reason-RFT) |
| Backbone Model        | Qwen2-VL-2/7B                                                 |
| RL Algorithm          | GRPO                                                         |
| Training Dataset      | Visual Counting: [CLEVR-Math](https://huggingface.co/datasets/dali-does/clevr-math), 35K for training,<br />Structure Perception: [Geo170K](https://huggingface.co/datasets/Luckyjhg/Geo170K), 4.5K for training,<br />Spatial Transformation: [TRANCE](https://github.com/hughplay/TVR), 60K for training;     |
| Rollout Configuration | 2 * 8 responses; Temperature=1.0;         |
| Reward Function       | Rule-based Rewards (Accuracy, Format)；         |
| Policy Optimization   | PPO Loss                            |
| Benchmark             | ID (In-Distribution), compared to base and CoT-SFT(stage-1):<br />Visual Counting: -2B +14.40%, +11.30%, -7B -3.00%, +12.30%;<br />Structure Perception: -2B +23.17%, +5.98%, -7B +15.97%, +7.93%;<br />Spatial Transformation: -2B +70.83%, +9.76%, -7B +66.44%, -1.34%;<br/><br/>OOD (Out-of-Distribution), compared to base and CoT-SFT(stage-1):<br/>Visual Counting: -2B +19.20%, +4.70%, -7B +8.90%, +8.60%;<br/>Structure Perception: -2B +12.50%, +7.88%, -7B +5.37%, +16.25%;<br/>Spatial Transformation: -2B +59.45%, +20.86%, -7B +46.64%, +11.46%;|
| Core Insights         |                                                              |
| Additional Notes      |                                                              |


#### <div id="curr-reft">2025.0409, Kimi-VL-Thinking</div>

| Project or Paper      | [KIMI-VL TECHNICAL REPORT](https://github.com/MoonshotAI/Kimi-VL/blob/main/Kimi-VL.pdf) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [MoonshotAI/Kimi-VL](https://github.com/MoonshotAI/Kimi-VL) |
| Backbone Model        | Kimi-VL-A3B                                                |
| RL Algorithm          | Online Policy Mirror Decent/Length Penalty Reward/Curriculum Sampling/Prioritized Sampling/Chain-of-Thought RM/Long2short RL                  |
| Training Dataset      | Long-CoT data about mathematical problem-solving and domain-specific VQA     |
| Rollout Configuration | None        |
| Reward Function       | Correctness, Length；         |
| Policy Optimization   | Online Policy Mirror Decent                     |
| Benchmark             | Comparable with Qwen2.5-VL-32/72B on MathVision (Pass@1)     |
| Core Insights         |                                                              |
| Additional Notes      |                                                              |


#### <div id="curr-reft">2025.0409, VideoChat-R1</div>

| Project or Paper      | [VideoChat-R1: Enhancing Spatio-Temporal Perception via Reinforcement Fine-Tuning](https://arxiv.org/pdf/2504.06958) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [OpenGVLab/VideoChat-R1](https://github.com/OpenGVLab/VideoChat-R1) |
| Backbone Model        | Qwen2.5-VL-7B                                               |
| RL Algorithm          | GRPO    |
| Training Dataset      | Joint training on three tasks: Temporal Grounding: Charade-STA, 5K; Object Tracking: GoT, 10K; Grounding QA: NExTGQA, 3K; total of 18K;   |  
| Rollout Configuration | 1 * 8 responses; Temperature=1.0;       |
| Reward Function       | Rule-based Rewards (Accuracy, Format, IoU)；         |
| Policy Optimization   | PPO Loss                    |
| Benchmark             | mIoU(Overlap on OT) compared with base and SFT:<br />Temporal Grounding: +31.8%, +14.5%;<br />Object Tracking: +31.2%, +2.0%;<br />Grounding QA: +17.0%, +4.2%;     |
| Core Insights         |                                                              |
| Additional Notes      |                                                              |


#### <div id="curr-reft">2025.0410, VL-Rethinker</div>

| Project or Paper      | [VL-Rethinker: Incentivizing Self-Reflection of Vision-Language Models with Reinforcement Learning](https://arxiv.org/pdf/2504.08837) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [TIGER-AI-Lab/VL-Rethinker](https://github.com/TIGER-AI-Lab/VL-Rethinker) |
| Backbone Model        | Qwen2.5-VL-7/72B                                                 |
| RL Algorithm          | GRPO + Selective Sample Replay                                                         |
| Training Dataset      | A 16K query set from Virgo, R1-OneVision, and MM-Eureka;    |
| Rollout Configuration |          |
| Reward Function       |        |
| Policy Optimization   |  PPO loss + KL loss;                      |
| Benchmark             | 7B compared to base model: +4.7%, +6.3%, +2.4% on MathVista, MathVerse, MathVision, +4.4%, +0.7%, +3.1% on MMMU-Pro, MMMU, EMMA,  +2.2% on MEGA;<br />72B compared to base model: +5.5%, +4.5%, +5.5% on MathVista, MathVerse, MathVision, +1.7%, -1.4%, +5.8% on MMMU-Pro, MMMU, EMMA, +2.3% on MEGA; |
| Core Insights         |                                                              |
| Additional Notes      |                                                              |


### Agentic Applications


#### <div id="r1-searcher">2025.0307, R1-Searcher</div>

| Project or Paper      | [R1-Searcher: Incentivizing the Search Capability in LLMs via Reinforcement Learning](https://arxiv.org/pdf/2503.05592) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [RUCAIBox/R1-Searcher](https://github.com/RUCAIBox/R1-Searcher) |
| Backbone Model        |  Qwen-2.5-7B-Base</br>Llama-3.1-8B-Instruct                                             |
| RL Algorithm          | REINFORCE++                                                         |
| Training Dataset      | [RAG-RL-Hotpotqa-with-2wiki](https://huggingface.co/datasets/XXsongLALA/RAG-RL-Hotpotqa-with-2wiki) & [HotpotQA](https://huggingface.co/datasets/BeIR/hotpotqa), 350 for Stage-1 Training, 8k for Stage-2 Training      |
| Rollout Configuration | 64 prompts * 16 responses; Temperature = 1.0;         |
| Reward Function       | Rule-based Rewards (Format Reward for Stage-1 Training and Format Reward and Anser Reward for Stage-2 Training);         |
| Policy Optimization   | REINFORCE++ without KL Penalty                            |
| Benchmark             | HotpotQA, 2WikiMultiHopQA, Musique,  Bamboogle |
| Core Insights         | The proposed R1-Searcher framework integrates RAG with RL, enabling the model to invoke an external search engine during the reasoning process. The framework demonstrates the ability to generalize from in-domain training datasets to out-of-domain test datasets, and can seamlessly switch to online search to obtain up-to-date information.   

#### <div id="AutoCoA">2025.0309, AutoCoA</div>

| Project or Paper      | [Agent Models: Internalizing Chain-of-Action Generation into Reasoning Models](https://arxiv.org/abs/2503.06580) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [ADaM-BJTU/AutoCoA](https://github.com/ADaM-BJTU/AutoCoA)       |
| Backbone Model        | DeepSeek-R1-Distill-Qwen-7B                                   |
| RL Algorithm          | GRPO                                                        |
| Training Dataset      | Synthesized data based on HotpotQA and DeepSeek-R1-Distill-Qwen-32B [data](https://github.com/ADaM-BJTU/AutoCoA/tree/main/data)  |
| Rollout Configuration | 1 prompt * 5 responses; Temperature=0.6;                                                           |
| Reward Function       | Rule-based Rewards (Exact Match and Format Reward)          |
| Policy Optimization   | First through multi-stage SFT (using improved contrastive loss to train CoT+A, CoT+CoA [with/without observation mask]), then combined with an RL stage (GRPO optimization) for end-to-end fine-tuning |
| Benchmark             | Open-domain QA evaluation: single-hop (NQ, TriviaQA) and multi-hop (HotpotQA, 2WikiMultiHopQA, MuSiQue, Bamboogle) |
| Core Insights         | The AutoCoA framework internalizes the decision-making for external tool invocation (Chain-of-Action) into the reasoning model, enabling seamless alternation between thought and action, which significantly improves performance on multi-turn long-horizon tasks. It proposes a two-phase training method: injecting the "when-to-act" and "how-to-act" capabilities via supervised fine-tuning and reinforcement learning, effectively reducing the cost of real interactions and enhancing adaptability in real-world environments. |

#### <div id="search-r1">2024.0312, Search-R1</div>

| Project or Paper      | [Search-R1: Training LLMs to Reason and Leverage Search Engines with Reinforcement Learning](https://arxiv.org/pdf/2503.09516) |
| --------------------- | ------------------------------------------------------------ |
| GitHub                | [PeterGriffinJin/Search-R1](https://github.com/PeterGriffinJin/Search-R1) |
| Backbone Model        | Qwen-2.5-3B (Base/Instruct) and Qwen-2.5-7B (Base/Instruct)                         |
| RL Algorithm          | GRPO and PPO                                                  |
| Training Dataset      | [2018 Wikipedia](https://huggingface.co/datasets/PeterJinGo/wiki-18-corpus)      |
| Rollout Configuration | 64 prompts * 5 responses; Temperature=1.0;         |
| Reward Function       | Rule-based Rewards (Exact Match)         |
| Policy Optimization   | PPO Loss with 0.001 KL coefficient, masking retrived tokens                         |
| Benchmark             | General QA; Multi-Hop QA |
| Core Insights         | SEARCH-R1 addresses the challenges of RL framework and stability, multi-turn interleaved reasoning and search, and reward design, and introduces retrieved token masking to ensure stable optimization.                                |
| Additional Notes      |   

#### <div id="DeepResearcher">2025.0404, DeepResearcher</div>

| Project or Paper      | [DeepResearcher: Scaling Deep Research via Reinforcement Learning in Real-world Environments](https://arxiv.org/abs/2504.03160) |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| GitHub                | [GAIR-NLP/DeepResearcher](https://github.com/GAIR-NLP/DeepResearcher)                                                     |
| Backbone Model        | Qwen2.5-7B-Instruct                                                                                                     |
| RL Algorithm          | GRPO                                               |
| Training Dataset      | [Open-domain QA datasets](https://github.com/GAIR-NLP/DeepResearcher/tree/main/data) (e.g. NQ, TQ, HotpotQA, 2Wiki) – – a total of about 80,000 examples                                           |
| Rollout Configuration | 256 prompts * 16 responses, with a maximum of 10 tool calls per rollout                                                        |
| Reward Function       | Rule-based Rewards(Word-level F1 score and Format Reward)                                                                                       |
| Policy Optimization   | GRPO with masking obvervations                         |
| Benchmark             | In-domain: NaturalQuestions, TriviaQA, HotpotQA, 2WikiMultiHopQA；Out-of-domain: Musique, Bamboogle, PopQA                                             |
| Core Insights         | By training end-to-end with reinforcement learning in a real-world web environment, DeepResearcher can autonomously plan, cross-validate from multiple sources, reflect, and maintain honesty; it significantly improves open-domain QA and deep research capabilities; while also overcoming practical challenges such as search API limitations, web noise, and anti-crawling mechanisms. |

#### <div id="SWiRL">2025.0407, SWiRL</div>

| Project or Paper | [Synthetic Data Generation & Multi-Step RL for Reasoning & Tool Use](https://arxiv.org/abs/2504.04736) |
| ---------------- | ----------------------------------------------------------------------------------------------- |
| **GitHub**       | N/A                                                                                            |
| **Backbone Model** | Gemma 2-27b                                                                                 |
| **RL Algorithm** | Step-Wise Reinforcement Learning (SWiRL)                                                        |
| **Training Dataset** | - HotPotQA: Generated 50,000 synthetic trajectories using 10,000 multi-step questions<br>- GSM8K: Generated 37,500 synthetic trajectories using 7,500 questions |
| **Rollout Configuration** | N/A                                                                                    |
| **Reward Function** | Model-based Rewards (scoring each step’s appropriateness using Gemini 1.5 Pro)               |
| **Policy Optimization** | SWiRL: Stepwise optimization, similar to RLHF in Gemma 2                              |
| **Benchmark**    | HotPotQA; GSM8K; CofCA; MuSiQue; BeerQA                                                           |
| **Core Insights** | 1. Multi-step reasoning can be optimized via step-level rewards, benefiting even if the final answer is incorrect<br>2. Process filtering (selecting based on intermediate step quality) is superior to outcome filtering<br>3. Strong cross-task generalization: for example, training only on HotPotQA can improve GSM8K performance by approximately 16.9% |


## Contributing

If you have any updates or improvements for this document, please feel free to submit a **Pull Request**. Thank you!

#### <div id="template">202x.0x0x, Template</div>

| Project or Paper      | [Project name or Paper title]()                          |
| :-------------------- | :------------------------------------------------------- |
| GitHub                | [Username/Project]()                                     |
| Backbone Model        | (Base / Instruct / Reasoning;  HF Model)                 |
| RL Algorithm          | (PPO / GRPO / RLOO / REINFORCE++; OpenRLHF / Verl / Trl) |
| Training Dataset      | (Size / Source / HF Dataset)                             |
| Rollout Configuration | (Batch Size * N Samples ; Temperature; Dynamic Sampling) |
| Reward Function       | (Outcome; Process; Repetition & Length)                  |
| Policy Optimization   | (KL Loss; Length Penalty; Token-level loss)              |
| Benchmark             | (MATH/GPQA; R1 level; GPT-4o level)                      |
| Core Insights         | (Empirical / Theoretical / Insightful Curves)            |
| Additional Notes      | (e.g., code snippet)                                     |

## Citation

 If you find our repository useful in your research, please star us ⭐ and consider citing:

```tex
@misc{zhang2025TripleR,
  title={Awesome RL Recipes for Reasoning},
  author={Kaiyan Zhang, Yuchen Fan, Yuxin Zuo, Guoli Jia, Kai Tian, Xingtai Lv, Xuekai Zhu, Ermo Hua, Ning Ding, Biqing Qi, Bowen Zhou},
  year={2025},
  howpublished={\url{https://github.com/}},
  note={Github Repository},
}
```

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=TsinghuaC3I/Awesome-RL-Reasoning-Recipes&type=Date)](https://www.star-history.com/#TsinghuaC3I/Awesome-RL-Reasoning-Recipes&Date)
