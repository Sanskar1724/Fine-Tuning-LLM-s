# 🚀 Fine-Tuning Large Language Models (LLMs)

> A complete hands-on learning repository covering the modern fine-tuning pipeline for Large Language Models—from Continued Pre-training (CPT) to Supervised Fine-Tuning (SFT), Direct Preference Optimization (DPO), and Reinforcement Learning with Verifiable Rewards (RLVR) using GRPO.

---

## 📖 About This Repository

This repository documents my journey of learning and implementing modern LLM fine-tuning techniques used in today's AI systems.

Instead of only studying the theory, I implemented every stage practically using open-source models, Hugging Face libraries, PEFT, LoRA, TRL, and reinforcement learning techniques.

The notebooks, documentation, and trained adapters included here demonstrate how modern LLMs evolve from a base model into instruction-following and reasoning models.

---

# 🎯 Learning Objectives

Through this repository, I learned how to:

- Perform Continued Pre-training (CPT)
- Fine-tune models using Supervised Fine-Tuning (SFT)
- Understand Reinforcement Learning from Human Feedback (RLHF)
- Implement Direct Preference Optimization (DPO)
- Train models using Reinforcement Learning with Verifiable Rewards (RLVR)
- Understand Group Relative Policy Optimization (GRPO)
- Design verifiable reward functions
- Fine-tune models efficiently using LoRA
- Analyze reinforcement learning training dynamics
- Evaluate reasoning capabilities after fine-tuning

---

# 📂 Repository Structure

```text
Fine-Tuning/
│
├── Continue Pre-training/
│   ├── CPT.ipynb
│   ├── CPT.md
│   └── LoRA Adapter
│
├── Supervised Fine-tuning/
│   ├── SFT.ipynb
│   └── LoRA Adapter
│
├── RLHF With DPO/
│   ├── Reinforcement Learning with DPO.ipynb
│   ├── Reinforcement Learning.md
│   └── Final Checkpoint
│
├── RLVR with GRPO/
│   ├── RLVR_with_GROP.ipynb
│   ├── Reinforcement Learning with Verified Reward.md
│   └── Training Dynamics
│
└── README.md
```

---

# 📚 Topics Covered

## 1️⃣ Continued Pre-training (CPT)

Learned:

- Domain adaptation
- Continued language modeling
- Financial text adaptation
- Catastrophic forgetting
- Data mixing
- LoRA for CPT

Notebook

- `Continue Pre-training/CPT.ipynb`

---

## 2️⃣ Supervised Fine-Tuning (SFT)

Learned:

- Instruction tuning
- Prompt formatting
- Chat templates
- LoRA Fine-tuning
- PEFT
- Dataset preparation
- Tokenization
- Model evaluation

Notebook

- `Supervised Fine-tuning/SFT.ipynb`

---

## 3️⃣ Reinforcement Learning with DPO

Learned:

- RLHF pipeline
- Preference datasets
- Chosen vs Rejected responses
- Bradley-Terry objective
- DPO loss
- Preference optimization
- LoRA with DPO

Notebook

- `RLHF With DPO/Reinforcement Learning with DPO.ipynb`

---

## 4️⃣ Reinforcement Learning with Verifiable Rewards (RLVR)

Learned:

- RLVR pipeline
- Automatic reward verification
- Reward engineering
- Mathematical reasoning optimization
- GSM8K training
- GRPO algorithm
- Policy optimization
- Reward normalization
- Advantage estimation

Notebook

- `RLVR with GRPO/RLVR_with_GROP.ipynb`

---

# 🛠 Tech Stack

| Category | Tools |
|-----------|-------|
| Language | Python |
| Framework | PyTorch |
| Transformers | Hugging Face Transformers |
| Fine-Tuning | PEFT, LoRA |
| RL Library | TRL |
| Dataset | Hugging Face Datasets |
| Optimization | AdamW |
| Quantization | BitsAndBytes |
| Notebook | Google Colab |
| Visualization | Matplotlib |

---

# 📈 Learning Pipeline

```text
                    Base LLM
                       │
                       ▼
          Continued Pre-training (CPT)
                       │
                       ▼
        Supervised Fine-Tuning (SFT)
                       │
                       ▼
        Preference Optimization (DPO)
                       │
                       ▼
 Reinforcement Learning with Verifiable Rewards
                       │
                       ▼
             Group Relative Policy Optimization
                       │
                       ▼
              Better Reasoning Model
```

---

# 📖 Documentation

Each notebook includes:

- Theory
- Mathematical intuition
- Step-by-step implementation
- Code explanation
- Training process
- Evaluation
- Practical observations
- Research notes

---

# 🎓 Key Concepts Learned

### Fine-Tuning

- Continued Pre-training
- Supervised Fine-Tuning
- Parameter Efficient Fine-Tuning
- LoRA
- PEFT

### Reinforcement Learning

- RLHF
- DPO
- RLVR
- PPO
- GRPO
- Policy Optimization
- Advantage Estimation
- Reward Functions

### Large Language Models

- Tokenization
- Chat Templates
- Prompt Engineering
- Reasoning Models
- Instruction Following
- Alignment

---


# 📚 References

- Hugging Face Transformers
- Hugging Face TRL
- PEFT
- Qwen Models
- OpenAI Research
- DeepSeek-R1
- GSM8K
- DPO Paper
- GRPO Paper

---

# ⭐ Repository Highlights

- ✅ End-to-end LLM Fine-Tuning pipeline
- ✅ Practical implementations
- ✅ Research-style documentation
- ✅ Mathematical explanations
- ✅ Modern alignment techniques
- ✅ LoRA-based efficient training
- ✅ Reinforcement learning experiments
- ✅ Well-documented notebooks

---

## 👨‍💻 Author

**Sanskar**

This repository represents my hands-on learning and practical implementation of modern Large Language Model fine-tuning techniques, covering the complete journey from domain adaptation to reinforcement learning-based alignment.