# Self-Hosted LLMs

This repo contains artifacts that can be used to build and run LLM (Large Language Model) services locally on your laptops using containerization methods.
These containerized LLM services can be used to help developers quickly prototype new LLM based applications, without the need for relying
on any other externally hosted services.

## Introduction to LLMs

A Large Language Model is a type of Artificial Intelligence that is trained on a massive dataset of text and code. This allows the model to learn statistical relationships between words and phrases which in turn allows it to generate text, translate languages, write creative content and answer your questions in an informative way.

Some common LLMs:
* GPT3.5, GPT4
* Gemini
* Llama, Llama2

## Setting up LLMs via Self-Hosting
The discussion surrounding LLMs has evolved, transitioning from "Should we utilize LLMs?" to "Should we opt for a self-hosted solution or rely on a proprietary off-the-shelf alternative?" Depending on your use-case, computational needs and engineering architecture availabilities you can decide whether to self-host your LLM.

Some benefits of self-hosting your LLM are:
* Greater security, privacy, and compliance
* Customization
* Avoid vendor lock-in
* Save computational costs
* Easy to get started for those new to or just starting their journey with LLMs

## Current LLM Use Cases:

There are various applications for LLMs and some of the use cases we are looking into include text generation, speech recognition and RAG applications. Currently, the use cases we have available are:

* [Speech Recognition](#speech-recognition)

### Speech Recognition

We are using the [OpenAI's Whisper model](https://github.com/openai/whisper) for speech recognition. Whisper is a general-purpose speech recognition model. It is trained on a large dataset of diverse audio and is also a multitasking model that can perform multilingual speech recognition, speech translation, and language identification. There are five model sizes, four with English-only versions, offering speed and accuracy tradeoffs:

* tiny
* base
* small
* medium
* large

We are using the compressed `.ggml` model binaries from HuggingFace which can be found here: https://huggingface.co/ggerganov/whisper.cpp.
