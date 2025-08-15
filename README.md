---
permalink: /
---
# Gemini API | Google AI for Developers

**ai.google.dev uses cookies from Google to deliver and enhance the quality of its services and to analyze traffic. [Learn more](https://policies.google.com/technologies/cookies).**

[OK, got it]

This repository contains the source code for the community-driven documentation for the Google Gemini API, hosted at [https://rikhoffbauer.github.io/google-gemini-documentation/](https://rikhoffbauer.github.io/google-gemini-documentation/).

## Google AI for Developers

  * Models
    * Gemini
      * [About](models.md)
      * [Docs](overview.md)
      * [API reference](https://ai.google.dev/api)
      * [Pricing](pricing.md)
    * Imagen
      * [About](imagen.md)
      * [Docs](imagen.md)
      * [Pricing](pricing.md)
    * Veo
      * [About](video.md)
      * [Docs](video.md)
      * [Pricing](pricing.md)
    * Gemma
      * [About](https://ai.google.dev/gemma)
      * [Docs](https://ai.google.dev/gemma/docs)
      * [Gemmaverse](https://ai.google.dev/gemma/docs/gemmaverse)
  * Solutions
    * Build with Gemini
      * [Gemini API](overview.md)
      * [Google AI Studio](ai-studio-quickstart.md)
    * Customize Gemma open models
      * [Gemma open models](https://ai.google.dev/gemma)
      * [Multi-framework with Keras](https://ai.google.dev/gemma/docs/keras_gemma)
      * [Fine-tune in Colab](https://ai.google.dev/gemma/docs/fine_tuning)
      * [Run on-device](https://ai.google.dev/edge)
  * Code assistance
    * [Android Studio](https://developer.android.com/studio/preview/gemini)
    * [Chrome DevTools](https://goo.gle/devtools-gemini)
    * [Colab](https://colab.research.google.com/)
    * [Firebase](https://firebase.google.com/docs/genkit)
    * [Google Cloud](https://cloud.google.com/docs/gemini/code-assist)
    * [JetBrains](https://plugins.jetbrains.com/plugin/22648-google-cloud-code)
    * [Jules](https://jules.ai/)
    * [VS Code](https://code.visualstudio.com/docs/editor/artificial-intelligence)
  * Showcase
    * [Gemini Showcase](https://ai.google.dev/showcase)
    * [Gemini API Developer Competition](https://aistudio.google.com/app/competition)
  * Community
    * [Google AI Forum](https://discuss.ai.google.dev/)
    * [Gemini for Research](https://deepmind.google/technologies/gemini/research/)

* * *

### Get a Gemini API Key

Get a Gemini API key and make your first API request in minutes.

**Python**
```python
from google import genai
client = genai.Client()
response = client.models.generate_content(
    model="gemini-2.5-flash",
    contents="Explain how AI works in a few words"
)
print(response.text)
```

**JavaScript**
```javascript
import { GoogleGenAI } from "@google/genai";
const ai = new GoogleGenAI({});
async function main() {
    const response = await ai.models.generateContent({
        model: "gemini-2.5-flash",
        contents: "Explain how AI works in a few words",
    });
    console.log(response.text);
}
await main();
```

**Go**
```go
package main
import (
    "context"
    "fmt"
    "log"
    "google.golang.org/genai"
)
func main() {
    ctx := context.Background()
    client, err := genai.NewClient(ctx, nil)
    if err != nil {
        log.Fatal(err)
    }
    result, err := client.Models.GenerateContent(
        ctx, "gemini-2.5-flash", genai.Text("Explain how AI works in a few words"), nil,
    )
    if err != nil {
        log.Fatal(err)
    }
    fmt.Println(result.Text())
}
```

**Java**
```java
package com.example;
import com.google.genai.Client;
import com.google.genai.types.GenerateContentResponse;
public class GenerateTextFromTextInput {
    public static void main(String[] args) {
        Client client = new Client();
        GenerateContentResponse response = client.models.generateContent(
            "gemini-2.5-flash", "Explain how AI works in a few words", null);
        System.out.println(response.text());
    }
}
```

**REST**
```bash
curl "https://generativelaanguage.googleapis.com/v1beta/models/gemini-2.5-flash:generateContent" \
    -H "x-goog-api-key: $GEMINI_API_KEY" \
    -H 'Content-Type: application/json' \
    -X POST \
    -d '{ "contents": [ { "parts": [ { "text": "Explain how AI works in a few words" } ] } ] }'
```

### Meet the models

  * **2.5 Pro**
Our most powerful thinking model with features for complex reasoning and much more
  * **2.5 Flash**
Our newest multimodal model, with next generation features and improved capabilities
  * **2.5 Flash-Lite**
Our fastest and most cost-efficient multimodal model with great performance for high-frequency tasks
  * **Veo 3**
Our state of the art video generation model
  * **Imagen 4**
Our highest quality image generation model that creates stunning visuals
  * **Gemini Embeddings**
Our first Gemini embedding model, designed for production RAG workflows

### Explore the API

  * **Native Image Generation**
Generate and edit highly contextual images natively with Gemini 2.0 Flash.
  * **Explore long context**
Input millions of tokens to Gemini models and derive understanding from unstructured images, videos, and documents.
  * **Generate structured outputs**
Constrain Gemini to respond with JSON, a structured data format suitable for automated processing.

### Start building with the Gemini API

[Get started](quickstart.md)

Sources:
[1] Gemini API | Google AI for Developers (overview.md)