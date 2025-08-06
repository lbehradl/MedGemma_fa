# README for inference folder

# MedGemma Fine-tuned Model Inference

This script demonstrates how to load the fine-tuned MedGemma model for Persian medical QA and perform inference on GPU.

## Features
- Automatically installs required libraries
- Loads tokenizer and base model from Hugging Face
- Applies fine-tuned LoRA adapters
- Sets up a text-generation pipeline for inference
- Runs sample medical question prompts to show model outputs
- Supports Hugging Face login using Kaggle secrets

## Usage
1. Make sure you have your Hugging Face token saved as `HF_TOKEN` in Kaggle Secrets.
2. Upload the fine-tuned model folder (e.g., `farsi-tuned`) under `/kaggle/input/`.
3. Run the script in a Kaggle notebook or any environment with GPU.
4. Use the text generation pipeline to query your own questions.

## Sample questions tested
- چه عصبی در سندروم کارپل تونل به مشکل میخورد؟
- آکرومگالی چیست؟
- علائم اولیه کم‌خونی چیست؟
- چرا تب بالا در کودکان خطرناک است؟
- چگونه می‌توان از ابتلا به هپاتیت B پیشگیری کرد؟
- ارتباط بین میکروبیوم روده و اختلالات روانی چیست؟


## Download fine-tuned model outputs
You can download all output files (adapter config, safetensors, tokenizer files, special tokens, etc.) from Kaggle dataset folder where the model is saved.

https://www.kaggle.com/code/behradkarimi/medgemma-finetune-for-persian-medical-literature
---

# Enjoy using the Persian MedGemma fine-tuned model for medical QA!
