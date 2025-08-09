# aws-ai-knowledge-assistant
AI assistant that can answer questions from your internal docs using AWS Bedrock + Kendra
# AWS AI Knowledge Assistant

An **enterprise-ready AI assistant** that lets teams **search, chat, and extract insights** from their internal documents securely — powered by **Amazon Bedrock** and **Amazon Kendra**.

## 🚀 Overview

This project combines AWS's latest AI capabilities to create a **private, domain-specific knowledge assistant**.  
Instead of sending sensitive data to public LLMs, your documents stay **securely indexed** within AWS and queries are served through a controlled environment.

**Core features:**
- 🔍 **Semantic search** across internal documentation  
- 💬 **Conversational Q&A** with contextual memory  
- 🔐 **Secure by default** — no data leaves your AWS environment  
- ⚡ **Bedrock FMs** for natural language understanding and answer generation  
- 📂 **Kendra indexing** for fast and accurate retrieval

---

## 🛠️ Architecture

1. **Amazon S3** – Storage for raw documents  
2. **Amazon Kendra** – Indexing & semantic search  
3. **Amazon Bedrock** – Foundation Model inference  
4. **AWS Lambda** – Backend processing logic  
5. **Amazon API Gateway** – Secure API endpoints  
6. **Front-end (React)** – Simple web interface for chat/search

![Architecture Diagram](docs/architecture-diagram.png)

---

## 📦 Getting Started

### Prerequisites
- AWS account with Bedrock & Kendra access
- AWS CLI configured
- Node.js & npm
- Python 3.9+

### Deployment (local dev)
```bash
git clone https://github.com/stamatis-petridis/aws-ai-knowledge-assistant.git
cd aws-ai-knowledge-assistant
npm install
npm run dev