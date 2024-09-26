# CoT Finetuning: Replicating ChatGPT-01 Logic with LoRA

This repository contains our work on replicating the Chain of Thought (CoT) reasoning capabilities similar to those used in OpenAI's ChatGPT-01 model, utilizing Low-Rank Adaptation (LoRA) for efficient fine-tuning.

## Project Overview

We've focused on fine-tuning two specific models to incorporate CoT reasoning:

1. Llama 3.2 3B Instruct
2. Qwen 2.5 7B

These models were chosen for their potential to effectively implement CoT reasoning while being computationally manageable.

## Repository Contents

- `finetuning-llama3.2-3b.ipynb`: Jupyter notebook for LoRA fine-tuning of the Llama 3.2 3B Instruct model
- `finetuning-qwen2.5-7b.ipynb`: Jupyter notebook for LoRA fine-tuning of the Qwen 2.5 7B model

## Chain of Thought (CoT) Implementation

Our fine-tuning process focuses on replicating key aspects of ChatGPT-01's CoT reasoning:

1. **Problem Decomposition**: Breaking complex tasks into smaller, manageable steps
2. **Sequential Reasoning**: Addressing each step logically and in order
3. **Transparent Thought Process**: Providing clear explanations for each reasoning step
4. **Self-Correction**: Allowing the model to revise its thoughts as it progresses

## Low-Rank Adaptation (LoRA)

We utilize LoRA for fine-tuning our models. LoRA is an efficient fine-tuning technique that offers several advantages:

- **Parameter Efficiency**: LoRA significantly reduces the number of trainable parameters, making fine-tuning more memory-efficient and faster.
- **Preservation of Pre-trained Weights**: The original model weights remain frozen, which helps in maintaining the model's general knowledge while adapting to new tasks.
- **Adaptability**: LoRA adapters can be easily switched or combined, allowing for flexible model customization.
- **Reduced Computational Requirements**: The reduced parameter count allows for fine-tuning on less powerful hardware.

## Fine-tuning Process

The Jupyter notebooks in this repository detail our LoRA-based fine-tuning approach, including:

- Dataset preparation and formatting for CoT tasks
- LoRA configuration (rank, alpha, dropout, etc.)
- Integration of LoRA with the base models
- Training procedures and hyperparameters optimized for CoT learning
- Evaluation metrics focused on reasoning capabilities


## Future Work

- Experiment with different LoRA configurations to optimize CoT performance
- Explore combining LoRA with other efficient fine-tuning techniques
- Develop specific applications leveraging these CoT-enhanced, LoRA-tuned models
- Investigate the transferability of LoRA adapters across different CoT tasks

## Getting Started

To explore our LoRA-based CoT fine-tuning process:

1. Clone this repository
2. Install required dependencies (list to be provided)
3. Open the google colab (`finetuning-llama3.2-3b.ipynb` or `finetuning-qwen2.5-7b.ipynb`)
4. Follow the step-by-step process detailed in each notebook (i will create it soon)

## Contributing

We welcome contributions and suggestions for improving our CoT implementation, LoRA configurations, or extending to other models. Please open an issue or submit a pull request with your ideas.



For questions or further information, please open an issue in this repository.
