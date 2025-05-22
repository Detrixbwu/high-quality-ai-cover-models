# Traning

```markdown
# Training Your AI Voice Model

## Tools:
- Applio (RVC GUI)
- RVC models with KMeans or FAISS

---

## Pre-training:

- Set model name
- Set sample rate: use 48kHz if you extracted in that
- Disable all effects in preprocessing
- Extract pitch with:
  - `rmvpe`
  - `contentvec`

---

## Index:
- ~1 hour dataset: use **KMeans**
- Less: use **FAISS**

---

## Training Settings:
- Epochs: 500
- Read TensorBoard regularly
- Choose pretrained model (optional)

---

## Result:
After ~500 epochs, your model should be stable and production-ready.
