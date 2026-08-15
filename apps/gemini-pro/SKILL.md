---
name: gemini-pro
description: >
  Multimodal content generation platform powered by Gemini Pro 2's vision, audio, 
  and video capabilities. Routes through 8 specialized sub-skills for image 
  understanding, video analysis, audio processing, and cross-modal synthesis. 
  Optimized for rich media workflows and multimodal AI applications.
license: MIT
compatibility: Requires Claude Code and Python 3.11+; Google Gemini API credentials
metadata:
  author: @edoneoo
  version: "1.0.0"
  model: gemini-2.0-pro
user-invokable: true
argument-hint: "[image|video|audio|analyze|generate|synthesize|extract|translate-media]"
---

# Gemini Pro 2: Multimodal Content Generation

Full-lifecycle multimodal platform: image analysis & generation, video understanding, audio processing, 
and cross-modal synthesis. Leverages vision, audio, and language models for rich media workflows.

## Quick Reference

| Command | What it does |
|---------|-------------|
| `/gemini image <file>` | Analyze image with detailed understanding |
| `/gemini video <file>` | Extract key frames & analyze video content |
| `/gemini audio <file>` | Transcribe & analyze audio |
| `/gemini analyze <media>` | Multi-modal content analysis |
| `/gemini generate <prompt>` | Generate images with text guidance |
| `/gemini synthesize <inputs>` | Combine multiple media types |
| `/gemini extract <media>` | Extract text/data from media |
| `/gemini translate-media <file>` | Translate across modalities |

## Core Architecture

**8 Sub-Skills:**
- `gemini-image` - Image analysis & understanding
- `gemini-video` - Video processing & key frame extraction
- `gemini-audio` - Audio transcription & analysis
- `gemini-analyze` - Multi-modal analysis coordination
- `gemini-generate` - Image generation from text
- `gemini-synthesize` - Cross-modal synthesis
- `gemini-extract` - Data extraction from media
- `gemini-translate-media` - Modality translation

**5 Specialized Agents:**
- `gemini-vision` - Image understanding expert
- `gemini-videographer` - Video analysis specialist
- `gemini-acoustician` - Audio processing expert
- `gemini-synthesizer` - Multi-modal synthesis specialist
- `gemini-extractor` - Data extraction expert

## 5-Gate Delivery Contract for Multimodal Content

| Gate | Enforces | Implementation |
|---|---|---|
| 1. Media Validation | Media files readable & valid | `scripts/gemini_validate_media.py --gate 1` |
| 2. Analysis Completeness | All modalities processed | `scripts/gemini_check_completeness.py` |
| 3. Quality Check | Output quality meets standards | `scripts/gemini_check_quality.py` |
| 4. Content Review | AI-generated content appropriate | `agents/gemini-vision.md` |
| 5. Integration Test | Output integrates with context | `scripts/gemini_validate_output.py` |

## Quality Scoring (100 points)

| Category | Points | Focus |
|---|---:|---|
| Analysis Accuracy | 25 | Correctness of interpretation |
| Completeness | 20 | Coverage of all modalities |
| Synthesis Quality | 20 | Integration across modalities |
| Technical Quality | 20 | Media quality & processing |
| Relevance | 15 | Fitness for intended use |

## Execution Flow

1. **Validate** - Check media formats & integrity
2. **Analyze** - Spawn appropriate specialist agents
3. **Extract** - Pull data/insights from media
4. **Synthesize** - Combine multi-modal insights
5. **Generate** - Create output based on synthesis
6. **Review** - Run 5-gate delivery contract
7. **Deliver** - Output with confidence scores

## Supported Media Types

**Images:**
- JPEG, PNG, GIF, WebP, TIFF, BMP
- Resolution: Up to 4K
- Processing: Object detection, OCR, scene understanding

**Video:**
- MP4, MOV, AVI, WebM, MKV
- Duration: Up to 2 hours
- Processing: Frame extraction, scene detection, motion analysis

**Audio:**
- MP3, WAV, OGG, M4A, FLAC
- Duration: Up to 1 hour
- Processing: Transcription, speaker identification, emotion detection

## Integration Points

- Image APIs: Google Vision, OpenAI Vision
- Video APIs: YouTube API, Vimeo API
- Audio APIs: Google Speech-to-Text, assembly.ai
- Media storage: Google Cloud Storage, AWS S3
- CDN delivery: Cloudflare, Google Cloud CDN

## Anti-Patterns (Never Do These)

| Anti-Pattern | Why |
|-------------|-----|
| Process corrupted media without validation | Results in failed analysis |
| Mix different quality levels in synthesis | Undermines output quality |
| Ignore metadata in media files | Loses context & authenticity info |
| Generate content without source attribution | Violates copyright & ethics |
| Over-compress media before processing | Loses critical visual details |
