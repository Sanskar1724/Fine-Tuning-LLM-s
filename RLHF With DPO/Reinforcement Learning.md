# Reinforcement Learning from Human Feedback (RLHF) with Direct Preference Optimization (DPO)

## Overview

This notebook provides a practical introduction to **Reinforcement Learning from Human Feedback (RLHF)** and its modern alternative, **Direct Preference Optimization (DPO)**.

Instead of focusing only on theory, this notebook builds the complete DPO pipeline step by step using a lightweight language model, LoRA, and a human preference dataset. The goal is to understand how modern LLMs are aligned to produce responses that better match human preferences.

---

# What You'll Learn

After completing this notebook, you will understand:

- Why Supervised Fine-Tuning (SFT) is not enough
- The complete RLHF pipeline
- Human preference datasets
- Reward Models
- PPO optimization
- Why DPO was introduced
- How DPO simplifies RLHF
- How to train an LLM using DPO
- How to evaluate a DPO model
- The limitations of DPO

---

# Prerequisites

Before starting this notebook, you should be familiar with:

- Python
- PyTorch
- Hugging Face Transformers
- LoRA / PEFT
- Supervised Fine-Tuning (SFT)

---

# Notebook Structure

## Part 0 — Setup

- Install dependencies
- Import libraries
- Configure environment

---

## Part 1 — Meet the Base Model

- Load an instruction model
- Generate responses
- Understand the baseline

---

## Part 2 — Understanding RLHF

- Why RLHF?
- Human Feedback
- Reward Model
- PPO
- RLHF Pipeline

---

## Part 3 — Understanding DPO

- Why DPO?
- RLHF vs DPO
- Preference Optimization
- DPO Loss

---

## Part 4 — Preference Dataset

- UltraFeedback Dataset
- Prompt
- Chosen Response
- Rejected Response
- Dataset preprocessing

---

## Part 5 — DPO Training

- Apply LoRA
- Configure DPOTrainer
- Training configuration
- Hyperparameters
- Model optimization

---

## Part 6 — Model Evaluation

- Compare Base vs DPO
- Test prompts
- Analyze improvements
- Training metrics

---

## Part 7 — Experiments

- Different training steps
- Different dataset sizes
- Learning rate experiments
- LoRA configuration

---

## Part 8 — Save & Load

- Save adapters
- Reload adapters
- Run inference

---

## Part 9 — Key Takeaways

- RLHF summary
- DPO summary
- Advantages
- Limitations
- Next learning steps

---

# Technologies Used

- Python
- PyTorch
- Hugging Face Transformers
- TRL
- PEFT (LoRA)
- Datasets
- Google Colab
- CUDA

---

# Learning Outcomes

By the end of this notebook, you will be able to:

- Explain the complete RLHF workflow.
- Understand the motivation behind DPO.
- Train a language model using human preference data.
- Analyze DPO training metrics.
- Compare a Base Model with a DPO-aligned model.
- Build your own DPO training pipeline.

---

# RLHF Pipeline

```text
Pretrained Model
        │
        ▼
Supervised Fine-Tuning (SFT)
        │
        ▼
Preference Dataset
        │
        ▼
Reward Model
        │
        ▼
PPO
        │
        ▼
Aligned Model
```

---

# DPO Pipeline

```text
Pretrained Model
        │
        ▼
Supervised Fine-Tuning (SFT)
        │
        ▼
Preference Dataset
        │
        ▼
Direct Preference Optimization (DPO)
        │
        ▼
Aligned Model
```

---

This notebook is designed for students and beginners who want to understand modern LLM alignment through practical implementation. All examples are compatible with **Google Colab (Free T4 GPU)** and use efficient fine-tuning techniques such as **LoRA** to keep training lightweight and accessible.