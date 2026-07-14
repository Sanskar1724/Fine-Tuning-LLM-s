# 📑 Notebook Documentation: Continuous Pre-training (CPT)

### Overview
This notebook demonstrates the end-to-end process of **Domain Adaptation** (CPT) using `SmolLM-135M` and SEC 10-K filings. 

### Pipeline Summary
1.  **Environment Setup**: Utilized `unsloth` for 4-bit quantization and 2x faster training on a Tesla T4 GPU.
2.  **Baseline Evaluation**: Established a baseline perplexity of **19.1** on financial text.
3.  **Data Engineering**: 
    *   Streamed SEC 10-K data from HuggingFace.
    *   Cleaned legal boilerplate and decorative symbols.
    *   Chunked text into 512-token segments with 20% overlap.
4.  **Training Strategy**: 
    *   Applied **LoRA** (Rank 32) to all modules, including `embed_tokens` and `lm_head` to learn new vocabulary.
    *   Used a lower learning rate for embeddings ($2 \times 10^{-5}$) to ensure stability.
5.  **Metrics**: Achieved a **31.2% improvement** in Perplexity (down to ~13.1).
6.  **Observations**: 
    *   **Success**: The model successfully adopted a formal financial 'voice'.
    *   **Catastrophic Forgetting**: The model lost its ability to perform general tasks (e.g., writing poetry), highlighting the need for **Data Mixing** in production.
    *   **Knowledge vs. Behavior**: While the model gained financial knowledge, it remains a completion engine. **SFT** is required to make it an instruction-following assistant.

### Important Resources
*   [Unsloth Documentation](https://github.com/unslothai/unsloth): For optimized LoRA training.
*   [HuggingFace PEFT](https://huggingface.co/docs/peft/index): Deep dive into Parameter-Efficient Fine-Tuning.
*   [SEC EDGAR Data](https://www.sec.gov/edgar/search/): Source of the raw data used in this tutorial.
