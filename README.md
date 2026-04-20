# Awesome Multimodal Data [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com) [![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

A curated list of multimodal datasets and data tooling — image-text, video, audio, and document corpora, plus streaming, curation, labeling, and embedding libraries that operate on them.

Maintained by [Backblaze](https://www.backblaze.com).

### Related Lists

- [Awesome ML Data Pipelines](https://github.com/backblaze-labs/awesome-ml-data-pipelines)
- [Awesome Agent Infrastructure](https://github.com/backblaze-labs/awesome-agent-infrastructure)
- [Awesome Physical AI](https://github.com/backblaze-labs/awesome-physical-ai)
- [Awesome Image Generation](https://github.com/backblaze-labs/awesome-image-generation)
- [Awesome Video Generation](https://github.com/backblaze-labs/awesome-video-generation)
- [Awesome Audio Generation](https://github.com/backblaze-labs/awesome-audio-generation)

## Contents

- [Image-Text Datasets](#image-text-datasets)
- [Video Datasets](#video-datasets)
- [Audio and Speech Datasets](#audio-and-speech-datasets)
- [Document and Text Datasets](#document-and-text-datasets)
- [Data Loading and Streaming](#data-loading-and-streaming)
- [Data Curation and Labeling](#data-curation-and-labeling)
- [Embedding and Indexing Models](#embedding-and-indexing-models)
- [Templates and Example Projects](#templates-and-example-projects)

---

## Image-Text Datasets

> Large-scale image-caption corpora for contrastive and generative training.

- **[COYO-700M](https://github.com/kakaobrain/coyo-dataset)** – 747M curated image-alt-text pairs from Kakao Brain. Alternative to LAION for pretraining multimodal models.
- **[DataComp](https://www.datacomp.ai)** – Benchmark and toolkit for building image-text datasets. DataComp-1B is the reference filtered training set. [Docs](https://github.com/mlfoundations/datacomp)
- **[Conceptual Captions 12M](https://github.com/google-research-datasets/conceptual-12m)** – 12M image-text pairs from Google, harvested from alt-text with automated cleaning. Widely used as a CLIP baseline.
- **[Cambrian-10M](https://huggingface.co/datasets/nyu-visionx/Cambrian-10M)** – 10M multimodal instruction-tuning samples from NYU VisionX. Combines VQA, OCR, knowledge-based, and GPT-generated data. Backbone for Cambrian-1 VLM training. Apache-2.0. [Docs](https://cambrian-mllm.github.io/)
- **[LAION-5B](https://laion.ai/blog/laion-5b/)** – 5.85B image-text pairs scraped from Common Crawl. Foundation dataset for Stable Diffusion and many open CLIP models. [Docs](https://huggingface.co/datasets/laion/laion2B-en)
- **[Nemotron-VLM-Dataset-v2](https://huggingface.co/datasets/nvidia/Nemotron-VLM-Dataset-v2)** – NVIDIA's 8M-sample VLM training set spanning image QA, OCR (10 languages), video QA, and chain-of-thought reasoning. Used to train Nemotron Nano 2 VL. CC-BY-4.0. [Docs](https://huggingface.co/blog/nvidia/nemotron-vlm-dataset-v2)
- **[OBELICS](https://huggingface.co/datasets/HuggingFaceM4/OBELICS)** – 141M interleaved image-text web documents, 353M images, 115B tokens, extracted from Common Crawl. Training data for IDEFICS. CC-BY-4.0. [Docs](https://github.com/huggingface/OBELICS)
- **[PixelProse / Docmatix](https://huggingface.co/datasets/HuggingFaceM4/Docmatix)** – Large-scale document-image instruction dataset from HuggingFace. Useful for training multimodal document-QA models.
- **[ReCap-DataComp-1B](https://huggingface.co/datasets/UCSC-VLAA/Recap-DataComp-1B)** – 1.3B DataComp-1B images recaptioned with LLaVA-1.5-LLaMA3-8B. Longer, more detailed captions improve CLIP and text-to-image training. ICML 2025. [Docs](https://github.com/UCSC-VLAA/Recap-DataComp-1B)

## Video Datasets

> Public video datasets with captions, action labels, or instruction annotations.

- **[Panda-70M](https://snap-research.github.io/Panda-70M/)** – 70M high-quality short video clips with automatically generated captions. Used in several video LLM pretraining runs. [Docs](https://github.com/snap-research/Panda-70M)
- **[WebVid-10M](https://github.com/m-bain/webvid)** – 10M weakly-captioned web videos. Common pretraining corpus for text-to-video and video-language models.
- **[Ego4D](https://ego4d-data.org)** – 3,670 hours of first-person video from 931 participants across 9 countries. Benchmarks for social, hands, memory, forecasting. [Docs](https://ego4d-data.org/docs/)
- **[HowTo100M](https://www.di.ens.fr/willow/research/howto100m/)** – 136M narrated instructional video clips from 1.22M YouTube videos. A staple for video-language pretraining. [Docs](https://github.com/antoine77340/howto100m)
- **[InternVid](https://huggingface.co/datasets/OpenGVLab/InternVid)** – 7M videos (~234M clips) with rich captions. Part of the InternVideo foundation-model release. [Docs](https://github.com/OpenGVLab/InternVideo)
- **[OpenVid-1M](https://huggingface.co/datasets/nkp37/OpenVid-1M)** – 1M curated text-video pairs with aesthetic/motion/consistency scores. Includes OpenVidHD-0.4M subset at 1080p. ICLR 2025. [Docs](https://github.com/NJU-PCALab/OpenVid-1M)
- **[PE-Video](https://huggingface.co/datasets/facebook/PE-Video)** – Meta's 1M diverse short videos with text descriptions and 120K human-verified captions. Released with Perception Encoder (2025). CC BY NC 4.0. [Docs](https://github.com/facebookresearch/perception_models)

## Audio and Speech Datasets

> Public speech, music, and sound-event corpora for training and evaluation.

- **[Mozilla Common Voice](https://commonvoice.mozilla.org)** – Open speech corpus built from community contributions. 100+ languages and growing. [Docs](https://commonvoice.mozilla.org/en/datasets)
- **[AudioSet](https://research.google.com/audioset/)** – Google's 2M+ human-labelled 10-second sound clips across 632 classes. Standard corpus for sound-event classification.
- **[CapSpeech](https://huggingface.co/datasets/OpenSound/CapSpeech)** – 10M+ machine-annotated and 360k human-annotated audio-caption pairs for style-captioned TTS. Covers accent, emotion, sound effects, and agent speech tasks. CC-BY-NC-4.0. [Docs](https://github.com/WangHelin1997/CapSpeech)
- **[Emilia](https://huggingface.co/datasets/amphion/Emilia-Dataset)** – 100k+ hours of multilingual, in-the-wild speech data from the Amphion team. Backbone for modern open TTS training. [Docs](https://github.com/open-mmlab/Amphion)
- **[LibriSpeech](https://www.openslr.org/12)** – 1,000-hour English speech corpus derived from LibriVox. The long-running default ASR benchmark.
- **[WavCaps](https://huggingface.co/datasets/cvssp/WavCaps)** – 400k weakly-labelled audio clips with ChatGPT-generated captions from FreeSound, BBC Sound Effects, and AudioSet. Academic use only. [Docs](https://github.com/XinhaoMei/WavCaps)

## Document and Text Datasets

> Large-scale web, code, and document corpora used to pretrain multimodal models.

- **[Dolma](https://github.com/allenai/dolma)** – AI2's 3T-token open pretraining corpus with a transparent pipeline. Backbone for OLMo training.
- **[BigDocs-7.5M](https://huggingface.co/datasets/ServiceNow/BigDocs-7.5M)** – 7.5M permissively licensed document image-text pairs from ServiceNow. Covers OCR, structured parsing, captioning, and QA across scientific papers, tables, and UI screenshots. ICLR 2025. CC-BY-4.0. [Docs](https://bigdocs.github.io/)
- **[Common Corpus](https://huggingface.co/blog/Pclanglais/common-corpus)** – 2T-token fully open text corpus from PleIAs. Public-domain and permissive text only — usable for commercial training. [Docs](https://huggingface.co/collections/PleIAs/common-corpus-65d46e3ea3980fdcd66a5613)
- **[DCLM-Baseline](https://huggingface.co/datasets/mlfoundations/dclm-baseline-1.0)** – 4T-token filtered web corpus from 240T-token Common Crawl pool. Trains 7B models to 64% MMLU at 2.6T tokens. NeurIPS 2024. [Docs](https://github.com/mlfoundations/dclm)
- **[FineWeb / FineWeb-Edu](https://huggingface.co/datasets/HuggingFaceFW/fineweb)** – 15T high-quality English tokens filtered from 96 Common Crawl dumps. Edu variant is ~1.3T educational-content tokens. [Docs](https://huggingface.co/blog/fineweb)
- **[The Stack v2](https://huggingface.co/datasets/bigcode/the-stack-v2)** – 3TB of permissively licensed source code across 600+ programming languages. Training data for StarCoder/StarCoder2. [Docs](https://huggingface.co/blog/bigcode-the-stack)

## Data Loading and Streaming

> Formats and libraries for streaming multimodal data from object storage into training jobs.

- **[HuggingFace Datasets](https://huggingface.co/docs/datasets)** – Unified loading, streaming, and processing of thousands of datasets. Native Arrow/Parquet with memory-mapped access. [Docs](https://github.com/huggingface/datasets) | SDK: Python (pip install datasets)
- **[Lance](https://lancedb.github.io/lance/)** – Columnar format designed for ML. 100x faster random access than Parquet, versioned, zero-copy from object storage. [Docs](https://github.com/lancedb/lance) | SDK: Python (pip install pylance), Rust
- **[WebDataset](https://github.com/webdataset/webdataset)** – PyTorch dataset format packaging samples as tar shards. Streams directly from S3-compatible object storage. [Docs](https://webdataset.github.io/webdataset/) | SDK: Python (pip install webdataset)
- **[MosaicML Streaming](https://docs.mosaicml.com/projects/streaming/en/stable/)** – Deterministic, shuffled, resumable streaming of datasets from cloud storage. Shard format: MDS. [Docs](https://github.com/mosaicml/streaming) | SDK: Python (pip install mosaicml-streaming)
- **[Ray Data](https://docs.ray.io/en/latest/data/data.html)** – Distributed data loading and preprocessing inside Ray. Native connectors for Parquet on S3-compatible stores. SDK: Python (pip install 'ray[data]')

## Data Curation and Labeling

> Tools for deduplication, cleaning, filtering, and annotating multimodal datasets.

- **[Label Studio](https://labelstud.io)** – Open-source labeling platform supporting text, image, audio, video, and time-series. [Docs](https://labelstud.io/guide/) | SDK: Python (pip install label-studio-sdk)
- **[CVAT](https://www.cvat.ai)** – Computer vision annotation tool with strong video and 3D support. Originally from Intel, now community-maintained. [Docs](https://docs.cvat.ai)
- **[cleanlab](https://cleanlab.ai)** – Finds label errors, outliers, and dataset issues automatically with confident-learning methods. [Docs](https://docs.cleanlab.ai) | SDK: Python (pip install cleanlab)
- **[FiftyOne](https://voxel51.com/fiftyone)** – Open-source dataset curation and model-evaluation toolkit for CV. Rich UI for exploring image/video datasets. [Docs](https://docs.voxel51.com) | SDK: Python (pip install fiftyone)
- **[Datatrove](https://github.com/huggingface/datatrove)** – HuggingFace's data-processing library for LLM pretraining. Parallel filters, deduplication, tokenization pipelines. SDK: Python (pip install datatrove)
- **[fastdup](https://www.visual-layer.com)** – Unsupervised analysis of large visual datasets. Detects duplicates, outliers, mislabels, and leakage in minutes. [Docs](https://github.com/visual-layer/fastdup) | SDK: Python (pip install fastdup)
- **[Cosmos-Curate](https://github.com/nvidia-cosmos/cosmos-curate)** – NVIDIA's distributed video curation pipeline for world foundation model training. Splits, annotates, filters, and deduplicates video at scale using Ray. Apache-2.0.
- **[NeMo Curator](https://github.com/NVIDIA-NeMo/Curator)** – GPU-accelerated curation toolkit from NVIDIA. Handles text, image, video, and audio at scale using RAPIDS and Ray. Apache-2.0. [Docs](https://docs.nvidia.com/nemo-framework/user-guide/latest/datacuration/index.html) | SDK: Python (pip install nemo-curator)
- **[SemHash](https://github.com/MinishLab/semhash)** – Lightweight multimodal library for semantic deduplication, outlier filtering, and representative sample selection across text, images, and audio. SDK: Python (pip install semhash)

## Embedding and Indexing Models

> Multimodal embedding models and frameworks for building searchable indices.

- **[FAISS](https://github.com/facebookresearch/faiss)** – Meta's library for efficient similarity search of dense vectors. The reference ANN library for research-scale indexing. [Docs](https://faiss.ai) | SDK: Python (pip install faiss-cpu), C++
- **[sentence-transformers](https://www.sbert.net)** – PyTorch framework for training and using dense embedding models. De-facto library for semantic search. [Docs](https://github.com/UKPLab/sentence-transformers) | SDK: Python (pip install sentence-transformers)
- **[OpenCLIP](https://github.com/mlfoundations/open_clip)** – Open-source reproduction of CLIP with many trained checkpoints (including SigLIP and EVA-CLIP variants). SDK: Python (pip install open-clip-torch)
- **[BGE (BAAI General Embedding)](https://github.com/FlagOpen/FlagEmbedding)** – Family of multilingual text embeddings from BAAI. Top performers on MTEB; extended to visual and multimodal variants.
- **[Nomic Embed](https://www.nomic.ai/embed)** – Open multimodal embedding family from Nomic. Nomic Embed Vision pairs with Nomic Embed Text for unified image/text search. [Docs](https://docs.nomic.ai)
- **[MMEB-train](https://huggingface.co/datasets/TIGER-Lab/MMEB-train)** – 2.1M training samples for the Massive Multimodal Embedding Benchmark. Covers visual QA, image retrieval, classification, and grounding across 20 datasets. Apache-2.0.
- **[SigLIP 2](https://huggingface.co/collections/google/siglip2-67b5dcef38c175486e240107)** – Google's sigmoid loss for contrastive image-text pretraining. SigLIP 2 adds multilingual and dense-caption training. [Docs](https://github.com/google-research/big_vision)
- **[VLM2Vec](https://github.com/TIGER-AI-Lab/VLM2Vec)** – Framework for training VLMs as dense embedding models. Ships MMEB-V2 benchmark with 78 tasks across images, videos, and visual documents. [Docs](https://tiger-ai-lab.github.io/VLM2Vec/) | SDK: Python

## Templates and Example Projects

> Reference implementations, demos, and starter projects.

- **[img2dataset](https://github.com/rom1504/img2dataset)** – Fast, resumable tool to turn image-URL lists into WebDataset shards. Routinely used to download LAION-scale datasets. SDK: Python (pip install img2dataset)
- **[video2dataset](https://github.com/iejMac/video2dataset)** – Download, trim, and package large video datasets into WebDataset shards.
- **[DataComp Quickstart](https://github.com/mlfoundations/datacomp#quickstart)** – Reference workflow for downloading, filtering, and training on DataComp. Good starting point for custom filters.

---

## Contributing

Contributions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md). One entry per PR — edit `entries.yaml` only and let the maintainers regenerate `README.md`.

## License

Released under [CC0 1.0 Universal](LICENSE). You may copy, modify, and redistribute without attribution.

## About Backblaze B2

[Backblaze B2 Cloud Storage](https://www.backblaze.com/cloud-storage) is S3-compatible object storage designed for AI and media workloads. This list is maintained as part of our work making B2 a convenient storage layer for AI workflows.
