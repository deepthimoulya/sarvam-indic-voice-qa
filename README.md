# Sarvam Multilingual Voice Q&A — Indic Language Demo

A working Colab notebook demonstrating multilingual voice Q&A 
for code-mixed Kannada and other Indian languages using Sarvam APIs.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1mZe4j1c7XVMxvffDlNzYg7mMMGSDo7a6?usp=sharing)

## What this does
- Generates code-mixed Kannada audio using Sarvam TTS (Bulbul v2)
- Transcribes it in 3 modes using Saaras v3: `transcribe`, `translate`, `codemix`
- Shows why code-mixed queries break RAG retrieval — and how to fix it
- Answers questions using sarvam-105b grounded in a knowledge base

## The problem this solves
Real Indian users don't speak in clean formal text. A query like  
*"Nanu hogbekitta but bus late aagide"* spans Kannada and English  
scripts — breaking standard embedding retrieval. This notebook  
demonstrates why `translate` mode is the correct retrieval key  
for Indic voice RAG systems.

## APIs used
- Saaras v3 — Speech to Text (transcribe / translate / codemix modes)
- Bulbul v2 — Text to Speech  
- sarvam-105b — Chat completion

## Setup
1. Get a free API key at [dashboard.sarvam.ai](https://dashboard.sarvam.ai)
2. Add `SARVAM_API_KEY` to Colab Secrets
3. Run all cells

Built by [Deepthi Moulya V M](https://linkedin.com)
