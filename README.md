# 🧠 Final Project: Developing Your Own Language Model

In this project, you will apply your knowledge of language models in practice and develop your own autoregressive model based on PyTorch. Additionally, you will learn about tools such as Weights & Biases (wandb) and the Hugging Face Model Hub – just like in a real ML workflow.

---

## ✅ Project Requirements

### 1. Model
- Create a **decoder-only language model** using modules from `torch.nn`.
- Use, for example, `nn.TransformerDecoder`, `nn.TransformerDecoderLayer`, etc.
- The model should function autoregressively (like GPT).

### 2. Tokenizer
- Use a tokenizer from the Hugging Face `transformers` library.
- Example: `AutoTokenizer` or `GPT2Tokenizer`.

### 3. Training
- Train your model for at least **3 epochs** (5 recommended).
- Use a small dataset such as **Tiny Shakespeare**, **WikiText-2**, or your own.
- Your model should also be trainable on a CPU (< 1 million parameters).
- Write the entire training loop yourself in PyTorch (do not use `Trainer`).

### 4. Evaluation
- Calculate the loss on a validation dataset after each epoch.
- The loss must **visibly decrease** during training.

### 5. Logging
- Use [wandb](https://wandb.ai) to log training and evaluation loss.

### 6. Publication
- Upload your final model to the [Hugging Face Model Hub](https://huggingface.co/).
- Add a brief model card with a description and tags.

---

## 🌟 Bonus Task
- Load a GPT-2 model and its corresponding tokenizer (`GPT2Tokenizer`) using `from_pretrained`.
- Train it on your dataset using the `Trainer` API.
- Log with wandb and also upload this model to Hugging Face.
