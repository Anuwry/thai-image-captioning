# Thai Image Captioning

Thai image captioning using Qwen2-VL LoRA fine-tuning and a ViT-WangchanBERTa encoder-decoder.

## Project context

Super AI Engineering Season 6, 2026. Individual competition project.

## Approach

Fine-tuning a 4-bit Qwen2-VL-7B model with Unsloth, LoRA and TRL. A separate notebook explores a ViT encoder with a WangchanBERTa decoder.

## Competition result

Competition leaderboard BLEU score: **20.62000**. This is a BLEU score, not an accuracy percentage.

Leaderboard results are from the project author's competition records, not newly generated benchmark results.

## Source files

- notebooks/qwen2_vl_lora_captioning.ipynb
- notebooks/vit_wangchanberta_captioning.ipynb

## Setup and use

1. Create a Python environment compatible with the historical notebook and selected model.
2. Install relevant dependencies from requirements.txt. GPU frameworks and Unsloth may require platform-specific CUDA instructions.
3. Provide authorized competition images and Thai caption annotations using paths configured in each notebook.
4. Start JupyterLab and run the selected notebook in order. Review experiment branches before a full training run.

    python -m venv .venv
    python -m pip install -r requirements.txt
    python -m jupyterlab

## Archive preparation

- Notebook outputs and execution metadata were cleared.
- Hardcoded credentials found in selected source were replaced with environment lookups.
- Datasets, personal records, submissions, model weights and local environments are excluded.
- Source was statically checked; training and external API calls were not rerun.

## Limitations

Historical experiment notebooks. The alternate encoder-decoder branch and fallback outputs are not claimed to be the final leaderboard model. Training loss is not a caption-quality metric.
