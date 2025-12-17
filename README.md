# Mendix Agentic AI – Practical MVP Sample

This repository contains a simple Mendix sample project demonstrating
how to adopt agentic AI in an MVP using Mendix GenAI and Agents.

## What’s included
- Application package as .mpk file is in /project folder
- Predictive agent for ticket prioritization and next-action suggestions
- Chat agent for querying ticket data using natural language
- Structured prompts with JSON outputs are in /agent folder
- Microflow-based function tools
- Support Starter App as the base
<img width="1536" height="1024" alt="Banner" src="https://github.com/user-attachments/assets/3f243677-4d67-4b23-b369-ff8f78370e12" />

## Mendix Version
Tested with Mendix Studio Pro 10.24.10

## Prerequisites
- Mendix Studio Pro
- Either:
  - Mendix GenAI Resource access, or
  - OpenAI API key (small credits are sufficient)

## Setup (Quick)
1. Open the project in Studio Pro
2. Configure the GenAI / OpenAI connector
3. Add your API key
<img width="1922" height="790" alt="API_Key" src="https://github.com/user-attachments/assets/399b669b-c2bb-459b-9b00-34f455c1c97d" />

4. Import the JSON via Agent screen, import button (Agent Overview page).
5. Run locally and test agents from Agent Overview

## Notes/ Limitations
- This project is intended for learning and MVP experimentation
- Prompts and agents can be exported/imported as JSON
- Demo-oriented prompts; not production hardened; keys must be stored safely
## Gemini via OpenAI Connector

 **Google Gemini** can be used with the Mendix **OpenAI Connector** via Google’s OpenAI-compatible endpoint (there is currently no official Mendix Gemini connector).

#### Endpoint
https://generativelanguage.googleapis.com/v1beta/openai/

<img width="607" height="504" alt="image" src="https://github.com/user-attachments/assets/d8e9cf61-8f85-43eb-bd08-890fe1ef7c14" />

#### Model
Gemini models must be **set explicitly** in Mendix (unlike OpenAI, where the connector auto-populates the model), for example:
- `gemini-2.5-flash`
- `gemini-2.0-flash`

#### Availability
⚠️ During testing (especially on the **free tier**), Gemini may return intermittent  
`503 – model overloaded` responses. Adding retry logic or a fallback model is recommended.

## Demo
A short silent demo video is included in the LinkedIn article.https://www.linkedin.com/pulse/ai-agents-mendix-practical-mvp-story-ishtiaq-ahmad-mmmwe 

<img width="1922" height="581" alt="Agents" src="https://github.com/user-attachments/assets/837c833b-5737-4215-b8aa-a83dc63b3c30" />

<img width="1919" height="1052" alt="Chat_Demo" src="https://github.com/user-attachments/assets/fd7f74c4-4c1d-46d7-af58-ed0541e230c3" />

<img width="1922" height="1040" alt="Agent_Prediction" src="https://github.com/user-attachments/assets/4c6ef0e5-2257-436f-a494-9a0cac9d0fcb" />




---
