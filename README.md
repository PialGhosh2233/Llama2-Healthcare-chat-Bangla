**Fine tuned Llama2 for Healthcare Q/A for Bangla**

#### Description:
This repository contains the code and configurations for fine-tuning **LLaMA-2-7b-chat** on a Bangla medical Q&A dataset using QLoRA (Quantized LoRA). The fine-tuned model is optimized to assist in generating accurate and context-aware responses for healthcare-related queries in Bangla.

---
#### About the dataset 
Here is the dataset [doctor_qa_bangla](https://huggingface.co/datasets/shetumohanto/doctor_qa_bangla) 

---
#### Features:
- **Model Architecture:** LLaMA-2-7b-chat fine-tuned using LoRA for efficient parameter updates.
- **Low-Rank Adaptation:** LoRA with `r=64`, dropout, and scaled parameters for improved training efficiency.
- **Quantization:** 4-bit precision (nf4 quantization) for reduced memory usage and accelerated training.
- **Training Pipeline:** 
  - Supervised fine-tuning using Hugging Face's `transformers` and `trl` libraries.
  - Customizable training hyperparameters (e.g., learning rate, gradient accumulation, and max sequence length).
- **Text Generation Pipeline:** Seamless inference setup for healthcare-related queries in Bangla.

---

#### Requirements:
- Python 3.8+
- GPUs with CUDA support.
- Libraries: `accelerate`, `peft`, `transformers`, `trl`, `bitsandbytes`, and `datasets`.

---

#### Training Highlights:
- **Efficient Training:** Utilizes QLoRA for memory-efficient fine-tuning on consumer-grade GPUs.
- **Customizable Training:** Easily tweak training settings like batch size, learning rate, and sequence length.

---

#### Applications:
- Bangla-English conversational agents for healthcare.
- Educational tools for bilingual healthcare training.

---

Contributions are welcome to improve the model. 🚀
