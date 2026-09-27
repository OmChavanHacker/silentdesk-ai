# SilentDesk AI

An early prototype for local meeting-intelligence workflows.

## Current prototype behavior

- Applies a basic amplitude threshold to synthetic audio data.
- Redacts configured terms from a supplied transcript.
- Computes an in-memory SHA-256 hash chain for redacted transcript events.

This scaffold does not load speech, embedding, or language models; execute workloads on an NPU; enforce network isolation; or persist its audit ledger. The timing and audio are demonstration values, not performance measurements or production security guarantees.

## Quick start

Run these commands from the project directory in PowerShell:

```powershell
pip install -r requirements.txt
python main.py
```

Edit `vault/nda_terms.txt` to configure the terms used by the demo redactor.
