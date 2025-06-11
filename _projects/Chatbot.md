---
layout: page
title: Building an Enterprise Chatbot with Open WebUI, AWS Bedrock, and Custom RAG Pipelines
description: An enterprise chatbot project that integrates Open WebUI, AWS Bedrock, and custom RAG pipelines. It supports secure, scalable deployments on AWS EC2, enables flexible tool use, and is highly customizable for enterprise settings.
img: /assets/img/chatbot/WebUI.png
importance: 2
category: work
---


## Demo

*Insert GIFs or screenshots here showing the UI, RAG config panel, or tool calling workflow.*

---

## Security

- Hosted on **AWS EC2** with a **private network via VPN**
- **Okta OIDC Single Sign-On (SSO)** integrated for user authentication
- Adheres to enterprise-level security practices

---

## License

- **Permissive license**
  - Fully customizable
  - Access to the complete codebase
  - Redistribution for profit is restricted

---

## Front-End

- **UI**: Open WebUI
- **Branding Support**: Customizable logos, colors, and interface text

---

## LLM Integration

- Enforced **Enterprise Policies**
  - No training or data sharing by provider
- **LLM Providers**:
  - AWS Bedrock
  - LiteLLM (local routing or multi-provider support)

---

## RAG Architecture

### 1. Built-in Knowledgebase (Open WebUI)

- Uses local embedding model: `all-MiniLM-L6-v2`
  - Ref: [SBERT](https://www.sbert.net/)
- Indexing & Vectorization done locally
- Configurable:
  - Chunk size, top-p, reranking models
- Template-driven response generation
- Limitation: < **1GB** total data
- Example query: *"Tell me about gradient descent"*

### 2. AWS Knowledgebase (Enterprise-Scale)

- Designed for larger datasets (>1GB)
- Bedrock supports:
  - Multiple parsing strategies
  - Custom chunking logic
  - Embedding + graph-based retrieval
- Integrated with proprietary enterprise content

---

## Tool Use

- Tools are **custom-built**
- Allow Open WebUI to interact with:
  - AWS Knowledgebase
  - Bedrock-hosted LLMs
- **Native tool-calling** experience
- Returns **citations** for transparency

---

## MCP Proxy (Model Context Protocol)

- Connects local MCP server with remote applications via OpenAPI
- Acts as a **proxy bridge**
  - Ref: [MCP GitHub](https://github.com/modelcontextprotocol/servers?tab=readme-ov-file)
- Enables:
  - Time-based and memory-sensitive tools
  - Unified context management

---

## Features Covered

- 🔍 Web search integration  
- 📁 Document upload and retrieval  
- 🔧 Tool execution via LLM  
- 📚 Scalable document ingestion (via AWS or local)

---

## Next Steps

- Optimize performance and latency
- Improve multi-user load balancing
- Extend model support and feedback collection
- Add end-to-end logging and observability

---

