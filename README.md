# Timeline Studio — Browser AI Video Editor

[![Live Demo](https://img.shields.io/badge/Live_Demo-Timeline_Studio-35ead9?style=flat-square)](https://video-editor.ai-creator.top/)
[![MIT License](https://img.shields.io/github/license/MartinDelophy/ai-video-editor?style=flat-square)](LICENSE)
[![skills.sh](https://skills.sh/b/MartinDelophy/ai-video-editor)](https://skills.sh/MartinDelophy/ai-video-editor)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md) [![LINUX DO](https://shorturl.at/ggSqS)](https://linux.do)
<a href="https://toolindex.net/tools/timeline-studio?ref=badge" target="_blank" rel="noopener">
  <img src="https://toolindex.net/badge/timeline-studio/small.svg?theme=dark" alt="Timeline Studio - Listed on Tool Index" width="130" height="30" />
</a>

## Responsible use of deep synthesis

This tool uses deep-synthesis technology and is intended solely for technical research and learning.

Users must ensure that they:

- use only facial images or videos of themselves or people who have provided lawful authorization;
- do not create or distribute any illegal, infringing, false, or misleading content;
- do not present generated content as authentic footage or impersonate another person without their consent.

Users are solely responsible for any legal liability arising from violations of these requirements.

## Project updates

- **2026-09-27** — Automatic captions now use word timestamps with short-phrase or word-by-word grouping, preventing long subtitle blocks in portrait videos. Preview, export and SRT share the same editable timed clips; controls support all 13 interface languages. AI voice generation also splits long scripts before synthesis and times each caption to its own audio, including caption-scoped voice generation. Caption display and SRT hide trailing commas, periods and semicolons while retaining expressive punctuation and the original editing/voice text.
- **2026-09-27** — Desktop playback now pages the timeline at the 85% edge, returning the playhead to 20%. Manual horizontal scrolling suspends following; Return to playhead or restarting playback restores it. Pausing preserves the view.
- **2026-09-27** — Unified video clips: main-video and picture-in-picture clips now combine a filename rail, filmstrip and source-audio waveform. Adjust each clip’s dB directly on its waveform, with matching preview/export gain and gain retained after audio separation. Includes all 13 interface languages. All audio lanes use fine bottom-aligned waveforms that follow gain, with orange caps above the display ceiling and existing track styling preserved. Timeline scrubbing advances the preview without waiting for compositor callbacks; release retains exact-frame confirmation.
- **2026-09-21 — Remove pauses:** Smart now detects long speech pauses locally with Silero VAD, lets you review and select cuts, and trims the selected main-track video with its source audio. Adjustable pause thresholds, retained gaps, ripple editing, cancellation and undo are included, with direct UI copy in all 13 languages.
- **2026-09-20 — Playhead marker snapping:** Dragging the white playhead previews the picture live and snaps to markers and range edges, with a shared alignment guide and time readout. Hold Alt to scrub freely. Marker details show Done until edited, then Apply changes.

See the public [Roadmap](ROADMAP.md) for planned work, [Releases](https://github.com/MartinDelophy/ai-video-editor/releases) for shipped changes, and [Issues](https://github.com/MartinDelophy/ai-video-editor/issues) for focused tasks and bugs.

## What can it produce?

Explore reproducible before/after examples and editing recipes:

→ [AI Video Editing Skills Handbook](https://github.com/MartinDelophy/timeline-studio-handbook)

<p align="center">
  <a href="https://trendshift.io/repositories/77422?utm_source=trendshift-badge&amp;utm_medium=badge&amp;utm_campaign=badge-trendshift-77422" target="_blank" rel="noopener noreferrer"><img src="https://trendshift.io/api/badge/trendshift/repositories/77422/daily?language=JavaScript" alt="MartinDelophy%2Fai-video-editor | Trendshift" width="250" height="55"/></a>
  <a href="https://trendshift.io/repositories/77422?utm_source=trendshift-badge&amp;utm_medium=badge&amp;utm_campaign=badge-trendshift-77422" target="_blank" rel="noopener noreferrer"><img src="https://trendshift.io/api/badge/trendshift/repositories/77422/weekly?language=JavaScript" alt="MartinDelophy%2Fai-video-editor | Trendshift" width="250" height="55"/></a>
</p>

Timeline Studio is a local-first AI video editor that runs in the browser. It combines a CapCut-style multi-track timeline with WebGPU AI music and repair, multilingual voiceovers, automatic captions, talking-avatar generation, and deterministic offline export.

[Open the editor](https://video-editor.ai-creator.top/) · [Watch on YouTube](https://youtu.be/bqKhpPPa-qo) · [Hugging Face Space](https://huggingface.co/spaces/haixin/timeline-studio)

## Video demo

### Auto Edit

Visual analysis, keyframes, captions, and export.

https://github.com/user-attachments/assets/e8327caa-429e-40ff-a7fe-a59e6cf7a464

### AI Repair

Timed watermark removal with before/after review.

https://github.com/user-attachments/assets/aea9f5b4-c720-4b0c-9067-5ec124eef982


Timeline Studio — Browser AI Video Editor
A local-first, browser-native AI video editing platform built around modern Web APIs, on-device inference, multi-track editing, and deterministic media export.

https://img.shields.io/badge/Live_Demo-video--editor.ai--creator.top-6C47FF?style=for-the-badge&logo=googlechrome&logoColor=white
https://img.shields.io/badge/Source-GitHub-181717?style=for-the-badge&logo=github&logoColor=white
https://img.shields.io/badge/Roadmap-ROADMAP.md-0A66C2?style=for-the-badge&logo=readthedocs&logoColor=white
https://img.shields.io/badge/Contributing-CONTRIBUTING.md-2EA043?style=for-the-badge&logo=handshake&logoColor=white

https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square
https://img.shields.io/badge/Model_Licenses-MODEL__LICENSES.md-orange?style=flat-square
https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black
https://img.shields.io/badge/TypeScript-5.x-3178C6?style=flat-square&logo=typescript&logoColor=white
https://img.shields.io/badge/Vite-Bundler-646CFF?style=flat-square&logo=vite&logoColor=white
https://img.shields.io/badge/WebGPU-Accelerated-00C7B7?style=flat-square&logo=webgpu&logoColor=white
https://img.shields.io/badge/ONNX_Runtime-Web-005CED?style=flat-square&logo=onnx&logoColor=white
https://img.shields.io/badge/WebCodecs-Native-4285F4?style=flat-square&logo=googlechrome&logoColor=white
https://img.shields.io/badge/FFmpeg-WASM-007808?style=flat-square&logo=ffmpeg&logoColor=white
https://img.shields.io/badge/PWA-Installable-5A0FC8?style=flat-square&logo=pwa&logoColor=white

Product Overview
Timeline Studio is a local-first AI video editor that brings a professional multi-track editing workflow and browser-native AI inference into a single web application.

Instead of treating the browser as a thin client for a remote media backend, Timeline Studio explores how far a modern browser can go as the editing runtime itself.

The application combines:

Professional multi-track timeline editing

Browser-local AI inference

WebGPU acceleration

ONNX Runtime Web

WebAssembly media processing

WebCodecs-based video composition

FFmpeg/WASM fallback processing

Automatic speech recognition and captions

AI music generation

AI voice synthesis

Intelligent subject detection and framing

Image/video restoration and repair

Vocal separation

Digital-human generation

Portable .timeline projects

Installable PWA support

Deterministic offline-oriented export workflows

Core idea: Move as much of the media and AI workflow as practical into the browser while preserving an editable timeline as the source of truth.

Why This Project Is Interesting
Traditional web video editors commonly depend on a server-side pipeline:

text
User Media → Upload → Remote Processing → AI/Rendering Backend → Encoded Output → Download
Timeline Studio explores a different architecture:

text
                 BROWSER
┌─────────────────────────────────────────────────┐
│                                                 │
│  Media ───────► Timeline Engine                 │
│                     │                           │
│                     ├────► Video / Audio        │
│                     │                           │
│                     ├────► AI Inference         │
│                     │          │                │
│                     │       WebGPU              │
│                     │       ONNX                │
│                     │       WASM                │
│                     │                           │
│                     └────► Composition          │
│                                │                │
│                         WebCodecs / FFmpeg      │
│                                │                │
│                                ▼                │
│                           MP4 / WebM            │
│                                                 │
└─────────────────────────────────────────────────┘
Supported workflows can run without uploading project media to an editing backend.

This architecture introduces a different engineering problem: browser constraints become part of the system design. That means dealing with GPU availability, WASM execution, model size, browser memory, worker isolation, model loading/caching, media decoding, audio synchronization, preview performance, export determinism, and cross-browser API availability.

Key Capabilities
1. Multi-Track Timeline
Timeline Studio provides a CapCut-style editing model with a portable, editable timeline.

Editing	Organization	Visual
Split / duplicate / delete	Contiguous main Visuals track	Direct canvas manipulation
Undo / redo	Picture-in-picture overlays	Proportional resize
Timeline zoom	Independent captions	Rotation
Snapping	Stickers	Masks
Alignment guides	Voiceover	Filters
Clip menus	Separated source audio	Effects
Explicit keyframes	Music	Animation
Color grading	Portable .timeline projects	Speed control
The timeline is treated as structured data rather than an opaque rendered video.

2. Browser AI Engine
Timeline Studio integrates multiple AI workloads directly into the browser.

🎵 AI Music
Stable Audio 3 Small Q4 ONNX

WebGPU inference

Free-form prompts & prompt translation

30 / 60 / 90 / 120 second generation

Waveform-aware long-track looping

Persistent model caching

Automatic insertion into project assets

text
Prompt → Prompt Translation → Stable Audio → WebGPU/ONNX → Generated Audio
   → Waveform Analysis → Timeline Music Track
📝 Automatic Captions
Whisper small q8 ONNX

Local transcription, word timestamps

Short phrase / word grouping

Waveform-aware timing

Editable caption clips

Synchronized preview and export

SRT generation

Multilingual UI

Caption-scoped voice generation

text
Preview → Timeline captions
       → Export
       → SRT
🎯 Smart Framing
YOLOS tiny for subject detection

MODNet for portrait matting

Subject-aware cropping, portrait framing

Caption-safe positioning

Background removal

Image & complete-video processing

text
Video/Image → Subject Detection → Bounding/Matte → Framing Logic
   → Smart Crop / Caption Avoidance / Background Removal
🛠 AI Repair
MI-GAN — watermark/object removal with timed repair regions and before/after review

NanoVSR — WebGPU-based restoration and 4× enhancement workflows

Reversible visual review rather than immediately replacing the source

🎙 AI Voiceover
Kokoro 82M

Piper browser voices

VITS-based voices

Multilingual voice workflows

Long-script chunking & phrase-level synthesis

Audio-aware caption timing

🎚 AI Vocal Separation
Isolate vocals and place resulting instrumental material into the music workflow — no desktop application required.

🧑 Digital Human
JoyVASA + LivePortrait

WebGPU acceleration

256px preview paths / 512px quality paths

text
Audio → JoyVASA → Audio-to-Motion → LivePortrait → Neural Rendering → Digital Human
3. Local-First Model Delivery
Large browser models are expensive in bandwidth and memory, so model lifecycle is treated as part of the application architecture.

Lazy model loading

Revision-pinned model assets

Service-worker caching

Persistent browser cache

Multiple model mirrors (Hugging Face + ModelScope)

Runtime source fallback

The application remembers a working model source and falls back when a source is unavailable.

4. Media Engine
Technology	Role
WebCodecs	Browser-native video/audio encoding & decoding
FFmpeg WASM	Media processing and fallback workflows
MediaBunny	Browser media pipeline utilities
LibAV / WebCodecs	Media compatibility paths
AAC Encoder	Browser audio encoding
Web Audio	Audio processing and mixing
Canvas	Visual composition
Web Workers	Heavy background processing
5. Preview vs Export Architecture
A major architectural decision is separating interactive preview from deterministic export.

Interactive Preview	Deterministic Export
Responsiveness	Reproducibility
Scrubbing	Correct timing
Interactive editing	Consistent geometry
Direct media playback	Audio mixing
Low-latency UI feedback	Captions, overlays, effects
Final encoding
text
                    PROJECT MODEL
                         │
              ┌──────────┴──────────┐
              ▼                     ▼
        INTERACTIVE             EXPORT
          PREVIEW              PIPELINE
              │                     │
        Native Playback       Composition
              │                     │
              │               WebCodecs
              │                     │
              │                  FFmpeg
              └──────────┬──────────┘
                         ▼
                    FINAL MEDIA
The project model remains the source of truth.

6. Portable .timeline Projects
A project can contain structured information for:

Tracks, clips, timestamps

Captions, overlays, audio, transitions

Project settings, media references, editing properties

This makes the editing state inspectable, reproducible, editable, automatable, and suitable for agent workflows.

Agent & Automation Layer
The repository includes an AI Video Editing Skill designed for Codex, Claude Code, Copilot, and Gemini CLI workflows.

The agent layer can help with:

Inspecting media & project structure

Planning and validating edits

Applying supported timeline operations

Inspecting tracks, clips, and transcripts

Producing field-level diffs

Transactional operations with idempotent operation IDs

Rendering supported project subsets

Verifying generated project artifacts

Example Commands
bash
npm run agent -- project.inspect /absolute/path/project.timeline
npm run agent -- track.inspect /absolute/path/project.timeline visuals
npm run agent -- clip.inspect /absolute/path/project.timeline visual-123
npm run agent -- transcript.inspect /absolute/path/project.timeline voice-123
npm run agent -- project.diff /absolute/path/edit-plan.json
npm run agent -- project.run /absolute/path/edit-plan.json
npm run agent -- project.render /absolute/path/render-request.json
The repository also contains a browser WebMCP integration for structured project operations and browser-based compatibility workflows.

Architecture
text
┌───────────────────────────────────────────────────────────────┐
│                         REACT UI                              │
│ Editor · Timeline · Canvas · Panels · Assets · Controls       │
└──────────────────────────────┬────────────────────────────────┘
                               ▼
┌───────────────────────────────────────────────────────────────┐
│                     PROJECT / TIMELINE MODEL                   │
│ Tracks · Clips · Captions · Keyframes · Effects · Audio       │
└───────────────┬─────────────────────┬─────────────────────────┘
                ▼                     ▼
┌──────────────────────────┐  ┌─────────────────────────────────┐
│      MEDIA PIPELINE      │  │           AI PIPELINE           │
│ WebCodecs · MediaBunny   │  │ ONNX Runtime Web · WebGPU       │
│ FFmpeg WASM · AAC        │  │ Transformers · MediaPipe        │
│ Web Audio                │  │ Whisper · Stable Audio          │
└─────────────┬────────────┘  │ MI-GAN · YOLOS/MODNet           │
              ▼               │ NanoVSR · JoyVASA/LivePortrait  │
┌──────────────────────────┐  └──────────────┬──────────────────┘
│       COMPOSITOR         │                 │
│   Preview + Export       │                 │
└─────────────┬────────────┘                 │
              └──────────────┬───────────────┘
                             ▼
                    ┌─────────────────┐
                    │ FINAL EXPORT    │
                    │   MP4 / WebM    │
                    └─────────────────┘
Repository Structure
text
.
├── src/
│   ├── assets/
│   ├── components/
│   ├── config/
│   ├── hooks/
│   ├── lib/
│   │   ├── __fixtures__/
│   │   └── ...
│   ├── plugins/
│   │   └── generation/
│   ├── styles/
│   ├── vendor/
│   │   └── libav-timeline-compat/
│   └── workers/
├── scripts/
│   └── timeline-command.mjs
├── skills/
│   └── edit-timeline-studio/
├── docs/
│   ├── screenshots/
│   └── ...
├── index.html
├── package.json
├── vite.config.mjs
├── tsconfig.json
├── eslint.config.js
├── netlify.toml
├── ROADMAP.md
├── MODEL_LICENSES.md
├── CONTRIBUTING.md
└── LICENSE
Technology Stack
Frontend
https://img.shields.io/badge/React_19-61DAFB?style=flat-square&logo=react&logoColor=black
https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white
https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white
https://img.shields.io/badge/Phosphor_Icons-FF6B6B?style=flat-square&logo=phosphor&logoColor=white

React 19, TypeScript, Vite, React DOM, Phosphor Icons

Browser AI / ML
https://img.shields.io/badge/ONNX_Runtime_Web-005CED?style=flat-square&logo=onnx&logoColor=white
https://img.shields.io/badge/WebGPU-00C7B7?style=flat-square&logo=webgpu&logoColor=white
https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black
https://img.shields.io/badge/MediaPipe-0097A7?style=flat-square&logo=google&logoColor=white
https://img.shields.io/badge/WebAssembly-654FF0?style=flat-square&logo=webassembly&logoColor=white

ONNX Runtime Web, Hugging Face Transformers, WebGPU, MediaPipe, WebAssembly

Kokoro, VITS, Piper, Whisper, Stable Audio

YOLOS, MODNet, MI-GAN, NanoVSR, JoyVASA, LivePortrait

Media
https://img.shields.io/badge/WebCodecs-4285F4?style=flat-square&logo=googlechrome&logoColor=white
https://img.shields.io/badge/FFmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white
https://img.shields.io/badge/Web_Audio-FF6B00?style=flat-square&logo=webaudio&logoColor=white

WebCodecs, FFmpeg, MediaBunny, LibAV compatibility layer, AAC encoding, Web Audio APIs

Application Architecture
https://img.shields.io/badge/PWA-5A0FC8?style=flat-square&logo=pwa&logoColor=white
https://img.shields.io/badge/Service_Worker-4285F4?style=flat-square&logo=googlechrome&logoColor=white
https://img.shields.io/badge/Zod-3E67B1?style=flat-square&logo=zod&logoColor=white

Service Worker, PWA, Web Workers, Local browser caching

Portable project files, MCP / WebMCP tooling, Zod validation

Browser Requirements
Recommended
Chromium-based browser (recent Chrome / Chromium / Edge)

WebGPU-enabled hardware

Capability Matrix
Capability	Requirement
WebGPU	✓ Recommended
WebAssembly	✓ Required for several workflows
WebCodecs	✓ Recommended
Workers	✓ Required by heavy processing paths
IndexedDB	✓ Recommended for model caching
The heaviest AI workflows benefit significantly from WebGPU. Hardware and browser support can affect model loading, inference speed, memory usage, available AI features, and export performance.

Quick Start
1. Clone
bash
git clone https://github.com/MartinDelophy/ai-video-editor.git
cd ai-video-editor
2. Install dependencies
bash
npm install
3. Start development server
bash
npm run dev
Open the local URL printed by Vite. The first AI workflow may download model assets — later runs can reuse browser cache.

Production Build
bash
npm run build
npm run preview   # preview the production build
Repository Validation
Run the complete project check:

bash
npm run check
This runs:

text
ESLint → TypeScript → Vite production build
Individual Checks
bash
npm run lint
npm run typecheck
npm run build
Formatting
bash
npm run format
npm run format:check
Deployment
The repository includes a netlify.toml configuration.

bash
npm run build
npx netlify-cli deploy --prod --dir=dist
The deployment configuration is designed around:

Vite output

SPA fallback

Browser media workers

Cross-origin isolation requirements used by browser AI/media workflows

Performance & Engineering Considerations
Browser AI changes the usual frontend performance model. The application has to manage several expensive resources simultaneously:

text
               Browser Memory
                     │
        ┌────────────┼────────────┐
        ▼            ▼            ▼
      Video         Audio       AI Models
        │            │            │
        └────────────┼────────────┘
                     ▼
                  Timeline
                     ▼
                 Compositor
                     ▼
                  Export
Important Engineering Concerns
Model Lifecycle — Models should not all load at application startup:

text
User requests feature → Lazy-load model → Initialize runtime
   → Run inference → Cache model → Reuse on future runs
Heavy Computation — Long-running AI and media operations use workers so the UI remains responsive.

Preview Performance — Interactive preview prioritizes responsiveness rather than performing a full final-quality render for every frame.

Export Correctness — The export path independently composes the timeline so final media output does not depend on the exact state of interactive preview rendering.

Feature Matrix
Area	Capability
Timeline	Multi-track editing
Video	Main visual track + overlays
Audio	Voiceover, music, separated source audio
Captions	Whisper transcription + editable timed clips
AI Music	Stable Audio via WebGPU / ONNX
AI Repair	MI-GAN
Restoration	NanoVSR
Smart Crop	YOLOS + MODNet
Voice	Kokoro / Piper / VITS workflows
Vocal Separation	Browser-local separation
Digital Human	JoyVASA + LivePortrait
Rendering	WebCodecs + FFmpeg fallback
Projects	Portable .timeline files
PWA	Installable application
Caching	Service worker + model cache
Automation	Agent Skill + command runner
Browser Automation	WebMCP integration
Localization	13 interface languages
Security & Privacy Model
Timeline Studio is designed around a local-first workflow.

For supported local inference paths:

text
User Media → Browser
              ├── AI inference
              ├── timeline processing
              ├── media composition
              └── export
…rather than automatically sending project media to a remote editing backend.

Users should distinguish between:

Local media processing

Remote model delivery

Optional external integrations

Third-party model hosting

Model files may be downloaded from configured model providers even when the actual project media remains local.

Responsible Use of Deep-Synthesis Features
Timeline Studio contains deep-synthesis capabilities including voice generation and digital-human workflows. Use these features responsibly.

Users should:

Use facial images, videos, and voices they own or are legally authorized to process

Obtain appropriate consent when working with another person's likeness or voice

Avoid deceptive impersonation

Avoid creating or distributing illegal, infringing, fraudulent, or misleading content

Clearly distinguish generated media from authentic recordings where appropriate

Third-party model licenses and usage restrictions may apply independently of the project's MIT license. See MODEL_LICENSES.md before redistribution or commercial use.

Model & Asset Licensing
The original application source is licensed under MIT.

However:

The MIT license does not automatically apply to third-party model weights, datasets, fonts, stock media, or remotely downloaded AI assets.

Always review the upstream license for each model before:

Redistribution

Commercial deployment

Bundling model weights

Publishing derivative assets

Creating hosted services

Relevant model documentation and licenses should be treated independently from the source-code license.

Development Roadmap
The project roadmap focuses on improving the editing and automation architecture.

🎯 Current Focus
Deterministic offline export

Timeline reliability

Command registry expansion

Browser media reliability

🔜 Next
Improved headless/browser render parity

Expanded WebMCP command coverage

More robust automated project verification

🔮 Later
Collaborative review workflows

Plugin extension surfaces

Additional locally verified AI models

See ROADMAP.md.

Contributing
Contributions are welcome around:

browser media · WebCodecs · WebGPU · ONNX Runtime · AI model integration · timeline UX · performance · testing · localization · accessibility · documentation · automation tooling

Before submitting a change:

bash
npm run check
For contribution guidelines, see CONTRIBUTING.md.

Useful Commands
bash
# Development
npm run dev

# Production build
npm run build

# Preview build
npm run preview

# Lint
npm run lint

# Type check
npm run typecheck

# Complete validation
npm run check

# Formatting
npm run format
npm run format:check

# Timeline agent
npm run agent -- project.inspect /absolute/path/project.timeline

# MCP server
npm run mcp

# Skill diagnostics
npm run skill:doctor

# Skill setup
npm run skill:setup
Project Philosophy
Timeline Studio is built around a few architectural principles:

#	Principle	Description
01	Browser as a compute platform	The browser is treated as a serious execution environment rather than merely a presentation layer.
02	Local-first media	When technically supported, media processing and AI inference should happen close to the user's device.
03	Structured editing	The timeline is structured, inspectable data.
04	Deterministic output	Export should be reproducible from the project representation.
05	Progressive AI	AI features should load when needed instead of forcing every model into the initial application payload.
06	Graceful degradation	The application should provide fallbacks when browser capabilities, GPU acceleration, or specific model runtimes are unavailable.
07	Automation-friendly workflows	An editable project representation makes video editing more suitable for programmatic tooling and AI agents.
What Makes the Architecture Different?
The interesting engineering challenge is not simply integrating an AI model. It is coordinating:

text
               ┌─────────────┐
               │   React UI  │
               └──────┬──────┘
                      ▼
               ┌─────────────┐
               │   Timeline  │
               └──────┬──────┘
          ┌───────────┼───────────┐
          ▼           ▼           ▼
       VIDEO        AUDIO         AI
          │           │           │
      WebCodecs   Web Audio     WebGPU
          │           │         ONNX
          │           │          WASM
          └───────────┼───────────┘
                      ▼
                COMPOSITION
                      ▼
                   EXPORT
…while keeping the application responsive and preserving an editable project model.

That combination makes Timeline Studio as much a browser systems project as it is a video editor.

Demo
Resource	Link
🌐 Live Editor	video-editor.ai-creator.top
▶️ YouTube	youtu.be/bqKhpPPa-qo
🤗 Hugging Face Space	huggingface.co/spaces/haixin/timeline-studio
Interactive Showcase
The repository can also be paired with the included cinematic portfolio showcase page to demonstrate:

The architecture

The AI pipeline

The interactive timeline

Local inference

Media processing

Export flow

Recruiter-oriented engineering overview

Screenshots & Media
Recommended repository presentation:

text
docs/
└── screenshots/
    ├── editor-timeline.png
    ├── ai-music.png
    ├── ai-repair.png
    ├── captions.png
    ├── smart-framing.png
    └── export.png
💡 Tip: For a polished GitHub landing page, place the strongest editor screenshot directly below the project overview and use short GIF/video demonstrations for the most visual AI workflows.

Status
Timeline Studio is an actively developed browser AI media application.

The architecture continues to evolve around:

Browser-native AI

Deterministic rendering

Timeline reliability

Media interoperability

AI-assisted editing

Automation

Local-first workflows

License
The original Timeline Studio source code is licensed under the MIT License.

Third-party models, weights, datasets, media, fonts, and other assets remain subject to their respective licenses and terms.

See MODEL_LICENSES.md for model-specific licensing information.

<p align="center"> <strong>Timeline Studio</strong><br/> <em>Browser-native AI video editing · Local-first inference · Structured timelines · Deterministic media export</em> </p><p align="center"> <a href="https://video-editor.ai-creator.top/">Live Demo</a> · <a href="https://github.com/MartinDelophy/ai-video-editor">Source</a> · <a href="ROADMAP.md">Roadmap</a> · <a href="CONTRIBUTING.md">Contributing</a> </p>
