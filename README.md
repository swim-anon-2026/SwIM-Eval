# SwIM Evaluation  (Anonymous Submission)

**SwIM (Switch Interval Measure)** is a segmental evaluation metric for multilingual / code-switched ASR.  
It measures transcription fidelity inside **Blended Spans (I)**—a **Contextual Window** around the **Language Alternation Point (LAP)**—to reveal performance degradation that conventional WER can mask.

This repository provides:
- Two runnable notebooks: a **context-window parser** and a **model execution + scoring** harness.
- A lightweight **scorer module** (`src/swim/scorer.py`) implementing WER/WWER/SwIM.
- **Configs** and **manifest schemas** to run on user-provided corpora (no data included).
- A tiny **synthetic demo** that executes end-to-end without external models.

> **Note:** Heavy model initialisation/downloads are intentionally omitted for anonymous review.  
> Commented examples are included for Whisper, wav2vec2, Canary (NeMo), and SeamlessM4T. See `REPRODUCING.md`.

## Quick start (demo)
1. Create a fresh Python 3 environment and install:
   ```bash
   pip install -r requirements.txt

2. Open and run, in order:
 - `notebooks/01_context_window_parser.ipynb`
 - `notebooks/02_model_exec_and_scoring.ipynb`

Demo outputs appear under `results/synthetic/`.

## Using real corpora/models (post-review)

- Obtain corpora from their official distributors and follow their licenses.
- Copy configs/paths.sample.yaml → configs/paths.local.yaml and edit paths.
- Adjust model IDs/parameters in configs/models.yaml.
- See REPRODUCING.md for details.


  
