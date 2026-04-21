# 02: Azure AI Services (Quiz-Ready)

This note is designed to fully cover Quiz 2 level questions without needing another source.

---

## 1) What Are Azure AI Services?

Azure AI Services are Microsoft's pre-built, cloud-hosted AI APIs and tools. You do not need to build or train models from scratch — you consume them via REST API or SDK.

Key principle for the exam:
- If a scenario says "without ML expertise" or "quickly add AI", the answer is usually an Azure AI Service.
- If a scenario says "custom model on your own data", it may involve Azure Machine Learning.

---

## 2) The Main Azure AI Service Categories

| Category | What It Does | Key Services |
|---|---|---|
| Vision | Analyze images and video | Azure AI Vision, Custom Vision, Face API |
| Speech | Convert speech to text and vice versa | Azure AI Speech |
| Language | Understand and process text | Azure AI Language |
| Decision | Make smart recommendations/decisions | Anomaly Detector, Content Moderator, Personalizer |
| OpenAI | Generative AI on Azure | Azure OpenAI Service |

---

## 3) Azure AI Vision

Provides image analysis without training your own model.

### Capabilities
- **Image Analysis**: detect objects, describe scenes, detect brands/logos
- **OCR (Read API)**: extract printed and handwritten text from images and documents
- **Image Classification**: classify what is in an image
- **Object Detection**: detect and locate multiple objects + bounding boxes
- **Spatial Analysis**: analyze people movement in video in real time
- **Background Removal**: remove backgrounds from images

### Custom Vision
- Use when pre-built image analysis is not specific enough.
- You upload your own labeled images and train a custom classifier or detector.
- No deep ML knowledge needed — portal-based training.

### Face API
- Detect faces in images.
- Identify facial landmarks, emotions, and attributes.
- Face verification and identification.

Exam distinction:
- General image understanding → Azure AI Vision
- Train your own image classifier → Custom Vision
- Face-specific tasks → Face API

---

## 4) Azure AI Speech

### Capabilities

| Feature | What It Does | Example Use |
|---|---|---|
| Speech to Text | Transcribe spoken audio to text | Voice commands, call transcription |
| Text to Speech | Convert text to natural-sounding audio | Accessibility, IVR systems |
| Speech Translation | Translate speech across languages in real time | Multilingual meetings |
| Speaker Recognition | Identify who is speaking | Authentication, call analytics |
| Custom Speech | Fine-tune transcription for domain-specific vocabulary | Medical, legal terminology |

Exam shortcut:
- Any scenario involving audio in or out → Azure AI Speech.

---

## 5) Azure AI Language

Processes and understands text.

### Capabilities

| Feature | What It Does | Example Use |
|---|---|---|
| Sentiment Analysis | Positive/negative/neutral tone | Customer review analysis |
| Key Phrase Extraction | Pull main topics from text | Document summarization |
| Named Entity Recognition (NER) | Identify people, places, dates, organizations | Information extraction |
| Entity Linking | Link entities to known knowledge base entries | Wikipedia-linked entities |
| Language Detection | Identify the language of text | Multi-language intake forms |
| Text Summarization | Condense long documents | News, reports |
| Question Answering | Build FAQ-style QA systems from documents | Support bots |
| Conversational Language Understanding (CLU) | Understand user intent and entities in conversation | Chatbots, virtual agents |
| PII Detection | Detect personally identifiable information | Compliance, data masking |

Exam pattern:
- "Extract key topics from reviews" → Key Phrase Extraction
- "Determine if feedback is positive or negative" → Sentiment Analysis
- "Build a chatbot that understands intent" → CLU (Conversational Language Understanding)
- "Answer questions from a knowledge base" → Question Answering

---

## 6) Azure AI Translator

- Translates text between 100+ languages.
- Part of the Azure AI Language group.
- Real-time text translation, document translation, and custom translation.

Exam distinction:
- Text translation → Azure AI Translator
- Speech translation (spoken audio) → Azure AI Speech (Speech Translation feature)

---

## 7) Azure OpenAI Service

- Access to OpenAI's powerful models (GPT-4, DALL-E, Codex, Whisper) hosted on Azure.
- Adds enterprise security, compliance, and regional availability.

### Models available
| Model | Primary Use |
|---|---|
| GPT-4 / GPT-3.5 | Text generation, summarization, chat |
| DALL-E | Image generation from text prompts |
| Whisper | Speech to text |
| Embeddings | Semantic similarity, search |

### Azure OpenAI Studio / Playground
- Web interface to test and configure models without code.
- Prompt engineering, fine-tuning, and deployment all available.

Exam shortcut:
- Generating text/images/code from prompts → Azure OpenAI Service
- Enterprise-grade generative AI on Azure infrastructure → Azure OpenAI Service

---

## 8) Azure Machine Learning (vs Azure AI Services)

Critical exam distinction:

| | Azure AI Services | Azure Machine Learning |
|---|---|---|
| Expertise needed | Minimal (consume pre-built API) | Data scientist level |
| Custom training | Limited (Custom Vision, Custom Speech) | Full custom training |
| Use case | Adding AI features quickly | Building bespoke ML models |
| Example | Sentiment analysis on text | Training a custom fraud model |

Rule:
- "No ML expertise, add AI to app quickly" → Azure AI Services
- "Build and train own model with own data" → Azure Machine Learning

---

## 9) Azure Cognitive Search (AI-Enriched Search)

- Full-text search with AI enrichment pipeline.
- Can extract text from images (OCR), detect language, extract key phrases from documents.
- Used to make large document stores searchable.

Exam pattern:
- "Make scanned documents searchable" → Cognitive Search with AI enrichment
- "Index content and add AI skills" → Cognitive Search

---

## 10) Content Moderator and Anomaly Detector

### Content Moderator
- Detects potentially offensive, risky, or unwanted content in text and images.
- Used for user-generated content moderation.

### Anomaly Detector
- Detects unusual patterns in time-series data.
- No labeling needed.
- Used for: equipment failure prediction, fraud signals, business metric monitoring.

---

## 11) Personalizer (Decision Service)

- Reinforcement learning-based service to personalize content for users.
- Learns what content to show based on user behavior and rewards.
- Example: personalizing news feed, article ranking, product recommendations.

---

## 12) Azure Bot Service

- Platform to build, test, and deploy intelligent chatbots.
- Integrates with Azure AI Language (CLU, Question Answering) as the AI brain.
- Supports Teams, Web Chat, Facebook Messenger, and more channels.

Exam pattern:
- "Deploy chatbot that understands user questions" → Azure Bot Service + Question Answering
- "Build a bot that understands intents and entities" → Azure Bot Service + CLU

---

## 13) Service Selection Decision Tree

Read the scenario and pick the right service:

```
Is it about images/video?
  → Yes → Azure AI Vision (general) / Custom Vision (custom) / Face API (faces)

Is it about audio/speech?
  → Yes → Azure AI Speech

Is it about text understanding?
  → Yes → Azure AI Language
       → Sentiment? → Sentiment Analysis
       → Topics/keywords? → Key Phrase Extraction
       → Chatbot intents? → CLU
       → FAQ bot? → Question Answering
       → Find names/places? → NER

Is it about text translation?
  → Yes → Azure AI Translator

Is it about generating text/images from prompts?
  → Yes → Azure OpenAI Service

Is it about searching documents with AI?
  → Yes → Azure Cognitive Search

Is it about detecting anomalies in data?
  → Yes → Anomaly Detector

Is it about personalizing user experience?
  → Yes → Personalizer

Is it about chatbots?
  → Yes → Azure Bot Service (+ Language service as AI backend)
```

---

## 14) How Azure AI Services Are Consumed

- All services expose **REST APIs** — send an HTTP request, get a JSON response.
- Also available as **SDKs** for Python, C#, JavaScript, and Java.
- Provisioned as an **Azure resource** in the Azure portal.
- Each resource has an **endpoint URL** and an **API key** for authentication.

---

## 15) One-Page Rapid Revision

- Vision tasks → Azure AI Vision / Custom Vision / Face API
- Speech in/out → Azure AI Speech
- Text understanding → Azure AI Language
- Text translation → Azure AI Translator
- Generative AI → Azure OpenAI Service
- Searchable documents → Cognitive Search
- Anomalies in time data → Anomaly Detector
- Personalized recommendations → Personalizer
- Chatbots → Azure Bot Service
- Quick AI, no expertise → Azure AI Services
- Custom ML model → Azure Machine Learning
- All services = REST API + endpoint + API key

---

## Optional Deep-Dive Citations

- Azure AI Services overview:
  - https://learn.microsoft.com/en-us/azure/ai-services/what-are-ai-services
- Azure AI Vision:
  - https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/overview
- Azure AI Language:
  - https://learn.microsoft.com/en-us/azure/ai-services/language-service/overview
- Azure AI Speech:
  - https://learn.microsoft.com/en-us/azure/ai-services/speech-service/overview
- Azure OpenAI Service:
  - https://learn.microsoft.com/en-us/azure/ai-services/openai/overview
- Azure Machine Learning:
  - https://learn.microsoft.com/en-us/azure/machine-learning/overview-what-is-azure-machine-learning
