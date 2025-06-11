---
layout: page
title: Building an Enterprise Chatbot with Open WebUI, AWS Bedrock, and Custom RAG Pipelines
description: CNN Traffic Sign Classification
img: /assets/img/GTSRB/output_10_0.png
importance: 2
category: work
---


# Building an Enterprise Chatbot with Open WebUI, AWS Bedrock, and Custom RAG Pipelines

## Description
An enterprise chatbot leveraging Open WebUI and AWS Bedrock API on Docker, enabling users to interact with LLMs while providing custom RAG pipelines for enhanced retrieval and decision-making.

## Overview
This project aims to develop an enterprise chatbot leveraging Open WebUI and AWS Bedrock API on Docker. It enables users to interact with readily available LLMs on Bedrock while also providing custom pipelines for Retrieval-Augmented Generation (RAG) implementations.

## Current Setup
- **Infrastructure**: Hosted on AWS EC2
- **UI**: Open WebUI for chatbot interaction
- **LLM Backend**: AWS Bedrock API
- **Deployment**: Docker containerized application
- **Users**: Limited to a few users for initial testing
- **Security & Scalability**: Designed for enterprise-level deployment with robust security and scalability considerations
  - **Security Measures**:
    - First non-share and training agreements with the LLM provider
    - Secure private network for restricted access
    - Potential integration of Single Sign-On (SSO) authentication for enhanced security
  - **Scalability**:
    - Access to the latest and most advanced LLMs through the provider
    - Secure infrastructure to support organization-wide deployment

## Features
- Direct access to AWS Bedrock-hosted models
- Custom RAG pipelines for specific team use cases
- Scalable deployment with Docker

## Work in Progress
- Enhancing multi-user support and performance scaling
- Expanding RAG pipelines with improved document retrieval and ranking
- Integrating additional enterprise authentication and access control mechanisms

## Next Steps
- Optimize latency and inference cost
- Implement logging and monitoring
- Expand model options beyond Bedrock-hosted LLMs

## Lessons Learned
- Docker simplifies deployment but requires proper resource allocation on EC2
- Fine-tuning retrieval mechanisms is crucial for effective RAG implementation
- Bedrock's API provides stability, but customization is needed for enterprise workflows

## Future Goals
- Deploy the chatbot at scale within the organization
- Enable integrations with internal knowledge bases
- Implement feedback loops for model improvement