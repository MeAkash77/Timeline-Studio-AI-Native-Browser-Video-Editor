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

<p align="center">
  <strong>A local-first, browser-native AI video editing platform built around modern Web APIs, on-device inference, multi-track editing, and deterministic media export.</strong>
</p>

<p align="center">
  <a href="https://video-editor.ai-creator.top/">Live Demo</a>
  ·
  <a href="https://github.com/MartinDelophy/ai-video-editor">Source</a>
  ·
  <a href="ROADMAP.md">Roadmap</a>
  ·
  <a href="CONTRIBUTING.md">Contributing</a>
</p>

<p align="center">











</p>

Product Overview

Timeline Studio is a local-first AI video editor that brings a professional multi-track editing workflow and browser-native AI inference into a single web application.

Instead of treating the browser as a thin client for a remote media backend, Timeline Studio explores how far a modern browser can go as the editing runtime itself.

The application combines:

professional multi-track timeline editing;

browser-local AI inference;

WebGPU acceleration;

ONNX Runtime Web;

WebAssembly media processing;

WebCodecs-based video composition;

FFmpeg/WASM fallback processing;

automatic speech recognition and captions;

AI music generation;

AI voice synthesis;

intelligent subject detection and framing;

image/video restoration and repair;

vocal separation;

digital-human generation;

portable .timeline projects;

installable PWA support;

deterministic offline-oriented export workflows.

Core idea: move as much of the media and AI workflow as practical into the browser while preserving an editable timeline as the source of truth.

Why This Project Is Interesting

Traditional web video editors commonly depend on a server-side pipeline:

User Media
    │
    ▼
Upload
    │
    ▼
Remote Processing
    │
    ▼
AI / Rendering Backend
    │
    ▼
Encoded Output
    │
    ▼
Download

Timeline Studio explores a different architecture:

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
│                     └────► Composition           │
│                                │                │
│                         WebCodecs / FFmpeg       │
│                                │                │
│                                ▼                │
│                           MP4 / WebM             │
│                                                 │
└─────────────────────────────────────────────────┘

Supported workflows can run without uploading project media to an editing backend.

This architecture introduces a different engineering problem: browser constraints become part of the system design.

That means dealing with:

GPU availability;

WASM execution;

model size;

browser memory;

worker isolation;

model loading and caching;

media decoding;

audio synchronization;

preview performance;

export determinism;

cross-browser API availability.

Key Capabilities

1. Multi-Track Timeline

Timeline Studio provides a CapCut-style editing model with a portable, editable timeline.

Editing capabilities

contiguous main Visuals track;

picture-in-picture overlays;

independent captions;

stickers;

voiceover;

separated source audio;

music;

split / duplicate / delete;

undo / redo;

timeline zoom;

snapping;

alignment guides;

clip menus;

direct canvas manipulation;

proportional resize;

rotation;

masks;

filters;

effects;

animation;

speed control;

explicit keyframes;

color grading;

portable .timeline projects.

The timeline is treated as structured data rather than an opaque rendered video.

2. Browser AI Engine

Timeline Studio integrates multiple AI workloads directly into the browser.

AI Music

Stable Audio 3 Small Q4 ONNX

WebGPU inference;

free-form prompts;

prompt translation;

30 / 60 / 90 / 120 second generation;

waveform-aware long-track looping;

persistent model caching;

automatic insertion into project assets.

Prompt
  │
  ▼
Prompt Translation
  │
  ▼
Stable Audio
  │
  ▼
WebGPU / ONNX
  │
  ▼
Generated Audio
  │
  ▼
Waveform Analysis
  │
  ▼
Timeline Music Track

Automatic Captions

Whisper small q8 ONNX

The caption pipeline supports:

local transcription;

word timestamps;

short phrase / word grouping;

waveform-aware timing;

editable caption clips;

synchronized preview and export;

SRT generation;

multilingual UI;

caption-scoped voice generation.

The same editable caption representation can drive:

Preview
   │
   ├──► Timeline captions
   │
   ├──► Export
   │
   └──► SRT

This avoids maintaining separate timing representations for each output path.

Smart Framing

The smart-framing pipeline combines:

YOLOS tiny for subject detection;

MODNet for portrait matting.

It can support:

subject-aware cropping;

portrait framing;

caption-safe positioning;

background removal;

image processing;

complete-video processing.

Conceptually:

Video / Image
      │
      ▼
Subject Detection
      │
      ▼
Bounding / Matte
      │
      ▼
Framing Logic
      │
      ├──► Smart Crop
      ├──► Caption Avoidance
      └──► Background Removal

AI Repair

Browser-local repair workflows use:

MI-GAN

For watermark/object removal with timed repair regions and before/after review.

NanoVSR

For WebGPU-based restoration and 4× enhancement workflows.

The UI is designed around reversible visual review rather than immediately replacing the source.

Source
  │
  ├──────────────► Original
  │
  ▼
Repair / Restoration
  │
  ▼
Preview
  │
  ▼
Before / After
  │
  ▼
Timeline / Export

AI Voiceover

Supported browser voice workflows include:

Kokoro 82M;

Piper browser voices;

VITS-based voices;

multilingual voice workflows;

long-script chunking;

phrase-level synthesis;

audio-aware caption timing.

Long scripts can be divided into smaller synthesis units before being placed back into the timeline.

AI Vocal Separation

Audio separation can isolate vocals and place the resulting instrumental material into the music workflow without requiring a separate desktop application.

Digital Human

The project also integrates neural talking-avatar workflows using:

JoyVASA;

LivePortrait;

WebGPU acceleration;

256px preview paths;

512px quality paths.

The conceptual pipeline is:

Audio
  │
  ▼
JoyVASA
  │
  ▼
Audio-to-Motion
  │
  ▼
LivePortrait
  │
  ▼
Neural Rendering
  │
  ▼
Digital Human

3. Local-First Model Delivery

Large browser models are expensive in terms of bandwidth and memory, so model lifecycle is treated as part of the application architecture.

Timeline Studio uses:

lazy model loading;

revision-pinned model assets;

service-worker caching;

persistent browser cache;

multiple model mirrors;

runtime source fallback.

Model delivery can use both:

Hugging Face;

ModelScope.

The application can remember a working model source for the runtime and fall back when a source is unavailable.

This allows the AI layer to be more resilient without forcing users to manually manage model files.

4. Media Engine

The media pipeline uses modern browser technologies rather than relying on one monolithic renderer.

Core media technologies

Technology

Role

WebCodecs

Browser-native video/audio encoding and decoding

FFmpeg WASM

Media processing and fallback workflows

MediaBunny

Browser media pipeline utilities

LibAV/WebCodecs

Media compatibility paths

AAC Encoder

Browser audio encoding

Web Audio

Audio processing and mixing

Canvas

Visual composition

Web Workers

Heavy background processing

5. Preview vs Export Architecture

A major architectural decision is separating interactive preview from deterministic export.

Preview

Optimized for:

responsiveness;

scrubbing;

interactive editing;

direct media playback;

low-latency UI feedback.

Export

Optimized for:

reproducibility;

correct timing;

consistent geometry;

audio mixing;

captions;

overlays;

effects;

final encoding.

                    PROJECT MODEL
                         │
              ┌──────────┴──────────┐
              │                     │
              ▼                     ▼
        INTERACTIVE             EXPORT
          PREVIEW              PIPELINE
              │                     │
        Native Playback       Composition
              │                     │
              │               WebCodecs
              │                     │
              │                  FFmpeg
              │                     │
              └──────────┬──────────┘
                         ▼
                    FINAL MEDIA

The project model remains the source of truth.

6. Portable .timeline Projects

Timeline Studio uses an editable project representation instead of treating a rendered MP4 as the only artifact.

A project can contain structured information for:

tracks;

clips;

timestamps;

captions;

overlays;

audio;

transitions;

project settings;

media references;

editing properties.

This makes the editing state:

inspectable;

reproducible;

editable;

automatable;

suitable for agent workflows.

Agent & Automation Layer

The repository includes an AI Video Editing Skill designed for Codex, Claude Code, Copilot and Gemini CLI workflows.

The agent layer can help with:

inspecting media;

inspecting project structure;

planning edits;

validating edit plans;

applying supported timeline operations;

inspecting tracks;

inspecting clips;

inspecting transcripts;

producing field-level diffs;

transactional operations;

idempotent operation IDs;

rendering supported project subsets;

verifying generated project artifacts.

Example commands

npm run agent -- project.inspect /absolute/path/project.timeline

npm run agent -- track.inspect /absolute/path/project.timeline visuals

npm run agent -- clip.inspect /absolute/path/project.timeline visual-123

npm run agent -- transcript.inspect /absolute/path/project.timeline voice-123

npm run agent -- project.diff /absolute/path/edit-plan.json

npm run agent -- project.run /absolute/path/edit-plan.json

npm run agent -- project.render /absolute/path/render-request.json

The repository also contains a browser WebMCP integration for structured project operations and browser-based compatibility workflows.

Architecture

At a high level:

┌───────────────────────────────────────────────────────────────┐
│                         REACT UI                              │
│                                                               │
│ Editor · Timeline · Canvas · Panels · Assets · Controls       │
└──────────────────────────────┬────────────────────────────────┘
                               │
                               ▼
┌───────────────────────────────────────────────────────────────┐
│                     PROJECT / TIMELINE MODEL                   │
│                                                               │
│ Tracks · Clips · Captions · Keyframes · Effects · Audio       │
└───────────────┬─────────────────────┬─────────────────────────┘
                │                     │
                ▼                     ▼
┌──────────────────────────┐  ┌─────────────────────────────────┐
│      MEDIA PIPELINE      │  │           AI PIPELINE           │
│                          │  │                                 │
│ WebCodecs                │  │ ONNX Runtime Web                │
│ MediaBunny               │  │ WebGPU                          │
│ FFmpeg WASM              │  │ Transformers                    │
│ AAC                      │  │ MediaPipe                       │
│ Web Audio                │  │ Whisper                         │
└─────────────┬────────────┘  │ Stable Audio                    │
              │               │ MI-GAN                          │
              ▼               │ YOLOS / MODNet                  │
┌──────────────────────────┐  │ NanoVSR                         │
│       COMPOSITOR         │  │ JoyVASA / LivePortrait          │
│                          │  └──────────────┬──────────────────┘
│ Preview + Export         │                 │
└─────────────┬────────────┘                 │
              │                              │
              └──────────────┬───────────────┘
                             ▼
                    ┌─────────────────┐
                    │ FINAL EXPORT    │
                    │ MP4 / WebM      │
                    └─────────────────┘

Repository Structure

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
│
├── scripts/
│   └── timeline-command.mjs
│
├── skills/
│   └── edit-timeline-studio/
│
├── docs/
│   ├── screenshots/
│   └── ...
│
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

React 19

TypeScript

Vite

React DOM

Phosphor Icons

Browser AI / ML

ONNX Runtime Web

Hugging Face Transformers

WebGPU

MediaPipe

WebAssembly

Kokoro

VITS

Piper

Whisper

Stable Audio

YOLOS

MODNet

MI-GAN

NanoVSR

JoyVASA

LivePortrait

Media

WebCodecs

FFmpeg

MediaBunny

LibAV compatibility layer

AAC encoding

Web Audio APIs

Application Architecture

Service Worker

PWA

Web Workers

Local browser caching

Portable project files

MCP / WebMCP tooling

Zod validation

Browser Requirements

Recommended

Chromium-based browser

Recent Chrome / Chromium / Edge

WebGPU-enabled hardware

Recommended capabilities

WebGPU       ✓ Recommended
WebAssembly  ✓ Required for several workflows
WebCodecs    ✓ Recommended
Workers      ✓ Required by heavy processing paths
IndexedDB    ✓ Recommended for model caching

The heaviest AI workflows benefit significantly from WebGPU.

Hardware and browser support can affect:

model loading;

inference speed;

memory usage;

available AI features;

export performance.

Quick Start

1. Clone

git clone https://github.com/MartinDelophy/ai-video-editor.git
cd ai-video-editor

2. Install dependencies

npm install

3. Start development server

npm run dev

Open the local URL printed by Vite.

The first AI workflow may download model assets. Later runs can reuse browser cache.

Production Build

npm run build

Preview the production build:

npm run preview

Repository Validation

Run the complete project check:

npm run check

This runs:

ESLint
   ↓
TypeScript
   ↓
Vite production build

Individual checks:

npm run lint

npm run typecheck

npm run build

Formatting:

npm run format

npm run format:check

Deployment

The repository includes a netlify.toml configuration.

Build:

npm run build

Deploy:

npx netlify-cli deploy --prod --dir=dist

The deployment configuration is designed around:

Vite output;

SPA fallback;

browser media workers;

cross-origin isolation requirements used by browser AI/media workflows.

Performance & Engineering Considerations

Browser AI changes the usual frontend performance model.

The application has to manage several expensive resources simultaneously:

               Browser Memory
                     │
        ┌────────────┼────────────┐
        ▼            ▼            ▼
      Video         Audio       AI Models
        │            │            │
        └────────────┼────────────┘
                     ▼
                  Timeline
                     │
                     ▼
                 Compositor
                     │
                     ▼
                  Export

Important engineering concerns include:

Model lifecycle

Models should not all load at application startup.

Instead:

User requests feature
        ↓
Lazy-load model
        ↓
Initialize runtime
        ↓
Run inference
        ↓
Cache model
        ↓
Reuse on future runs

Heavy computation

Long-running AI and media operations can use workers so that the UI remains responsive.

Preview performance

Interactive preview prioritizes responsiveness rather than performing a full final-quality render for every frame.

Export correctness

The export path independently composes the timeline so that final media output does not depend on the exact state of interactive preview rendering.

Feature Matrix

Area

Capability

Timeline

Multi-track editing

Video

Main visual track + overlays

Audio

Voiceover, music, separated source audio

Captions

Whisper transcription + editable timed clips

AI Music

Stable Audio via WebGPU / ONNX

AI Repair

MI-GAN

Restoration

NanoVSR

Smart Crop

YOLOS + MODNet

Voice

Kokoro / Piper / VITS workflows

Vocal Separation

Browser-local separation

Digital Human

JoyVASA + LivePortrait

Rendering

WebCodecs + FFmpeg fallback

Projects

Portable .timeline files

PWA

Installable application

Caching

Service worker + model cache

Automation

Agent Skill + command runner

Browser Automation

WebMCP integration

Localization

13 interface languages

Security & Privacy Model

Timeline Studio is designed around a local-first workflow.

For supported local inference paths:

User Media
    │
    ▼
Browser
    │
    ├── AI inference
    ├── timeline processing
    ├── media composition
    └── export

rather than automatically sending project media to a remote editing backend.

However, users should distinguish between:

local media processing;

remote model delivery;

optional external integrations;

third-party model hosting.

Model files may be downloaded from configured model providers even when the actual project media remains local.

Responsible Use of Deep-Synthesis Features

Timeline Studio contains deep-synthesis capabilities including voice generation and digital-human workflows.

Use these features responsibly.

Users should:

use facial images, videos, and voices they own or are legally authorized to process;

obtain appropriate consent when working with another person's likeness or voice;

avoid deceptive impersonation;

avoid creating or distributing illegal, infringing, fraudulent, or misleading content;

clearly distinguish generated media from authentic recordings where appropriate.

Third-party model licenses and usage restrictions may apply independently of the project's MIT license.

See:

MODEL_LICENSES.md

before redistribution or commercial use.

Model & Asset Licensing

The original application source is licensed under MIT.

However:

The MIT license does not automatically apply to third-party model weights, datasets, fonts, stock media, or remotely downloaded AI assets.

Always review the upstream license for each model before:

redistribution;

commercial deployment;

bundling model weights;

publishing derivative assets;

creating hosted services.

Relevant model documentation and licenses should be treated independently from the source-code license.

Development Roadmap

The project roadmap focuses on improving the editing and automation architecture.

Current focus

deterministic offline export;

timeline reliability;

command registry expansion;

browser media reliability.

Next

improved headless/browser render parity;

expanded WebMCP command coverage;

more robust automated project verification.

Later

collaborative review workflows;

plugin extension surfaces;

additional locally verified AI models.

See ROADMAP.md.

Contributing

Contributions are welcome around:

browser media;

WebCodecs;

WebGPU;

ONNX Runtime;

AI model integration;

timeline UX;

performance;

testing;

localization;

accessibility;

documentation;

automation tooling.

Before submitting a change:

npm run check

For contribution guidelines, see:

CONTRIBUTING.md

Useful Commands

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

# Formatting validation
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

01 — Browser as a compute platform

The browser is treated as a serious execution environment rather than merely a presentation layer.

02 — Local-first media

When technically supported, media processing and AI inference should happen close to the user's device.

03 — Structured editing

The timeline is structured, inspectable data.

04 — Deterministic output

Export should be reproducible from the project representation.

05 — Progressive AI

AI features should load when needed instead of forcing every model into the initial application payload.

06 — Graceful degradation

The application should provide fallbacks when browser capabilities, GPU acceleration, or specific model runtimes are unavailable.

07 — Automation-friendly workflows

An editable project representation makes video editing more suitable for programmatic tooling and AI agents.

What Makes the Architecture Different?

The interesting engineering challenge is not simply integrating an AI model.

It is coordinating:

               ┌─────────────┐
               │   React UI  │
               └──────┬──────┘
                      │
               ┌──────▼──────┐
               │   Timeline  │
               └──────┬──────┘
                      │
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
                      │
                      ▼
                   EXPORT

while keeping the application responsive and preserving an editable project model.

That combination makes Timeline Studio as much a browser systems project as it is a video editor.

Demo

Live Editor

https://video-editor.ai-creator.top/

YouTube

https://youtu.be/bqKhpPPa-qo

Hugging Face Space

https://huggingface.co/spaces/haixin/timeline-studio

Interactive Showcase

The repository can also be paired with the included cinematic portfolio showcase page to demonstrate:

the architecture;

the AI pipeline;

the interactive timeline;

local inference;

media processing;

export flow;

recruiter-oriented engineering overview.

Screenshots & Media

Recommended repository presentation:

docs/
└── screenshots/
    ├── editor-timeline.png
    ├── ai-music.png
    ├── ai-repair.png
    ├── captions.png
    ├── smart-framing.png
    └── export.png

For a polished GitHub landing page, place the strongest editor screenshot directly below the project overview and use short GIF/video demonstrations for the most visual AI workflows.

Status

Timeline Studio is an actively developed browser AI media application.

The architecture continues to evolve around:

browser-native AI;

deterministic rendering;

timeline reliability;

media interoperability;

AI-assisted editing;

automation;

local-first workflows.

License

The original Timeline Studio source code is licensed under the MIT License.

Third-party models, weights, datasets, media, fonts, and other assets remain subject to their respective licenses and terms.

See MODEL_LICENSES.md for model-specific licensing information.

<p align="center">

Timeline Studio

Browser-native AI video editing · Local-first inference · Structured timelines · Deterministic media export

</p>
