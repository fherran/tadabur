<div align="center">
  <img src="static/images/tadabur_logo.png" width="120" alt="Tadabur"><br><br>

  # Tadabur

  A large-scale Quran audio dataset featuring ... reciters and word-level alignment — built for Arabic speech research.

  [![Paper](https://img.shields.io/badge/Paper-Read-a27b5c?style=flat-square)](https://arxiv.org/abs/2604.18932)
  [![Dataset](https://img.shields.io/badge/🤗_Dataset-FaisaI%2Ftadabur-c8a97a?style=flat-square)](https://huggingface.co/datasets/FaisaI/tadabur)
  [![Models](https://img.shields.io/badge/🎙_Models-FaisaI-374440?style=flat-square)](https://huggingface.co/FaisaI)
  [![License](https://img.shields.io/badge/License-CC_BY--NC_4.0-e6ddd0?style=flat-square)](https://creativecommons.org/licenses/by-nc/4.0/)

</div>

---

## Overview

Tadabur covers the entire Qur’an with automatic word-level timestamp alignment and structured JSON metadata for each file. It is the largest and most diverse publicly available Qur’anic speech dataset.

| | |
|:---|:---|
| 🕐 Audio | 1400+ hours |
| 🎙️ Reciters | 600+ |
| 🔗 Alignment | Word-level timestamps |

---

## Dataset Structure

Each example contains an audio file and a JSON metadata file:

```json
{
  "reciter_id": 88,
  "surah_id": 3,
  "ayah_id": 82,
  "word_alignments": [
    {
      "word": "أفلا",
      "start": 0.089,
      "end": 0.87
    },
    ...
  ],
  "text_ar_simple": "افلا يتدبرون القران ولو كان من عند غير الله لوجدوا فيه اختلافا كثيرا",
  "text_ar_uthmani": "أَفَلَا يَتَدَبَّرُونَ ٱلْقُرْءَانَ ۚ وَلَوْ كَانَ مِنْ عِندِ غَيْرِ ٱللَّهِ لَوَجَدُوا۟ فِيهِ ٱخْتِلَـٰفًا كَثِيرًا",
  "ayah_duration_s": 10.9,
  "audio_filename": "tadabur_spk0088_S3_A82_db1f8e71_000003.wav"
}
```

---

## Models

Whisper models fine-tuned on Tadabur for Qur'anic ASR, available on HuggingFace:

| Model | Base | Status | Link |
|:---|:---|:---:|:---|
| **Tadabur-Whisper-Small** | Whisper Small | ✅ Available | [🤗 HuggingFace](https://huggingface.co/FaisaI/tadabur-Whisper-Small)|

---

## Citation

```bibtex
@misc{alherran2026tadabur,
  author = {Alherran, Faisal},
  title  = {Tadabur: A Large-Scale Quran Audio Dataset},
  year   = {2026},
  url    = {https://github.com/fherran/tadabur}
}
```

---
## Contact

For questions or collaboration, feel free to reach out on [LinkedIn](https://www.linkedin.com/in/faisal-alherran-caie/).

<div align="center">
  <sub>Released under CC BY-NC 4.0 · For research and educational use only · Please engage with Qur'anic content respectfully.</sub>
</div>
