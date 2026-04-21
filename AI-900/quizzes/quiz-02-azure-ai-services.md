# Quiz 2: Azure AI Services

**Instructions:** Answer all 25 questions without looking at your notes. Check the answer key at the bottom when done.

---

## Questions

### **Q1: Service Category - Image Analysis**
A developer wants to add the ability to describe what is in a photo (objects, scenes) to their mobile app, without training any model. Which service should they use?

A) Azure Machine Learning  
B) Custom Vision  
C) Azure AI Vision  
D) Azure OpenAI Service  

---

### **Q2: Service Category - Text Sentiment**
A retail company wants to automatically determine if customer reviews are positive, negative, or neutral. Which Azure AI Language feature fits?

A) Key Phrase Extraction  
B) Named Entity Recognition  
C) Sentiment Analysis  
D) Language Detection  

---

### **Q3: OCR Use Case**
A logistics company wants to digitize scanned delivery forms by extracting printed text. Which capability handles this?

A) Face API  
B) Azure AI Vision - Read API (OCR)  
C) Azure AI Speech - Speech to Text  
D) Custom Vision  

---

### **Q4: Custom vs Pre-Built Vision**
A hospital wants to classify X-ray images as normal or abnormal. Pre-built Azure AI Vision categories do not cover medical images. What should they use?

A) Azure AI Vision image analysis  
B) Face API  
C) Custom Vision — train a custom image classifier  
D) Azure OpenAI DALL-E  

---

### **Q5: Speech Service**
A call center wants to automatically transcribe customer phone calls into text for quality review. Which service fits?

A) Azure AI Language  
B) Azure AI Translator  
C) Azure AI Speech - Speech to Text  
D) Azure AI Vision  

---

### **Q6: Text to Speech**
An accessibility app needs to read out web articles aloud to visually impaired users. Which service and feature fits?

A) Azure AI Speech - Text to Speech  
B) Azure AI Language - Text Summarization  
C) Azure AI Translator  
D) Azure OpenAI - Whisper  

---

### **Q7: Translation Scenario**
A global e-commerce company wants to translate product descriptions from English to 50 other languages automatically. Which service fits?

A) Azure AI Speech - Speech Translation  
B) Azure AI Language  
C) Azure AI Translator  
D) Azure OpenAI Service  

---

### **Q8: Speech vs Translator**
A real-time meeting tool wants to translate spoken English to spoken French during a video call. Which service handles this?

A) Azure AI Translator (text)  
B) Azure AI Language - CLU  
C) Azure AI Speech - Speech Translation  
D) Azure OpenAI Whisper  

---

### **Q9: Generative AI Service**
A company wants to build a chatbot that generates personalized email drafts for sales reps based on a customer's history. Which Azure service fits best?

A) Azure AI Language - Question Answering  
B) Azure OpenAI Service (GPT model)  
C) Azure Bot Service only  
D) Azure AI Language - Sentiment Analysis  

---

### **Q10: Azure OpenAI - DALL-E**
A marketing team wants to generate product images from text descriptions (for example, "a red sneaker on a white background"). Which model fits?

A) GPT-4  
B) Whisper  
C) DALL-E  
D) Embeddings  

---

### **Q11: Azure AI Services vs Azure Machine Learning**
A startup with no data scientists wants to quickly add language translation to their customer portal. What is the most appropriate approach?

A) Build a custom translation model in Azure Machine Learning  
B) Use Azure AI Translator (pre-built service, no training needed)  
C) Deploy a custom neural network  
D) Use Azure OpenAI to train a translation model  

---

### **Q12: Azure Machine Learning Use Case**
A fintech company has proprietary transaction data and wants to train a custom fraud detection model with full control over the training pipeline. What fits?

A) Azure AI Language  
B) Azure AI Services - Anomaly Detector  
C) Azure Machine Learning  
D) Azure OpenAI Service  

---

### **Q13: Chatbot Architecture**
A company wants to build a customer service bot that answers questions from their product documentation. What is the best combination?

A) Azure Bot Service + CLU  
B) Azure Bot Service + Question Answering  
C) Azure OpenAI + Face API  
D) Azure AI Vision + Azure Bot Service  

---

### **Q14: Conversational Language Understanding**
A food delivery app wants a voice assistant that understands orders like "Order two large pizzas to my home address." What Azure AI Language feature handles intent and entity extraction?

A) Sentiment Analysis  
B) Named Entity Recognition (standalone)  
C) Conversational Language Understanding (CLU)  
D) Key Phrase Extraction  

---

### **Q15: Named Entity Recognition**
A legal firm wants to automatically extract all person names, court names, and case dates from legal documents. Which feature fits?

A) Sentiment Analysis  
B) Key Phrase Extraction  
C) Named Entity Recognition (NER)  
D) Language Detection  

---

### **Q16: Content Moderation**
A social platform wants to automatically flag user-uploaded images that contain adult or violent content. Which service fits?

A) Face API  
B) Azure AI Vision - Image Analysis (content moderation)  
C) Custom Vision  
D) Azure AI Language - PII Detection  

---

### **Q17: Anomaly Detection**
A manufacturing company monitors temperature sensor data every minute and wants automatic alerts when readings deviate abnormally. Which service fits?

A) Azure AI Language  
B) Azure OpenAI  
C) Anomaly Detector  
D) Custom Vision  

---

### **Q18: Personalizer**
A news website wants to dynamically reorder articles based on what each individual user is most likely to read. Which service applies?

A) Azure AI Language - Key Phrase Extraction  
B) Personalizer  
C) Anomaly Detector  
D) Azure Cognitive Search  

---

### **Q19: Cognitive Search**
A law firm has thousands of scanned PDF contracts. They want to make these documents full-text searchable, with the ability to filter by extracted person names and dates. What fits?

A) Azure AI Vision only  
B) Azure Cognitive Search with AI enrichment  
C) Azure OpenAI Service  
D) Azure Machine Learning  

---

### **Q20: Face API Capability**
A security system wants to verify that the person presenting an ID badge is the same person as in the photo on the badge. Which service and capability fits?

A) Azure AI Vision - Object Detection  
B) Custom Vision  
C) Face API - Face Verification  
D) Azure AI Language - NER  

---

### **Q21: Consuming Azure AI Services**
How do applications typically integrate with Azure AI Services?

A) By downloading and running models locally  
B) By calling REST APIs with an endpoint URL and API key  
C) By accessing a shared public model without authentication  
D) By writing SQL queries to an Azure database  

---

### **Q22: PII Detection**
A healthcare app processes patient feedback forms and must mask names, phone numbers, and email addresses before storing data for analytics. Which feature fits?

A) Key Phrase Extraction  
B) Sentiment Analysis  
C) Language Detection  
D) PII Detection (Azure AI Language)  

---

### **Q23: Azure OpenAI - Embeddings**
A job platform wants to match job descriptions to candidate resumes based on semantic similarity, even if the exact words differ. Which Azure OpenAI model type is most suited?

A) DALL-E  
B) GPT-4  
C) Whisper  
D) Embeddings  

---

### **Q24: Key Phrase Extraction**
A research company processes thousands of academic papers and wants to automatically surface the most important topics from each paper. Which feature fits?

A) Sentiment Analysis  
B) Key Phrase Extraction  
C) Language Detection  
D) Named Entity Recognition  

---

### **Q25: Multi-Service Scenario**
A bank's customer service platform needs to: (1) transcribe customer calls, (2) detect if the customer is frustrated, and (3) extract the account numbers mentioned. Which combination of services/features is needed?

A) Azure AI Vision + Personalizer + Anomaly Detector  
B) Azure AI Speech (Speech to Text) + Sentiment Analysis + NER  
C) Azure OpenAI + CLU + Face API  
D) Custom Vision + Key Phrase Extraction + Translator  

---

---

## Answer Key & Explanations

| Q | Answer | Explanation |
|---|--------|-------------|
| 1 | C | Azure AI Vision provides pre-built image analysis without training. |
| 2 | C | Determining positive/negative/neutral tone = Sentiment Analysis. |
| 3 | B | Extracting text from scanned documents = OCR / Read API in Azure AI Vision. |
| 4 | C | Medical images need a custom classifier → Custom Vision. |
| 5 | C | Transcribing phone calls = Speech to Text feature of Azure AI Speech. |
| 6 | A | Reading text aloud = Text to Speech in Azure AI Speech. |
| 7 | C | Translating text across many languages = Azure AI Translator. |
| 8 | C | Real-time spoken translation = Speech Translation in Azure AI Speech. |
| 9 | B | Generating personalized text content = Azure OpenAI (GPT model). |
| 10 | C | Generating images from text descriptions = DALL-E model. |
| 11 | B | Quick, no-expertise translation = Azure AI Translator (pre-built). |
| 12 | C | Custom model, full pipeline control, proprietary data = Azure Machine Learning. |
| 13 | B | FAQ-style bot from documents = Azure Bot Service + Question Answering. |
| 14 | C | Understanding intents and entities in conversation = CLU. |
| 15 | C | Extracting people, places, dates from text = Named Entity Recognition (NER). |
| 16 | B | Flagging inappropriate image content = Azure AI Vision content moderation. |
| 17 | C | Detecting anomalies in time-series sensor data = Anomaly Detector. |
| 18 | B | Personalizing content per user based on behavior = Personalizer. |
| 19 | B | Making scanned documents searchable with AI extraction = Cognitive Search + AI enrichment. |
| 20 | C | Matching a person to a photo = Face API - Face Verification. |
| 21 | B | Azure AI Services are consumed via REST APIs with endpoint + API key. |
| 22 | D | Masking names, phone numbers, emails = PII Detection. |
| 23 | D | Semantic similarity matching = Embeddings model. |
| 24 | B | Surfacing main topics from documents = Key Phrase Extraction. |
| 25 | B | Transcribe audio → Speech to Text; detect frustration → Sentiment Analysis; extract account numbers → NER. |

---

## Scoring Guide

| Score | Assessment |
|-------|------------|
| 23–25 (92–100%) | Excellent! Ready for Computer Vision topic. |
| 20–22 (80–91%) | Strong. Review misses, then move on. |
| 17–19 (68–79%) | Revisit the service selection decision tree in notes. |
| 16 or below | Re-read 02-azure-ai-services.md focusing on service categories and scenarios. |

---

**Your Score: _____ / 25 (_____%)**

**Date Taken: ________________**

**Areas to Review:** [Write weak areas here after taking quiz]
