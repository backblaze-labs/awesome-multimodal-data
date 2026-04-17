# CLAUDE.md — awesome-multimodal-data

## What this list is

A curated directory of multimodal **datasets** and **data tooling**: image-text/video/audio/document corpora, plus the streaming formats, curation libraries, labeling tools, and embedding models that work on them.

## Scope

**Include**
- Public image-text, video, audio, speech, and document datasets.
- Data-loading and streaming formats (WebDataset, MDS, Lance, Parquet streaming).
- Curation and cleaning libraries (dedup, quality filtering, outlier detection).
- Labeling platforms with multimodal support.
- Multimodal embedding models and libraries (CLIP family, SigLIP, Nomic, BGE, FAISS).
- Template pipelines for downloading/building multimodal datasets (img2dataset, video2dataset).

**Exclude**
- Generic ML orchestrators and warehouses — see `awesome-ml-data-pipelines`.
- Pure LLM agent tooling — see `awesome-agent-infrastructure`.
- Robotics datasets/benchmarks — see `awesome-physical-ai`.
- Datasets without a public download or HuggingFace/GitHub mirror.

**Inclusion requirements (every entry)**
- Public download URL or HuggingFace hub page.
- Documentation or paper describing licensing and contents.
- Demonstrated use in real training runs or production pipelines.

## Files, schema, workflow, rules

Identical to the rest of the awesome-* family. See `~/awesome-lists/CLAUDE.md` for the global workflow and `~/awesome-lists/_shared/schema.json` for field definitions.

Per-repo reminders:

- Edit `entries.yaml` only. `README.md` and `llms.txt` are generated.
- For datasets, use the `license` field carefully — many large corpora are redistribution-restricted; note the terms in `description` if non-obvious.
- `b2_integration` is a URL to B2 docs, or `""` if none.
- Never delete an entry; tag `needs-review` and log a note in `~/awesome-lists/_tasks/`.
