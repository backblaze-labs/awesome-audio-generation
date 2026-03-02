# Awesome Audio Generation [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com) [![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

A curated list of AI audio generation APIs, SDKs, and production-ready tools — covering text-to-speech, music generation, and sound design.
Focused on services developers can integrate today.

> Last verified: March 2026

### Related Lists

- [Awesome Video Generation](../awesome-video-generation)
- [Awesome Image Generation](../awesome-image-generation)

---

## Contents

- [Text-to-Speech APIs](#text-to-speech-apis)
- [Music and Sound Generation APIs](#music-and-sound-generation-apis)
- [Open Source TTS Models](#open-source-tts-models)
- [Open Source Music and Audio Models](#open-source-music-and-audio-models)
- [SDKs and Developer Tooling](#sdks-and-developer-tooling)
- [Infrastructure and Deployment](#infrastructure-and-deployment)
- [Evaluation and Observability](#evaluation-and-observability)
- [Templates and Example Projects](#templates-and-example-projects)
- [Learning Resources](#learning-resources)

---

## Text-to-Speech APIs

- **[ElevenLabs](https://elevenlabs.io)** – Industry-leading TTS with voice cloning, multilingual support, and streaming. Flagship `eleven_v3` model. [Docs](https://elevenlabs.io/docs/overview/intro) | SDK: [Python](https://github.com/elevenlabs/elevenlabs-python), JS, Flutter, Swift, Kotlin
- **[OpenAI TTS](https://platform.openai.com/docs/guides/text-to-speech)** – `tts-1`, `tts-1-hd`, and `gpt-4o-mini-tts` models. Also offers Realtime API (WebSocket/WebRTC) for low-latency streaming speech. [API Reference](https://platform.openai.com/docs/api-reference/audio/createSpeech) | SDK: Python, Node
- **[Google Cloud TTS](https://cloud.google.com/text-to-speech)** – 380+ voices across 75+ languages. Chirp 3 HD voices available. [Docs](https://docs.cloud.google.com/text-to-speech/docs) | SDK: Python, Java, Node, Go, Ruby, PHP, C#
- **[Amazon Polly](https://aws.amazon.com/polly)** – Neural TTS with SSML support. Accessible through any AWS SDK. [Docs](https://docs.aws.amazon.com/polly/latest/dg/) | SDK: Python (boto3), Node, Java, .NET, Go, Ruby, PHP
- **[Microsoft Azure Speech](https://azure.microsoft.com/en-us/products/ai-services/ai-speech)** – HD voices GA since March 2025. SSML for fine-grained control. Also includes STT and speaker recognition. [Docs](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/) | SDK: C#, C++, Python, Java, JS, Go, Swift
- **[Resemble AI](https://www.resemble.ai)** – Custom voice cloning specialist. Also publishes open-source Chatterbox TTS model. [Docs](https://docs.resemble.ai) | SDK: [Python](https://github.com/resemble-ai/resemble-python), [Node](https://github.com/resemble-ai/resemble-node)
- **[Play.ht](https://play.ht)** – Streaming TTS with PlayDialog (multi-voice dialogue) and Play3.0-mini (multilingual). [Docs](https://docs.play.ht/reference/api-getting-started) | SDK: [Python](https://github.com/playht/pyht), [Node](https://github.com/playht/text-to-speech-api)
- **[Cartesia](https://cartesia.ai)** – Ultra-low latency Sonic model family. WebSocket multiplexing. [Docs](https://docs.cartesia.ai) | SDK: [Python](https://github.com/cartesia-ai/cartesia-python)
- **[LMNT](https://www.lmnt.com)** – Ultra-low latency TTS. Voice cloning with 5 seconds of audio. [Docs](https://docs.lmnt.com) | SDK: [Python](https://github.com/lmnt-com/lmnt-python), [Node](https://github.com/lmnt-com/lmnt-node)
- **[Hume AI (Octave)](https://www.hume.ai)** – LLM-trained TTS that understands context and emotion. Octave 2 supports 11+ languages. Also includes EVI for voice agents. [Docs](https://dev.hume.ai/docs/text-to-speech-tts/overview) | SDK: Python, TypeScript, .NET
- **[Deepgram](https://deepgram.com)** – Aura TTS model with WebSocket streaming. Also offers Voice Agent API bundling STT + TTS + LLM orchestration. [Docs](https://developers.deepgram.com/docs/text-to-speech) | SDK: Python, JS, .NET, Go
- **[Murf AI](https://murf.ai)** – 150+ voices, 35+ languages, 20 speaking styles. Murf Falcon for low-latency voice agents. [Docs](https://murf.ai/api/docs) | SDK: [Python](https://github.com/murf-ai/murf-python-sdk)
- **[WellSaid Labs](https://www.wellsaid.io)** – Enterprise-focused TTS. Major API upgrade June 2025 with 50% cost reduction. [Docs](https://docs.wellsaidlabs.com/docs/getting-started)

## Music and Sound Generation APIs

- **[Stability AI (Stable Audio)](https://stability.ai/stable-audio)** – Commercial Stable Audio 2.5 model for music and sound generation. Also on Replicate, fal.ai
- **[Beatoven.ai](https://www.beatoven.ai)** – Royalty-free background music from text/mood descriptions. REST API with Python SDK. [API](https://github.com/Beatoven/public-api)
- **[Soundraw](https://soundraw.io)** – Enterprise/B2B royalty-free music generation. Up to 1000 songs/month via API. [API](https://discover.soundraw.io/api)
- **[Suno](https://suno.com)** – Leading music generation (V5 model). No official public API as of early 2026; beta/partner access only.
- **[Udio](https://www.udio.com)** – Music generation with v1.5 and v1.5 Allegro models. Developer portal available; limited public docs.

## Open Source TTS Models

- **[Chatterbox (Resemble AI)](https://github.com/resemble-ai/chatterbox)** – SOTA open-source TTS. Outperformed ElevenLabs in blind tests (63.75% preference). 1M+ HF downloads. Includes Perth neural watermarking. MIT license. [HuggingFace](https://huggingface.co/ResembleAI/chatterbox) | `pip install chatterbox-tts`
- **[Kokoro TTS](https://github.com/hexgrad/kokoro)** – 82M param model, top-ranked on TTS Arena. ~210x real-time on RTX 4090. 8 languages, 26 voices. Apache 2.0. [HuggingFace](https://huggingface.co/hexgrad/Kokoro-82M) | `pip install kokoro`
- **[Coqui TTS / XTTS-v2](https://github.com/idiap/coqui-ai-TTS)** – 17 languages, <200ms streaming latency, zero-shot voice cloning. Company closed Dec 2023; IDIAP maintains fork. [XTTS-v2 Weights](https://huggingface.co/coqui/XTTS-v2) | `pip install coqui-tts`
- **[Fish Speech / FishAudio S1](https://github.com/fishaudio/fish-speech)** – SOTA multilingual TTS with fine-grained emotion control. 13+ languages. Zero-shot voice cloning with 10-30s reference. [HuggingFace](https://huggingface.co/fishaudio/fish-speech-1.5)
- **[F5-TTS](https://github.com/SWivid/F5-TTS)** – Flow-matching zero-shot voice cloning. 335M params, trained on 95k hours. English and Chinese.
- **[StyleTTS2](https://github.com/yl4579/StyleTTS2)** – Style diffusion + adversarial training. Achieves human-level MOS on LJSpeech. Architecture basis for Kokoro. MIT license. [HuggingFace](https://huggingface.co/yl4579/StyleTTS2-LJSpeech)
- **[Bark (Suno)](https://github.com/suno-ai/bark)** – Generative text-to-audio (speech, music, sound effects). GPT-style + EnCodec architecture. MIT license. [HuggingFace](https://huggingface.co/suno/bark)
- **[OpenVoice](https://github.com/myshell-ai/OpenVoice)** – Instant voice cloning by MIT + MyShell. V2 clones tone color across multiple languages. MIT license. [HuggingFace](https://huggingface.co/myshell-ai/OpenVoiceV2)
- **[MeloTTS](https://github.com/myshell-ai/MeloTTS)** – Fast, CPU-capable multilingual TTS. English, Spanish, French, Chinese, Japanese, Korean. MIT license. `pip install melotts`
- **[Piper TTS](https://github.com/OHF-Voice/piper1-gpl)** – Fast local TTS, runs on CPU. ~60MB. ONNX-based, designed for edge/IoT. Original archived; active at OHF-Voice. [Voice Samples](https://rhasspy.github.io/piper-samples/)
- **[Tortoise TTS](https://github.com/neonbjb/tortoise-tts)** – Multi-voice, high-quality TTS with autoregressive + diffusion decoders. Excellent for voice cloning. Apache 2.0. `pip install tortoise-tts`

## Open Source Music and Audio Models

- **[AudioCraft (Meta)](https://github.com/facebookresearch/audiocraft)** – MusicGen (text-to-music), AudioGen (text-to-SFX), EnCodec (neural codec), AudioSeal (watermarking). MIT code license. [Demo](https://audiocraft.metademolab.com) | `pip install audiocraft`
- **[ACE-Step](https://github.com/ace-step/ACE-Step)** – 3.5B param music foundation model. Up to 4 min of music in 20s on A100. 19 languages, all mainstream styles. Apache 2.0. [HuggingFace](https://huggingface.co/ACE-Step/ACE-Step-v1-3.5B)
- **[Stable Audio Open](https://github.com/Stability-AI/stable-audio-tools)** – Open-weight music and sound generation up to 47s (44.1kHz stereo). [HuggingFace](https://huggingface.co/stabilityai/stable-audio-open-1.0)
- **[Riffusion](https://github.com/riffusion/riffusion-hobby)** – Fine-tuned Stable Diffusion generating spectrograms from text, converted to audio. Flask server + Streamlit app included. [HuggingFace](https://huggingface.co/riffusion/riffusion-model-v1)
- **[Mustango](https://github.com/AMAAI-Lab/mustango)** – Text-to-music with controllable chords, beats, tempo, and key. LDM + Flan-T5. Apache 2.0. [Demo](https://amaai-lab.github.io/mustango/)

## SDKs and Developer Tooling

### Audio Processing

- **[FFmpeg](https://ffmpeg.org)** – Universal audio/video processing CLI. Backend for PyDub and many TTS pipelines. Python: [ffmpeg-python](https://github.com/kkroening/ffmpeg-python) | Node: fluent-ffmpeg
- **[PyDub](https://github.com/jiaaro/pydub)** – High-level Python audio manipulation. Slicing, concatenating, normalizing, format conversion. `pip install pydub`
- **[librosa](https://github.com/librosa/librosa)** – Python audio analysis. Spectrograms, MFCCs, beat tracking, pitch analysis. [Docs](https://librosa.org/doc/latest/) | `pip install librosa`
- **[Pedalboard (Spotify)](https://github.com/spotify/pedalboard)** – Python library wrapping JUCE for audio effects, VST/AU plugin loading, audio I/O. `pip install pedalboard`
- **[Torchaudio](https://github.com/pytorch/audio)** – PyTorch's official audio library. I/O, feature extraction, transforms, pretrained models. [Docs](https://pytorch.org/audio/) | `pip install torchaudio`
- **[soundfile](https://github.com/bastibe/python-soundfile)** – Reads and writes WAV, FLAC, OGG via libsndfile. Pairs with NumPy/librosa. `pip install soundfile`

### Voice Agent Frameworks

- **[Pipecat (Daily)](https://github.com/pipecat-ai/pipecat)** – Open-source Python framework for STT → LLM → TTS voice agent pipelines. Modular adapters for ElevenLabs, Cartesia, Deepgram, OpenAI, and more. BSD 2-Clause. [Docs](https://docs.pipecat.ai) | `pip install pipecat-ai`
- **[LiveKit Agents](https://github.com/livekit/agents)** – Open-source framework for real-time voice AI agents with semantic turn detection. [Docs](https://docs.livekit.io) | SDKs: JS, Python, Swift, Android, Flutter, Go, Rust
- **[Vapi](https://vapi.ai)** – Managed voice AI agent platform. Abstracts STT/LLM/TTS orchestration. Integrates ElevenLabs, Deepgram, OpenAI, Anthropic. [Docs](https://docs.vapi.ai) | SDK: JS, Python, Java, Swift

## Infrastructure and Deployment

### Real-Time Audio Infrastructure

- **[LiveKit](https://livekit.io)** – Open-source WebRTC SFU (Go). Managed cloud available. Foundation for voice AI agents. [GitHub](https://github.com/livekit/livekit) | [Docs](https://docs.livekit.io)
- **[Daily](https://www.daily.co)** – WebRTC audio/video API. Creator of Pipecat. Supports OpenAI Audio Models natively. [Docs](https://docs.daily.co)
- **[OpenAI Realtime API](https://platform.openai.com/docs/guides/realtime)** – Native speech-to-speech with GPT-4o. WebSocket and WebRTC. Audio streamed as base64 PCM chunks.

### GPU Cloud Providers

- **[RunPod](https://www.runpod.io)** – GPU pods and serverless endpoints. REST, GraphQL, and CLI. [Docs](https://docs.runpod.io)
- **[Modal](https://modal.com)** – Serverless Python-first GPU platform. Sub-second cold starts. [Docs](https://modal.com/docs/guide)
- **[Replicate](https://replicate.com)** – Serverless model hosting for open-source audio models. [Docs](https://replicate.com/docs)
- **[fal.ai](https://fal.ai)** – Serverless inference for generative media. [Docs](https://docs.fal.ai)

## Evaluation and Observability

- **[TTS Arena (HuggingFace)](https://huggingface.co/spaces/TTS-AGI/TTS-Arena-V2)** – Community blind pairwise voting with Elo-style ranking. The most referenced human-preference benchmark for TTS. [Blog](https://huggingface.co/blog/arena-tts)
- **[Speech Arena (Artificial Analysis)](https://huggingface.co/spaces/ArtificialAnalysis/Speech-Arena-Leaderboard)** – Broader speech model leaderboard including latency, cost, and quality dimensions.
- **[UTMOS](https://github.com/sarulab-speech/UTMOS22)** – MOS prediction system from UTokyo-Sarulab. Predicts Mean Opinion Score without human listeners. Pearson correlation ~0.82. [Paper](https://arxiv.org/abs/2204.02152)
- **[DNSMOS (Microsoft)](https://github.com/microsoft/DNS-Challenge)** – Deep Noise Suppression MOS. Non-intrusive perceptual quality metric for speech enhancement. P.835 framework. Also in `torchmetrics`
- **WER (Word Error Rate)** – Standard intelligibility metric. Run synthesized speech through Whisper ASR and measure transcription error rate.

## Templates and Example Projects

- **[Kokoro Web](https://github.com/eduardolat/kokoro-web)** – Self-hosted, OpenAI API-compatible TTS server using Kokoro-82M. Drop-in replacement for OpenAI TTS endpoint.
- **[Stable Audio Open Demo](https://github.com/Stability-AI/stable-audio-open-demo)** – Official Stability AI demo notebook for Stable Audio Open 1.0.
- **[Real-Time Voice Cloning](https://github.com/CorentinJ/Real-Time-Voice-Cloning)** – Classic SV2TTS demo. Clone a voice in 5 seconds. ~55k stars.
- **[LiveKit Agent Examples](https://github.com/livekit-examples/)** – Official examples for building voice/video AI agents.
- **[B2 Whisper Transcriber](https://github.com/backblaze-b2-samples/b2-whisper-transformersjs-transcriber)** – Audio transcription app using Whisper and Transformers.js with Backblaze B2 cloud storage.
- **[ACE-Step Demo](https://ace-step.github.io/)** – Official music generation samples and comparisons.

## Learning Resources

- [ElevenLabs API Documentation](https://elevenlabs.io/docs/overview/intro)
- [OpenAI TTS Guide](https://platform.openai.com/docs/guides/text-to-speech)
- [OpenAI Realtime API Guide](https://platform.openai.com/docs/guides/realtime)
- [Pipecat Documentation](https://docs.pipecat.ai)
- [LiveKit Voice AI Agent Docs](https://docs.livekit.io)
- [AudioCraft Documentation](https://github.com/facebookresearch/audiocraft)

---

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first. PRs for new tools, corrections, and updates are appreciated.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
