# 🇺🇿 Awesome Uzbek NLP [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of resources for Natural Language Processing (NLP) in the Uzbek language — datasets, pretrained models, tools, papers, and community links.

**Contributions welcome!** If you know a resource that should be here, please open a PR. 🙌

---

## 📚 Table of Contents

- [📊 Datasets](#-datasets)
  - [Speech / Audio](#speech--audio)
  - [Text Corpora](#text-corpora)
  - [Task-Specific](#task-specific)
- [🤖 Pretrained Models](#-pretrained-models)
  - [Language Models](#language-models)
  - [Speech Models (ASR / TTS)](#speech-models-asr--tts)
  - [Translation Models](#translation-models)
- [🛠️ Tools & Libraries](#️-tools--libraries)
- [📄 Papers](#-papers)
- [🌐 Useful Links](#-useful-links)
- [👥 Community & People](#-community--people)
- [🤝 Contributing](#-contributing)

---

## 📊 Datasets

### Speech / Audio

| Dataset | Description | Size | License |
|---------|-------------|------|---------|
| [Uzbek Speech Corpus (USC)](https://huggingface.co/datasets/issai/Uzbek_Speech_Corpus) | Open-source ASR corpus, manually verified by native speakers (958 speakers) | 105 hours | CC BY 4.0 |
| [Mozilla Common Voice (Uzbek)](https://commonvoice.mozilla.org/uz/datasets) | Community-contributed Uzbek speech recordings | Growing | CC0 |
| [Google FLEURS (Uzbek)](https://huggingface.co/datasets/google/fleurs) | Few-shot learning evaluation benchmark for Uzbek speech | ~12 hours | CC BY 4.0 |
| [IT Uzbek Speech Dataset](https://huggingface.co/datasets/islomov/it_youtube_uzbek_speech_dataset) | IT-domain speech from Uzbek YouTube channels, transcribed with Gemini 2.5 Pro | — | Apache 2.0 |
| [News Uzbek Speech Dataset](https://huggingface.co/datasets/islomov/news_youtube_uzbek_speech_dataset) | News-domain speech from Uzbek YouTube channels (Kunuz, Qalampir), various dialects | — | Apache 2.0 |

### Text Corpora

| Dataset | Description | License |
|---------|-------------|---------|
| [Uzbek Wikipedia Dump](https://dumps.wikimedia.org/uzwiki/) | Full Uzbek Wikipedia text dump | CC BY-SA |
| [OSCAR (Uzbek subset)](https://huggingface.co/datasets/oscar-corpus/OSCAR-2301) | Uzbek web text extracted from Common Crawl | CC0 |
| [CC-100 (Uzbek)](https://data.statmt.org/cc-100/) | Uzbek monolingual data from Common Crawl | — |
| [15GB Uzbek Text Corpus + BPE Tokenizer](https://github.com/topics/uzbek-tokenizer) | Cleaned 15GB Uzbek text with Cyrillic removal + trained Byte-Level BPE tokenizer | — |

### Task-Specific

| Dataset | Task | Description |
|---------|------|-------------|
| [Uzbek Text Classification Dataset](https://arxiv.org/abs/2302.14494) | Text Classification | 15 categories from 10 news/press sites; used in BERTbek evaluation |
| [Uzbek NER Dataset](https://pubmed.ncbi.nlm.nih.gov/38708296/) | Named Entity Recognition | Comprehensive NER dataset (2024, Data in Brief journal) |
| [Uzbek-Kazakh Parallel Corpus](https://www.sciencedirect.com/science/article/pii/S2352340924001653) | Machine Translation | Uzbek↔Kazakh parallel texts on HuggingFace |
| [Aspect-Based Sentiment (Uzbek)](https://huggingface.co/datasets/Sanatbek/aspect-based-sentiment-analysis-uzbek) | Sentiment Analysis | Aspect-level sentiment dataset for Uzbek |
| [Universal Dependencies (Uzbek)](https://universaldependencies.org/) | POS Tagging / Dependency Parsing | Uzbek treebank |

---

## 🤖 Pretrained Models

### Language Models

| Model | Description | Link |
|-------|-------------|------|
| **BERTbek** | BERT-based model trained on Uzbek corpus; SOTA on sentiment, NER, topic classification | [HuggingFace](https://huggingface.co/models?language=uz&sort=downloads) |
| **UzBERT** | BERT model trained on Uzbek Wikipedia + news | [HuggingFace](https://huggingface.co/models?language=uz) |
| **mGPT-1.3B (Uzbek)** | GPT model fine-tuned on Uzbek by ai-forever; 50k additional steps on A100 | [HuggingFace](https://huggingface.co/ai-forever/mGPT-1.3B-uzbek) |
| **mBERT** | Multilingual BERT with Uzbek support | [HuggingFace](https://huggingface.co/bert-base-multilingual-cased) |
| **XLM-RoBERTa** | Multilingual RoBERTa with strong Uzbek support | [HuggingFace](https://huggingface.co/xlm-roberta-base) |

### Speech Models (ASR / TTS)

| Model | Task | Description | Link |
|-------|------|-------------|------|
| **USC ASR Model** | ASR | Trained on Uzbek Speech Corpus | [GitHub](https://github.com/IS2AI/Uzbek_ASR) |
| **Whisper (Uzbek)** | ASR | OpenAI Whisper large-v3 with Uzbek support | [HuggingFace](https://huggingface.co/openai/whisper-large-v3) |
| **MMS (Uzbek)** | ASR + TTS | Meta's Massively Multilingual Speech — includes Uzbek | [HuggingFace](https://huggingface.co/facebook/mms-1b-all) |
| **uzbek-stt-3** | ASR | Fine-tuned on legal and military Uzbek text | [HuggingFace](https://huggingface.co/sarahai/uzbek-stt-3) |

### Translation Models

| Model | Direction | Link |
|-------|-----------|------|
| **Helsinki-NLP** | uz↔en, uz↔ru | [HuggingFace](https://huggingface.co/Helsinki-NLP) |
| **NLLB-200** | 200 languages including Uzbek | [HuggingFace](https://huggingface.co/facebook/nllb-200-distilled-600M) |

---

## 🛠️ Tools & Libraries

| Tool | Description | Link |
|------|-------------|------|
| **Uzbek Hunspell Dictionary** | Spell checker + morphological analyzer (Hunspell format). Supports lemmatization. Funded by MUNIS project 2022–2024 | [Website](https://uzbek-spell.github.io/) |
| **Uzbek Morphological Analyser** | Morphology analyzer based on affixes (stemmer + lemmatizer) | [GitHub](https://github.com/topics/morphological-analyser?q=uzbek) |
| **uzbek-tokenizers** | Various NLTK-based tokenizers for Uzbek | [GitHub](https://github.com/coppercitylabs/uzbek-tokenizers) |
| **Tahrirchi** | Spell-checker keyboard for Android (Uzbek); FST-based morphology in C++ | [GitHub](https://github.com/topics/uzbek) |
| **HuggingFace Transformers** | General NLP library with support for Uzbek models | [GitHub](https://github.com/huggingface/transformers) |

---

## 📄 Papers

| Year | Paper | Link |
|------|-------|------|
| 2021 | **USC: An Open-Source Uzbek Speech Corpus and Initial Speech Recognition Experiments** — First open Uzbek ASR corpus (105h, 958 speakers) | [[arXiv]](https://arxiv.org/abs/2107.14419) [[GitHub]](https://github.com/IS2AI/Uzbek_ASR) |
| 2023 | **Text Classification Dataset and Analysis for Uzbek Language** — 15-category classification; BERTbek achieves best results | [[arXiv]](https://arxiv.org/abs/2302.14494) |
| 2024 | **BERTbek: A Pretrained Language Model for Uzbek** — BERT model evaluated on NER, sentiment, topic classification | [[ACL Anthology]](https://aclanthology.org/2024.sigul-1.5.pdf) |
| 2024 | **Parallel Texts Dataset for Uzbek–Kazakh Machine Translation** — Parallel corpus for low-resource Turkic MT | [[ScienceDirect]](https://www.sciencedirect.com/science/article/pii/S2352340924001653) |
| 2024 | **Comprehensive NER Dataset and Neural Network for Uzbek** — NER dataset with neural approach | [[PubMed]](https://pubmed.ncbi.nlm.nih.gov/38708296/) |
| 2024 | **Recent Advancements in Turkic Central Asian Language Processing** — Survey including Uzbek NLP | [[arXiv]](https://arxiv.org/abs/2407.05006) |
| 2025 | **BBPOS: BERT-based POS Tagging for Uzbek** — First neural POS tagger for Uzbek | [[arXiv]](https://arxiv.org/pdf/2501.10107) |

---

## 🌐 Useful Links

- [HuggingFace — Uzbek models](https://huggingface.co/models?language=uz)
- [HuggingFace — Uzbek datasets](https://huggingface.co/datasets?language=uz)
- [Kaggle — Uzbek datasets](https://www.kaggle.com/search?q=uzbek)
- [OpenSLR — Speech resources](https://www.openslr.org/)
- [Universal Dependencies — Uzbek](https://universaldependencies.org/)
- [Mozilla Common Voice — Uzbek](https://commonvoice.mozilla.org/uz)
- [Uzbek NLP blog post (stemmer)](https://ahikmat.blogspot.com/2016/05/nlp-for-uzbek-language.html)

---

## 👥 Community & People

Uzbek NLP bilan shug'ullanayotgan tadqiqotchilar va tashkilotlar:

- **[ISSAI](https://github.com/IS2AI)** — Uzbek ASR, speech datasets (Nazarbayev University)
- **[TUIT](https://tuit.uz/)** — Tashkent University of IT — Uzbek language processing research
- **[Aiphoria](https://medium.com/aiphoria)** — Uzbek LLM fine-tuning for banking/production
- **[uzbek-spell](https://uzbek-spell.github.io/)** — Hunspell dictionary team (MUNIS project, TSUE)
- **AI Uzbekistan** — Local ML/AI community

---

## 🤝 Contributing

Yangi resurs topdingizmi? PR oching yoki Issue yozing!

1. Fork this repo
2. Add your resource to the relevant section
3. Submit a Pull Request

Please follow the existing format and make sure links are working. ✅

### Contribution Guidelines
- Resources should be freely accessible (open-source or freely available)
- Links must be working and pointing to original sources
- Descriptions should be in English (resource names can be in Uzbek)
- Prefer HuggingFace, GitHub, arXiv, and official academic sources

---

## ⭐ Star History

Agar bu repo foydali bo'lsa, **star bosing** — bu Uzbek NLP rivojiga hissa qo'shadi! 🇺🇿

---

*Made with ❤️ by [Baxrom Abdusalomov](https://github.com/Abdusalom0v) — a student from Uzbekistan passionate about AI & NLP.*
