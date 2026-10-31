# ICT4403 Assignment 3 — English to Hindi Machine Translation

## Objective
Compare a custom encoder–decoder Transformer, fine-tuned mT5-small, LoRA-adapted LLaMA 3.2 1B, and LoRA-adapted Gemma 2 2B.

## Dataset
IIT Bombay English–Hindi Parallel Corpus: https://huggingface.co/datasets/cfilt/iitb-english-hindi

The notebook inspects the dataset, filters empty/long pairs, removes duplicates, and creates reproducible train/validation/test splits (seed 42). The default subset is capped for Colab resources. Record actual split sizes from your run.

## Running
Open `ICT4403_Assignment3_English_Hindi.ipynb` in Google Colab, select a GPU runtime, and run sequentially. LLaMA/Gemma may require accepting model terms and Hugging Face authentication. Their cells are opt-in and may be run in separate runtimes.

## Evaluation
The notebook measures corpus BLEU, chrF, training/fine-tuning time, inference time and parameter count on common test examples. Compare results while discussing model size, pretraining, tokenization and adaptation differences.

## Results
Commit actual outputs under `results/`: `model_comparison.csv`, `quality_comparison.png`, and `generated_samples.json`. Never invent metrics. Clearly state if a model did not complete.

## Responsible AI
Use observed examples to discuss bias, hallucinations, cultural misrepresentation and sensitive-content errors. Consider human review, targeted evaluation, bias audits, dataset documentation and uncertainty handling.

## Dependencies
See `requirements.txt`; the notebook installs the packages in Colab.
