<h1>Hi, I'm Hisham 👋</h1>

**I use data science and ML to find the moments people want to watch.** My Python pipelines pull signals out of raw audio, video and chat with machine learning models, rank what's worth making, and measure how each upload performs.

🌐 **Portfolio:** [hishamkhan1.github.io](https://hishamkhan1.github.io)

## 📈 Proven results

**Funnycom**, the comedy channel I run, Jan 1 – Dec 31, 2025 (YouTube Studio):

| Views | Watch time | Subscribers | Est. revenue |
|:-:|:-:|:-:|:-:|
| **3.1M** | **558.1K hrs** | **+4.9K** | **$6.6K** |

≈10.8 min watched per view · ≈$2.13 per 1,000 views · ≈1.6 new subscribers per 1,000 views · best day ~87K views

<a href="https://hishamkhan1.github.io/#results"><img src="https://raw.githubusercontent.com/HishamKhan1/HishamKhan1.github.io/master/assets/results/funnycom-2025-youtube-studio.png" width="640" alt="YouTube Studio Insights for Funnycom, 2025: 3.1M views, 558.1K watch hours, +4.9K subscribers, $6.6K estimated revenue"></a>

<sub>The videos behind these numbers have since been set to private. FunnyComm automates the clip-to-Short workflow behind the channel.</sub>

## 🚀 Projects

| | Project | What it does |
|:-:|---|---|
| <img src="https://raw.githubusercontent.com/HishamKhan1/funnycomm-twitch-pipeline/main/assets/funnycomm.png" width="48" alt=""> | **[FunnyComm Twitch Pipeline](https://github.com/HishamKhan1/funnycomm-twitch-pipeline)** | Finds the funniest Twitch moments with five ML models (speech, laughter, faces, chat OCR, safety), crowd-signal clustering and a scoring model, then edits face-aware vertical Shorts with a human review queue and scheduled YouTube upload. |
| <img src="https://raw.githubusercontent.com/HishamKhan1/anime-what-if-studio/main/assets/logo_128.png" width="48" alt=""> | **[Anime What If Studio](https://github.com/HishamKhan1/anime-what-if-studio)** | Produces long-form narrated "What if…?" anime episodes: story linter, AI artwork, ElevenLabs narration, 60 FPS motion, a locally synthesized score and hard cost caps. |
| <img src="https://raw.githubusercontent.com/HishamKhan1/HishamKhan1.github.io/master/assets/youtube-automation-pipeline.svg" width="48" alt=""> | **[YouTube Automation Pipeline](https://github.com/HishamKhan1/youtube-automation-pipeline)** | Generates complete long-form horror story videos: AI story generation and revision, TTS, word-aligned subtitles, FFmpeg rendering and thumbnails. |
| <img src="https://raw.githubusercontent.com/HishamKhan1/HishamKhan1.github.io/master/assets/streamer-shorts-studio.svg" width="48" alt=""> | **[Streamer Shorts Studio](https://github.com/HishamKhan1/streamer-shorts-studio)** | Turns landscape stream clips into 1080×1920 Shorts with automatic webcam detection, green-screen keying and a scene-aware moving crop. Runs fully offline. |

## 🧑‍💻 How I build

**Written by me, optimized with AI.** I'm not a vibe coder. I plan each pipeline, decide how it should work and write much of the code myself. I use AI assistants to optimize, refactor and catch bugs in code I already understand, the way I'd use a code reviewer.

The proof is in the repos: thresholds measured on my own data (a duplicate-audio cutoff from 114 files, safety limits from real clips), 170+ automated tests, and version histories that show each tool growing release by release.

## 🛠️ Tech I use

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![FFmpeg](https://img.shields.io/badge/FFmpeg-007808?style=for-the-badge&logo=ffmpeg&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0097A7?style=for-the-badge&logo=google&logoColor=white)
![ONNX](https://img.shields.io/badge/ONNX-005CED?style=for-the-badge&logo=onnx&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_API-412991?style=for-the-badge&logo=openai&logoColor=white)
![ElevenLabs](https://img.shields.io/badge/ElevenLabs-000000?style=for-the-badge&logoColor=white)
![YouTube API](https://img.shields.io/badge/YouTube_Data_API-FF0000?style=for-the-badge&logo=youtube&logoColor=white)
![Twitch API](https://img.shields.io/badge/Twitch_API-9146FF?style=for-the-badge&logo=twitch&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![C#](https://img.shields.io/badge/C%23-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)

## 🧠 Data science in my pipelines

- **ML signal extraction:** five models run locally on CPU: Whisper (speech), a CED audio tagger (laughter, screams, music), YuNet (faces), OCR (stream chat) and NudeNet (safety)
- **Feature engineering:** loudness percentiles, spectral brightness, motion, face tracks and laughing-chat bursts aligned to the moment that caused them
- **Clustering:** a 180-day clip index groups clips of the same stream seconds, so moments many viewers clipped rank highest
- **Scoring that learns:** a weighted score ranks clips, and keep rates from my review queue adjust it
- **A/B testing:** square and full-screen Shorts take turns, with views pulled per upload from the YouTube Data API
- **Data engineering:** an 8-table SQLite database with an event log, backups, duplicate detection and API cost tracking
- **Tested:** 170+ automated tests across my projects
