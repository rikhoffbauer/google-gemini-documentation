# Gemini Models

This document provides an overview of the Gemini models available through the
Gemini API.

# Model Variants

The Gemini API offers a range of models optimized for various use cases. Here's a
summary of the available Gemini variants:

| Model variant | Input(s) | Output | Optimized for |
| --- | --- | --- | --- |
| Gemini 2.5 Pro | Audio, images, videos, text, and PDF | Text | Enhanced thinking and reasoning, multimodal understanding, advanced coding, and more |
| Gemini 2.5 Flash | Audio, images, videos, and text | Text | Adaptive thinking, cost efficiency |
| Gemini 2.5 Flash-Lite | Text, image, video, audio | Text | Most cost-efficient model supporting high throughput |
| Gemini 2.5 Flash Live | Audio, video, and text | Text, audio | Low-latency bidirectional voice and video interactions |
| Gemini 2.5 Flash Native Audio | Audio, videos, and text | Text and audio, interleaved | High quality, natural conversational audio outputs, with or without thinking |
| Gemini 2.5 Flash Preview TTS | Text | Audio | Low latency, controllable, single- and multi-speaker text-to-speech audio generation |
| Gemini 2.5 Pro Preview TTS | Text | Audio | Low latency, controllable, single- and multi-speaker text-to-speech audio generation |
| Gemini 2.0 Flash | Audio, images, videos, and text | Text | Next generation features, speed, and realtime streaming. |
| Gemini 2.0 Flash Preview Image Generation | Audio, images, videos, and text | Text, images | Conversational image generation and editing |
| Gemini 2.0 Flash-Lite | Audio, images, videos, and text | Text | Cost efficiency and low latency |
| Gemini 2.0 Flash Live | Audio, video, and text | Text, audio | Low-latency bidirectional voice and video interactions |
| Gemini 1.5 Flash | Audio, images, videos, and text | Text | Fast and versatile performance across a diverse variety of tasks |
| Gemini 1.5 Flash-8B | Audio, images, videos, and text | Text | High volume and lower intelligence tasks |
| Gemini 1.5 Pro | Audio, images, videos, and text | Text | Complex reasoning tasks requiring more intelligence |

You can find the rate limits for each model on the rate limits page.

## Gemini 2.5 Pro

Gemini 2.5 Pro is a state-of-the-art thinking model, capable of reasoning
over complex problems in code, math, and STEM, as well as analyzing large
datasets, codebases, and documents using long context.

## Gemini 2.5 Flash

Gemini 2.5 Flash is a price-performance model, offering well-rounded
capabilities. It is best for large scale processing, low-latency, high volume
tasks that require thinking, and agentic use cases.

## Gemini 2.5 Flash-Lite

Gemini 2.5 Flash-Lite is a model optimized for cost-efficiency and high
throughput.

## Gemini 2.5 Flash Live

The Gemini 2.5 Flash Live model works with the Live API to enable low-latency
bidirectional voice and video interactions with Gemini.

## Gemini 2.5 Flash Native Audio

These native audio dialog models, with and without thinking, are available
through the Live API. They provide interactive and unstructured conversational
experiences, with style and control prompting.

## Gemini 2.5 Flash Preview Text-to-Speech

Gemini 2.5 Flash Preview TTS is a price-performant text-to-speech model,
delivering high control and transparency for structured workflows like podcast
generation, audiobooks, customer support, and more.

## Gemini 2.5 Pro Preview Text-to-Speech

Gemini 2.5 Pro Preview TTS is a powerful text-to-speech model, delivering high
control and transparency for structured workflows.

## Gemini 2.0 Flash

Gemini 2.0 Flash delivers next-gen features and improved capabilities, including
superior speed, native tool use, and a 1M token context window.

## Gemini 2.0 Flash Preview Image Generation

This model delivers improved image generation features, including generating and
editing images conversationally.

## Gemini 2.0 Flash-Lite

A Gemini 2.0 Flash model optimized for cost efficiency and low latency.

## Gemini 2.0 Flash Live

The Gemini 2.0 Flash Live model works with the Live API to enable low-latency
bidirectional voice and video interactions with Gemini.

## Gemini 1.5 Flash

Gemini 1.5 Flash is a fast and versatile multimodal model for scaling across
diverse tasks.

## Gemini 1.5 Flash-8B

Gemini 1.5 Flash-8B is a small model designed for lower intelligence tasks.

## Gemini 1.5 Pro

Gemini 1.5 Pro is a mid-size multimodal model that is optimized for a wide-range
of reasoning tasks. It can process large amounts of data at once, including 2
hours of video, 19 hours of audio, codebases with 60,000 lines of code, or
2,000 pages of text.

# Model Version Name Patterns

Gemini models are available in stable, preview, or experimental versions. You
can use the following model name formats to specify which model and version you
want to use:

  * **Latest stable:** Points to the most recent stable version released for the
    specified model generation and variation.
  * **Stable:** Points to a specific stable model. Stable models usually don't
    change.
  * **Preview:** Points to a preview model which may not be suitable for
    production use, come with more restrictive rate limits, but may have
    billing enabled.
  * **Experimental:** Points to an experimental model which may not be suitable
    for production use and come with more restrictive rate limits.

## Supported Languages

Gemini models are trained to work with a wide variety of languages, including
Arabic, Chinese, English, French, German, Japanese, Russian, and Spanish.