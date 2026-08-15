---
name: notebooklm
description: >
  Document-grounded Q&A platform powered by Google NotebookLM's research 
  synthesis capabilities. Routes through 6 specialized sub-skills for document 
  processing, knowledge base construction, conversational retrieval, study guide 
  generation, and audio synthesis. Optimized for document-centric workflows and 
  research synthesis.
license: MIT
compatibility: Requires Claude Code and Python 3.11+; Google NotebookLM API
metadata:
  author: @edoneoo
  version: "1.0.0"
  model: notebooklm-premium
user-invokable: true
argument-hint: "[process|ask|synthesize|guide|audio|compare]"
---

# NotebookLM: Document-Grounded Q&A & Synthesis

Full-lifecycle document intelligence platform: multi-document ingestion, knowledge base construction, 
conversational Q&A with grounding, study guide generation, audio podcast synthesis, and cross-document 
analysis. Leverages Google's document understanding for research synthesis.

## Quick Reference

| Command | What it does |
|---------|-------------|
| `/notebooklm process <files>` | Ingest & process documents |
| `/notebooklm ask <question>` | Document-grounded Q&A |
| `/notebooklm synthesize <topic>` | Cross-document synthesis |
| `/notebooklm guide <subject>` | Generate study guide from documents |
| `/notebooklm audio <format>` | Generate audio podcast from documents |
| `/notebooklm compare <documents>` | Cross-document comparison |

## Core Architecture

**6 Sub-Skills:**
- `notebooklm-process` - Document ingestion & processing
- `notebooklm-ask` - Conversational Q&A with grounding
- `notebooklm-synthesize` - Cross-document synthesis
- `notebooklm-guide` - Study guide generation
- `notebooklm-audio` - Audio synthesis (podcasts)
- `notebooklm-compare` - Document comparison

**5 Specialized Agents:**
- `notebooklm-processor` - Document processing expert
- `notebooklm-qa` - Q&A specialist
- `notebooklm-synthesizer` - Synthesis expert
- `notebooklm-educator` - Study guide expert
- `notebooklm-podcaster` - Audio synthesis specialist

## 5-Gate Delivery Contract for Document Intelligence

| Gate | Enforces | Implementation |
|---|---|---|
| 1. Document Validation | All documents processed | `scripts/notebooklm_validate_docs.py --gate 1` |
| 2. Grounding Verification | Answers grounded in docs | `scripts/notebooklm_verify_grounding.py` |
| 3. Completeness Check | All documents covered | `scripts/notebooklm_check_coverage.py` |
| 4. Quality Review | Synthesis quality verified | `agents/notebooklm-synthesizer.md` |
| 5. Integration Test | Output integrates properly | `scripts/notebooklm_validate_output.py` |

## Quality Scoring (100 points)

| Category | Points | Focus |
|---|---:|---|
| Grounding Accuracy | 25 | Answers backed by source docs |
| Coverage | 20 | All key documents utilized |
| Synthesis Quality | 20 | Coherent cross-document synthesis |
| Clarity | 20 | Clear & well-organized output |
| Relevance | 15 | Fitness for intended use |

## Execution Flow

1. **Ingest** - Spawn `notebooklm-processor` for document processing
2. **Index** - Build knowledge base from documents
3. **Ground** - Map queries to source documents
4. **Synthesize** - Combine relevant passages
5. **Generate** - Create output (Q&A, guide, or audio)
6. **Review** - Run 5-gate delivery contract
7. **Deliver** - Output with source citations

## Supported Document Types

- **Text**: PDF, DOCX, TXT, Markdown
- **Presentations**: PPTX, Google Slides
- **Spreadsheets**: XLSX, CSV, Google Sheets
- **Academic**: Research papers, theses
- **Web**: HTML, web articles
- **Audio**: Transcripts, podcast transcriptions

## Features

**Knowledge Base:**
- Multi-document indexing (up to 100 documents)
- Semantic search & retrieval
- Document cross-referencing
- Automatic citation tracking

**Q&A:**
- Conversational interface
- Multi-turn dialogue
- Source attribution
- Confidence scoring

**Study Guides:**
- Automatic outline generation
- Key concept extraction
- Quiz generation
- Flashcard creation

**Audio Synthesis:**
- Podcast generation (2 speakers or solo)
- Custom narration styles
- Chapter-based separation
- Video clip support

## Integration Points

- Document storage: Google Drive, Dropbox, OneDrive
- File processing: Google Docs API, PDF processors
- Audio APIs: Google Text-to-Speech, ElevenLabs
- Citation management: BibTeX, RIS, Zotero

## Anti-Patterns (Never Do These)

| Anti-Pattern | Why |
|-------------|-----|
| Ingest documents without preprocessing | Poor indexing & retrieval |
| Ignore citation sources | Loses document grounding |
| Mix document domains without context | Confused synthesis across domains |
| Generate without source attribution | Violates research integrity |
| Over-summarize documents | Loses critical details |
