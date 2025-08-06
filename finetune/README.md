This folder contains ipynb file for fine-tuning Google’s MedGemma language model to improve its performance on Persian medical question-answering tasks.

## Requirements

- Python 3.8+
- Install dependencies:
  ```bash
  pip install -q -U transformers peft trl bitsandbytes scipy datasets huggingface_hub unsloth unsloth_zoo
  ```
- Hugging Face token setup:
  - Use Kaggle Secrets with key \`HF_TOKEN\` or login manually via:
    ```python
    from huggingface_hub import login
    login(token=\"YOUR_HF_TOKEN\")
    ```

## Usage Overview

1. Login to Hugging Face
2. Load and preprocess the \`gaokerena/MF3QA\` Persian medical QA dataset
3. Load MedGemma model and tokenizer with optional UnsloTh optimization
4. Configure LoRA for efficient fine-tuning
5. Set training parameters and start training
6. Save the fine-tuned model and tokenizer for inference

## Notes

- Designed for 4-bit quantized LoRA fine-tuning to reduce resource use
- Ensure appropriate GPU availability for training
