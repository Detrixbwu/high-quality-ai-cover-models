# Training

## Setup

- Set model name
- Select sample rate (e.g., 48kHz if audio extracted at 48k)
- Disable all preprocessing effects

---

## Feature Extraction

- Extract pitch with `rmvpe`
- Extract features with `contentvec`

---

## Indexing Method

- Dataset ~1 hour: use **KMeans**
- Smaller datasets: use **FAISS**

---

## Training Parameters

- Train up to 500 epochs
- Monitor progress with TensorBoard
- Optionally start from a pretrained model

---

## Result

- Model should be stable and ready for production after training
