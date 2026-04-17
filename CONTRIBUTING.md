# Contributing

Thanks for your interest in contributing. This list covers multimodal datasets and the tooling that operates on them.

## How to contribute

1. Fork this repo.
2. Edit **`entries.yaml`** only. Do not edit `README.md` or `llms.txt` — those are regenerated.
3. Place your entry in the appropriate category (see `categories.yaml`).
4. Open a PR. One entry per PR.

## What belongs in the list

**We accept**
- Public image-text, video, audio, speech, and document datasets.
- Data-loading and streaming formats suited to multimodal training.
- Curation, cleaning, dedup, and labeling tools.
- Multimodal embedding models and indexing libraries.
- Pipelines/templates for building multimodal datasets.

**We don't accept**
- Datasets without a public download or Hub mirror.
- Tools whose only contribution is a thin wrapper around another library.
- Generic ML tooling (see `awesome-ml-data-pipelines`).
- Robotics data (see `awesome-physical-ai`).

## Inclusion requirements

- Public download URL or HuggingFace hub page.
- Documentation or paper describing licensing and contents.
- Actual usage in training runs or production pipelines.

## Entry format

```yaml
- name: WebDataset
  url: https://github.com/webdataset/webdataset
  docs_url: https://webdataset.github.io/webdataset/
  description: PyTorch dataset format packaging samples as tar shards.
  category: data-loading-and-streaming
  github: webdataset/webdataset
  license: BSD-3-Clause
  sdks:
    - {language: Python (pip install webdataset)}
  b2_integration: ""
  last_verified: 2026-04-17
```

Field reference is identical across all awesome-* lists in this family.

## Code of conduct

This project follows standard open-source community norms. Be kind, be constructive, focus on the contribution.
