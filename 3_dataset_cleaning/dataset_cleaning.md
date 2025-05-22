# Dataset Cleaning

After vocal extraction:

### 1. Remove reverb/echo/noise

- Use **UVR5** with the following models to clean vocal tracks:
  - **denoise**
  - **dereverb**
  - **de-eco**
- This step removes reverb, echo, and noise from vocals before training

---

### 2. Truncate silence:
- Threshold: -20 dB
- Duration: 0.5s

---

### 3. Normalize to -5 dB
- Ensure uniform volume across all samples

---

### 4. Convert to mono
Use ffmpeg or Audacity:

```bash
ffmpeg -i input.wav -ac 1 output_mono.wav
