# Vocal Extraction

## If song has backing vocals:
Use **MelBand Karaoke (viperx + aufr33)** with “use as is” (do NOT split into instrum + vocals).

## If it’s just lead vocals:
Use **MelBand Roformer 2024.10** trained by MVSep (@becruily).

---

## Model performance (Latest benchmarks):

| Model                      | Vocals fullness | Vocals bleedless | Vocals SDR | Vocals L1Freq | Instrum fullness | Instrum bleedless | Instrum SDR | Instrum L1Freq |
|----------------------------|-----------------|------------------|------------|---------------|------------------|-------------------|-------------|----------------|
| MelBand Roformer (2024.10) | 16.92           | 37.78            | 11.28      | 39.41         | 27.71            | 47.29             | 17.59       | 40.29          |

---

## Extraction Algorithms comparison:

| Algorithm                         | Lead Vocals (SDR) | Back Vocals (SDR) | Back Vocals + Instrum SDR | Instrum SDR |
|----------------------------------|-------------------|-------------------|---------------------------|-------------|
| MelBand Roformer (@becruily)     | 9.67              | 5.05              | 14.70                     | 15.49       |

---

## General Settings:
- Keep sample rate: 48kHz
- Use full-band models
- Avoid reverb-enhancing models
