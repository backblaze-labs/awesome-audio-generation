# Awesome Audio Generation [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com) [![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

A curated list of AI audio generation APIs, SDKs, and production-ready tools — covering text-to-speech, music generation, and sound design. Focused on services developers can integrate today.

Maintained by [Backblaze](https://www.backblaze.com).

### Related Lists

- [Awesome Image Generation](https://github.com/backblaze-labs/awesome-image-generation)
- [Awesome Video Generation](https://github.com/backblaze-labs/awesome-video-generation)
- [Awesome ML Data Pipelines](https://github.com/backblaze-labs/awesome-ml-data-pipelines)
- [Awesome Multimodal Data](https://github.com/backblaze-labs/awesome-multimodal-data)
- [Awesome Agent Infrastructure](https://github.com/backblaze-labs/awesome-agent-infrastructure)
- [Awesome Physical AI](https://github.com/backblaze-labs/awesome-physical-ai)

## Contents

- [Text-to-Speech APIs](#text-to-speech-apis)
- [Music and Sound Generation APIs](#music-and-sound-generation-apis)
- [Open Source TTS Models](#open-source-tts-models)
- [Open Source Music and Audio Models](#open-source-music-and-audio-models)
- [Audio Processing](#audio-processing)
- [Voice Agent Frameworks](#voice-agent-frameworks)
- [Real-Time Audio Infrastructure](#real-time-audio-infrastructure)
- [GPU Cloud Providers](#gpu-cloud-providers)
- [Evaluation and Observability](#evaluation-and-observability)
- [Templates and Example Projects](#templates-and-example-projects)

---

## Text-to-Speech APIs

> Commercial TTS APIs with hosted inference and developer SDKs.

- **[Amazon Polly](https://aws.amazon.com/polly)** – Neural TTS with SSML support, accessible through any AWS SDK. [Docs](https://docs.aws.amazon.com/polly/latest/dg/) | SDK: Python (boto3), Node, Java, .NET, Go, Ruby, PHP
- **[Cartesia](https://cartesia.ai)** – Ultra-low latency Sonic model family with WebSocket multiplexing. [Docs](https://docs.cartesia.ai) | SDK: [Python](https://github.com/cartesia-ai/cartesia-python)
- **[Deepgram](https://deepgram.com)** – Aura TTS model with WebSocket streaming. Also offers a Voice Agent API bundling STT + TTS + LLM orchestration. [Docs](https://developers.deepgram.com/docs/text-to-speech) | SDK: Python, JavaScript, .NET, Go
- **[ElevenLabs](https://elevenlabs.io)** – Industry-leading TTS with voice cloning, multilingual support, and streaming. Flagship eleven_v3 model. [Docs](https://elevenlabs.io/docs/overview/intro) | SDK: [Python](https://github.com/elevenlabs/elevenlabs-python), JavaScript, Flutter, Swift, Kotlin
- **[Google Cloud TTS](https://cloud.google.com/text-to-speech)** – 380+ voices across 75+ languages. Chirp 3 HD voices available. [Docs](https://docs.cloud.google.com/text-to-speech/docs) | SDK: Python, Java, Node, Go, Ruby, PHP, C#
- **[Hume AI (Octave)](https://www.hume.ai)** – LLM-trained TTS that understands context and emotion. Octave 2 supports 11+ languages. Also includes EVI for voice agents. [Docs](https://dev.hume.ai/docs/text-to-speech-tts/overview) | SDK: Python, TypeScript, .NET
- **[Inworld TTS](https://inworld.ai/tts-api)** – Commercial TTS API ranked. [Docs](https://docs.inworld.ai/tts/tts)
- **[LMNT](https://www.lmnt.com)** – Ultra-low latency TTS. Voice cloning with 5 seconds of audio. [Docs](https://docs.lmnt.com) | SDK: [Python](https://github.com/lmnt-com/lmnt-python), [Node](https://github.com/lmnt-com/lmnt-node)
- **[Microsoft Azure Speech](https://azure.microsoft.com/en-us/products/ai-services/ai-speech)** – HD voices GA since March 2025. SSML for fine-grained control. Also includes STT and speaker recognition. [Docs](https://learn.microsoft.com/en-us/azure/ai-services/speech-service/) | SDK: C#, C++, Python, Java, JavaScript, Go, Swift
- **[Murf AI](https://murf.ai)** – 150+ voices, 35+ languages, 20 speaking styles. Murf Falcon for low-latency voice agents. [Docs](https://murf.ai/api/docs) | SDK: [Python](https://github.com/murf-ai/murf-python-sdk)
- **[OpenAI TTS](https://platform.openai.com/docs/guides/text-to-speech)** – tts-1, tts-1-hd, and gpt-4o-mini-tts models plus a Realtime API (WebSocket/WebRTC) for low-latency streaming speech. [Docs](https://platform.openai.com/docs/api-reference/audio/createSpeech) | SDK: Python, Node
- **[Play.ht](https://play.ht)** – Streaming TTS with PlayDialog (multi-voice dialogue) and Play3.0-mini (multilingual). [Docs](https://docs.play.ht/reference/api-getting-started) | SDK: [Python](https://github.com/playht/pyht), [Node](https://github.com/playht/text-to-speech-api)
- **[Resemble AI](https://www.resemble.ai)** – Custom voice cloning specialist. Also publishes the open-source Chatterbox TTS model. [Docs](https://docs.resemble.ai) | SDK: [Python](https://github.com/resemble-ai/resemble-python), [Node](https://github.com/resemble-ai/resemble-node)
- **[WellSaid Labs](https://www.wellsaid.io)** – Enterprise-focused TTS. Major API upgrade June 2025 with 50% cost reduction. [Docs](https://docs.wellsaidlabs.com/docs/getting-started)

## Music and Sound Generation APIs

> Hosted APIs for music, background audio, and sound-effect generation.

- **[Beatoven.ai](https://www.beatoven.ai)** – Royalty-free background music from text/mood descriptions. REST API with Python SDK. [Docs](https://github.com/Beatoven/public-api) | SDK: Python
- **[Soundraw](https://soundraw.io)** – Enterprise/B2B royalty-free music generation. Up to 1000 songs/month via API. [Docs](https://discover.soundraw.io/api)
- **[Stability AI (Stable Audio)](https://stability.ai/stable-audio)** – Commercial Stable Audio 2.5 model for music and sound generation. Also available on Replicate and fal.ai.
- **[Suno](https://suno.com)** – Leading music generation (V5 model). No official public API as of early 2026; beta/partner access only.
- **[Udio](https://www.udio.com)** – Music generation with v1.5 and v1.5 Allegro models. Developer portal available; limited public docs.

## Open Source TTS Models

> Open-weight speech-synthesis models you can run locally or self-host.

- **[Bark (Suno)](https://github.com/suno-ai/bark)** – Generative text-to-audio (speech, music, sound effects). GPT-style + EnCodec architecture. [Docs](https://huggingface.co/suno/bark)
- **[OpenVoice](https://github.com/myshell-ai/OpenVoice)** – Instant voice cloning by MIT + MyShell. V2 clones tone color across multiple languages. [Docs](https://huggingface.co/myshell-ai/OpenVoiceV2)
- **[Fish Speech / FishAudio S1](https://github.com/fishaudio/fish-speech)** – SOTA multilingual TTS with fine-grained emotion control. 13+ languages. Zero-shot voice cloning with 10-30s reference. [Docs](https://huggingface.co/fishaudio/fish-speech-1.5)
- **[Chatterbox (Resemble AI)](https://github.com/resemble-ai/chatterbox)** – SOTA open-source TTS. Outperformed ElevenLabs in blind tests (63.75% preference). 1M+ HF downloads. Includes Perth neural watermarking. [Docs](https://huggingface.co/ResembleAI/chatterbox) | SDK: Python (pip install chatterbox-tts)
- **[Tortoise TTS](https://github.com/neonbjb/tortoise-tts)** – Multi-voice, high-quality TTS with autoregressive + diffusion decoders. Excellent for voice cloning. SDK: Python (pip install tortoise-tts)
- **[F5-TTS](https://github.com/SWivid/F5-TTS)** – Flow-matching zero-shot voice cloning. 335M params, trained on 95k hours. English and Chinese.
- **[MeloTTS](https://github.com/myshell-ai/MeloTTS)** – Fast, CPU-capable multilingual TTS. English, Spanish, French, Chinese, Japanese, Korean. SDK: Python (pip install melotts)
- **[Kokoro TTS](https://github.com/hexgrad/kokoro)** – 82M param model, top-ranked on TTS Arena. ~210x real-time on RTX 4090. 8 languages, 26 voices. [Docs](https://huggingface.co/hexgrad/Kokoro-82M) | SDK: Python (pip install kokoro)
- **[StyleTTS2](https://github.com/yl4579/StyleTTS2)** – Style diffusion + adversarial training. Achieves human-level MOS on LJSpeech. Architecture basis for Kokoro. [Docs](https://huggingface.co/yl4579/StyleTTS2-LJSpeech)
- **[Piper TTS](https://github.com/OHF-Voice/piper1-gpl)** – Fast local TTS that runs on CPU. ~60MB ONNX-based, designed for edge/IoT. Original repo archived; active at OHF-Voice. [Docs](https://rhasspy.github.io/piper-samples/)
- **[Coqui TTS / XTTS-v2](https://github.com/idiap/coqui-ai-TTS)** – 17 languages, <200ms streaming latency, zero-shot voice cloning. Company closed Dec 2023; IDIAP maintains the fork. [Docs](https://huggingface.co/coqui/XTTS-v2) | SDK: Python (pip install coqui-tts)
- **[CosyVoice (FunAudioLLM)](https://github.com/FunAudioLLM/CosyVoice)** – Alibaba/FunAudioLLM multilingual TTS. CosyVoice2 streaming at 150ms latency; CosyVoice3 (Dec 2025) adds RL-tuned voice quality. 9+ languages, zero-shot cloning. [Docs](https://huggingface.co/FunAudioLLM/CosyVoice2-0.5B) | SDK: Python (pip install -r requirements.txt)
- **[Dia (Nari Labs)](https://github.com/nari-labs/dia)** – 1.6B-param dialogue TTS. Generates multi-speaker audio with nonverbal cues (laughter, sighs) in one pass. Voice cloning via audio prompt. Apache-2.0. [Docs](https://huggingface.co/nari-labs/Dia-1.6B) | SDK: Python (pip install git+https://github.com/nari-labs/dia.git)
- **[IndexTTS](https://github.com/index-tts/index-tts)** – Zero-shot TTS with duration control and emotion-timbre disentanglement. IndexTTS-2 adds multilingual support (Chinese, English, Japanese, Spanish). Bilibili model license. [Docs](https://index-tts.github.io/)
- **[Qwen3-TTS](https://github.com/QwenLM/Qwen3-TTS)** – Alibaba Cloud open-source TTS series (0.6B–1.7B). Voice cloning from 3s reference, free-form voice design, 97ms streaming latency. 10 languages. [Docs](https://huggingface.co/collections/Qwen/qwen3-tts) | SDK: Python (pip install qwen-tts)
- **[VoxCPM2 (OpenBMB)](https://github.com/OpenBMB/VoxCPM)** – 2B tokenizer-free diffusion-AR TTS. Voice Design (voice from text description), controllable cloning, 30 languages, 48kHz stereo. Streaming API support. [Docs](https://huggingface.co/openbmb/VoxCPM2-2B) | SDK: Python (pip install voxcpm)
- **[Voxtral TTS (Mistral)](https://huggingface.co/mistralai/Voxtral-4B-TTS-2603)** – 4B open-weight TTS from Mistral. 9 languages, 20 preset voices, 24 kHz output. Deployable via vLLM-Omni; also available as hosted API at console.mistral.ai. [Docs](https://docs.mistral.ai/capabilities/audio/text_to_speech)

## Open Source Music and Audio Models

> Open-weight models for music, soundscapes, and general audio generation.

- **[AudioCraft (Meta)](https://github.com/facebookresearch/audiocraft)** – MusicGen (text-to-music), AudioGen (text-to-SFX), EnCodec (neural codec), AudioSeal (watermarking). [Docs](https://audiocraft.metademolab.com) | SDK: Python (pip install audiocraft)
- **[ACE-Step](https://github.com/ace-step/ACE-Step)** – 3.5B param music foundation model. Up to 4 min of music in 20s on A100. 19 languages, all mainstream styles. [Docs](https://huggingface.co/ACE-Step/ACE-Step-v1-3.5B)
- **[Riffusion](https://github.com/riffusion/riffusion-hobby)** – Fine-tuned Stable Diffusion generating spectrograms from text, converted to audio. Flask server + Streamlit app included. [Docs](https://huggingface.co/riffusion/riffusion-model-v1)
- **[Stable Audio Open](https://github.com/Stability-AI/stable-audio-tools)** – Open-weight music and sound generation up to 47s (44.1kHz stereo). [Docs](https://huggingface.co/stabilityai/stable-audio-open-1.0)
- **[Mustango](https://github.com/AMAAI-Lab/mustango)** – Text-to-music with controllable chords, beats, tempo, and key. LDM + Flan-T5. [Docs](https://amaai-lab.github.io/mustango/)
- **[ACE-Step 1.5](https://github.com/ace-step/ACE-Step-1.5)** – Music generation model combining LM planning + Diffusion Transformer synthesis. Full songs in <2s on A100, <10s on RTX 3090. XL variant (4B DiT) released April 2026. SDK: Python (pip install acestep)
- **[Amphion](https://github.com/open-mmlab/Amphion)** – OpenMMLab toolkit for TTS, voice conversion, singing voice conversion, and text-to-audio. Includes Vevo2 (speech + singing) and DualCodec neural codec.
- **[HeartMuLa (heartlib)](https://github.com/HeartMuLa/heartlib)** – 3B open-source music LM conditioned on lyrics, style tags, and reference audio. Includes HeartCodec (12.5Hz music codec), HeartCLAP (audio-text alignment), and HeartTranscriptor (lyrics ASR). [Docs](https://heartmula.github.io/) | SDK: Python (pip install -e .)
- **[InspireMusic (FunAudioLLM)](https://github.com/FunAudioLLM/InspireMusic)** – Alibaba toolkit for text-to-music, music continuation, and audio super-resolution. Autoregressive transformer + flow-matching model generates 48kHz music from text and audio prompts. [Docs](https://funaudiollm.github.io/inspiremusic/)
- **[SongGeneration (Tencent / LeVo)](https://github.com/tencent-ailab/SongGeneration)** – 4B-param open-source song generation model producing vocals + accompaniment from lyrics and style prompts. LeVo-v2-large released March 2026. Non-commercial license. [Docs](https://huggingface.co/tencent/LeVo-v2-large)
- **[TangoFlux](https://github.com/declare-lab/TangoFlux)** – Flow-matching DiT model for text-to-audio and sound-effects generation. 44.1kHz stereo, up to 30s, generated in ~3s on one A40. Research use only (Stability AI Community License). [Docs](https://huggingface.co/declare-lab/TangoFlux)
- **[YuE (M-A-P)](https://github.com/multimodal-art-projection/YuE)** – Open-source LLaMA2-based foundation model for full-song generation. Converts lyrics to vocals + accompaniment across diverse genres and languages. Supports LoRA fine-tuning and in-context style transfer. [Docs](https://map-yue.github.io/)

## Audio Processing

> Libraries and CLIs for manipulating, analysing, and encoding audio.

- **[PyDub](https://github.com/jiaaro/pydub)** – High-level Python audio manipulation. Slicing, concatenating, normalizing, format conversion. SDK: Python (pip install pydub)
- **[librosa](https://github.com/librosa/librosa)** – Python audio analysis. Spectrograms, MFCCs, beat tracking, pitch analysis. [Docs](https://librosa.org/doc/latest/) | SDK: Python (pip install librosa)
- **[Pedalboard (Spotify)](https://github.com/spotify/pedalboard)** – Python library wrapping JUCE for audio effects, VST/AU plugin loading, audio I/O. SDK: Python (pip install pedalboard)
- **[Torchaudio](https://github.com/pytorch/audio)** – PyTorch's official audio library. I/O, feature extraction, transforms, pretrained models. [Docs](https://pytorch.org/audio/) | SDK: Python (pip install torchaudio)
- **[soundfile](https://github.com/bastibe/python-soundfile)** – Reads and writes WAV, FLAC, OGG via libsndfile. Pairs with NumPy/librosa. SDK: Python (pip install soundfile)
- **[BigVGAN (NVIDIA)](https://github.com/NVIDIA/BigVGAN)** – Universal neural vocoder converting mel spectrograms to waveforms. 112M-param model with HuggingFace Hub integration. Generalizes zero-shot to speech, music, and instruments at up to 44kHz. [Docs](https://nv-adlr.github.io/projects/bigvgan/)
- **[ClearerVoice-Studio](https://github.com/modelscope/ClearerVoice-Studio)** – ModelScope toolkit for speech enhancement, separation, super-resolution, and target speaker extraction. Includes SpeechScore quality metrics (PESQ, STOI, DNSMOS). SDK: Python (pip install clearvoice)
- **[FFmpeg](https://ffmpeg.org)** – Universal audio/video processing CLI. Backend for PyDub and many TTS pipelines. SDK: [Python (ffmpeg-python)](https://github.com/kkroening/ffmpeg-python), Node (fluent-ffmpeg)
- **[LALAL.AI](https://www.lalal.ai)** – Commercial API for AI-powered stem separation (vocals, drums, bass, guitar, strings) and voice cloning. API v1 released Feb 2026 with OpenAPI spec and Python code examples. [Docs](https://www.lalal.ai/api/v1/docs/)

## Voice Agent Frameworks

> Frameworks for building real-time STT → LLM → TTS voice agents.

- **[Pipecat (Daily)](https://github.com/pipecat-ai/pipecat)** – Open-source Python framework for STT → LLM → TTS voice agent pipelines. Modular adapters for ElevenLabs, Cartesia, Deepgram, OpenAI, and more. [Docs](https://docs.pipecat.ai) | SDK: Python (pip install pipecat-ai)
- **[LiveKit Agents](https://github.com/livekit/agents)** – Open-source framework for real-time voice AI agents with semantic turn detection. [Docs](https://docs.livekit.io) | SDK: JavaScript, Python, Swift, Android, Flutter, Go, Rust
- **[Vapi](https://vapi.ai)** – Managed voice AI agent platform. Abstracts STT/LLM/TTS orchestration. Integrates ElevenLabs, Deepgram, OpenAI, Anthropic. [Docs](https://docs.vapi.ai) | SDK: JavaScript, Python, Java, Swift

## Real-Time Audio Infrastructure

> WebRTC, streaming, and low-latency audio transport platforms.

- **[LiveKit](https://livekit.io)** – Open-source WebRTC SFU (Go). Managed cloud available. Foundation for voice AI agents. [Docs](https://docs.livekit.io)
- **[Daily](https://www.daily.co)** – WebRTC audio/video API. Creator of Pipecat. Supports OpenAI Audio Models natively. [Docs](https://docs.daily.co)
- **[OpenAI Realtime API](https://platform.openai.com/docs/guides/realtime)** – Native speech-to-speech with GPT-4o. WebSocket and WebRTC. Audio streamed as base64 PCM chunks.

## GPU Cloud Providers

> Serverless and on-demand GPU platforms for running audio models.

- **[fal.ai](https://fal.ai)** – Serverless inference for generative media. [Docs](https://docs.fal.ai)
- **[Modal](https://modal.com)** – Serverless Python-first GPU platform. Sub-second cold starts. [Docs](https://modal.com/docs/guide)
- **[Replicate](https://replicate.com)** – Serverless model hosting for open-source audio models. [Docs](https://replicate.com/docs)
- **[RunPod](https://www.runpod.io)** – GPU pods and serverless endpoints. REST, GraphQL, and CLI. [Docs](https://docs.runpod.io)

## Evaluation and Observability

> Benchmarks, leaderboards, and perceptual quality metrics for audio and speech.

- **[WER via Whisper](https://github.com/openai/whisper)** – Standard intelligibility metric. Run synthesized speech through Whisper ASR and measure transcription error rate.
- **[DNSMOS (Microsoft)](https://github.com/microsoft/DNS-Challenge)** – Deep Noise Suppression MOS. Non-intrusive perceptual quality metric for speech enhancement. P.835 framework. Also in torchmetrics.
- **[UTMOS](https://github.com/sarulab-speech/UTMOS22)** – MOS prediction system from UTokyo-Sarulab. Predicts Mean Opinion Score without human listeners. Pearson correlation ~0.82. [Docs](https://arxiv.org/abs/2204.02152)
- **[Speech Arena (Artificial Analysis)](https://huggingface.co/spaces/ArtificialAnalysis/Speech-Arena-Leaderboard)** – Broader speech model leaderboard including latency, cost, and quality dimensions.
- **[TTS Arena (HuggingFace)](https://huggingface.co/spaces/TTS-AGI/TTS-Arena-V2)** – Community blind pairwise voting with Elo-style ranking. The most referenced human-preference benchmark for TTS. [Docs](https://huggingface.co/blog/arena-tts)

## Templates and Example Projects

> Reference implementations, demos, and starter projects.

- **[Real-Time Voice Cloning](https://github.com/CorentinJ/Real-Time-Voice-Cloning)** – Classic SV2TTS demo. Clone a voice in 5 seconds. ~55k stars.
- **[Kokoro Web](https://github.com/eduardolat/kokoro-web)** – Self-hosted, OpenAI API-compatible TTS server using Kokoro-82M. Drop-in replacement for OpenAI TTS endpoint.
- **[Stable Audio Open Demo](https://github.com/Stability-AI/stable-audio-open-demo)** – Official Stability AI demo notebook for Stable Audio Open 1.0.
- **[B2 Whisper Transcriber](https://github.com/backblaze-b2-samples/b2-whisper-transformersjs-transcriber)** – Audio transcription app using Whisper and Transformers.js with Backblaze B2 cloud storage. [B2 integration](https://github.com/backblaze-b2-samples/b2-whisper-transformersjs-transcriber)
- **[ACE-Step Demo](https://ace-step.github.io/)** – Official music generation samples and comparisons.
- **[HuggingFace Speech-to-Speech](https://github.com/huggingface/speech-to-speech)** – Cascaded VAD → STT → LLM → TTS pipeline for local voice agents. Supports Whisper, MeloTTS, and Hugging Face LLMs via server/client or WebSocket.
- **[LiveKit Agent Examples](https://github.com/livekit-examples)** – Official examples for building voice/video AI agents.

---

## Contributing

Contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md). One entry per PR — edit `entries.yaml` only and let the maintainers regenerate `README.md`.

## License

Released under [CC0 1.0 Universal](LICENSE). You may copy, modify, and redistribute without attribution.

## About Backblaze B2

[Backblaze B2 Cloud Storage](https://www.backblaze.com/cloud-storage) is S3-compatible object storage designed for AI and media workloads. This list is maintained as part of our work making B2 a convenient storage layer for AI workflows.
