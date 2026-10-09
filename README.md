# Hi, I'm Burthcer

Building client-side tools and developer utilities, from local AI systems to browser-based document processing and reference/learning resources.

## Featured Flagship

### [Wisperno](https://github.com/Burthcer/Wisperno): 100% offline, GPU-accelerated push-to-talk dictation

A local alternative to Wispr Flow: `faster-whisper large-v3-turbo` (CTranslate2/CUDA) for speech-to-text, a local quantized LLM (llama.cpp, Qwen2.5/Llama-3.2 GGUF) for cleanup/formatting, all running on-device. No audio or text ever leaves the machine.

- **Zero-cloud by design**: Wispr Flow (the product this takes after) has no offline mode at any pricing tier and sends every word to a cloud subprocessor stack; Wisperno makes zero network calls once models are on disk.
- **Runs inside a strict hardware budget**: four engine presets trade fidelity for footprint, all measured (not estimated) on the actual shipping target (RTX 4070 Laptop, 8GB VRAM):

  | Preset | VRAM | System RAM | Decode Speed |
  |---|---|---|---|
  | **Turbo Flagship (default)** | 3.5 GB | 2.3 GB | 113.8 tok/s |
  | Eco | 3.6 GB | 2.3 GB | 103.3 tok/s |
  | Standard | 3.7 GB | 2.6 GB | 91.7 tok/s |
  | Flagship | 5.1 GB | 3.9 GB | 63.1 tok/s |

- **Real speech, measured, not projected**: a genuine TTS-generated sample transcribed end to end at **RTF 0.097** (~10.3x faster than real-time), came back 100% word-for-word verbatim.
- **Cold start**: Whisper loads in 2.8-5.2s, the local LLM in ~1.1-1.2s.
- Full benchmark methodology, reproducible via the two scripts that ship in the repo, is in [Wisperno's README](https://github.com/Burthcer/Wisperno#measured-performance).

## Skills

**Languages:** TypeScript · JavaScript · Python · HTML/CSS

**Frameworks & Libraries:** Next.js · React · Tailwind CSS · faster-whisper · llama.cpp · PySide6

**AI/Tools:** Claude Code · Git · GitHub CLI · Web Crypto API · PWA/Service Workers

## Other Projects

- **[UniDoc Vault](https://github.com/Burthcer/unidoc-vault)**: Client-side document compression & encryption vault for university admission uploads, built with Next.js, React, and TypeScript.
- **[Python Cheat Sheet Central](https://github.com/Burthcer/Python-Html-Cheat-Sheet)**: Offline-capable, themeable PWA dashboard of Python cheat sheets.
