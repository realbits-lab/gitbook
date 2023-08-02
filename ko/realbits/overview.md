---
description: Service Overview
---

# 🎑 Overview

## AI Service

Our company provides a data-driven chatbot SaaS. You can ask questions and receive answers using personal documents or other public data. You can use personal documents to use the chatbot in confidential mode or provide the service through our own chatbot API. If you want to use it on-premises, we can support personal vector storage, embedding, and LLM technology.

{% hint style="success" %}
<mark style="color:orange;">**Data-driven chatbot**</mark> uses <mark style="color:green;">**RAG**</mark> (Retrieval-Augmented Generation) and <mark style="color:green;">**TAG**</mark> (Tool-Augmented Generation) technologies.
{% endhint %}

A data-driven chatbot is similar to a QA chatbot that retrieves data from documents or databases. Users can write blog posts with product information or customer response emails with customer history data. If you can manage prompts, you can create chatbot characters like foreign language teachers or astrologers.

```mermaid
graph LR
  style U fill:#f96,stroke:#f00,stroke-width:2px
  style L fill:#f96,stroke:#f00,stroke-width:2px

  U["User"] -->|Write|Q(["Question"])
  Q -->|Search|V[("Vector Storage")]
  V -->|Result|T("Question with Data")
  T -->|Question|L["LLM"]
  L -->|Answer|U
```

## Web3 Service

We can provide services through our own chatbot API. We plan to offer several services using web3 and generative AI technology. All of these are open source. Make your ideas come true with Realbits.