# Service pharmaceutical company customer support Agent



An AI-powered Retrieval-Augmented Generation (RAG) assistant designed to help pharmaceutical company customers quickly access relevant product information through natural-language conversations.

## Overview

Pharmaceutical companies manage large amounts of product information, including product details, active ingredients, uses, formulations, availability, and other relevant information.

Finding and providing this information manually can require repeated searching and effort from customer support teams. This can make the support process slower and less efficient.

This project demonstrates how an AI-powered customer support assistant can provide customers with a more accessible way to retrieve relevant pharmaceutical product information through a conversational interface.

## The Problem

Customers may have questions about pharmaceutical products, ingredients, uses, availability, and other product information.

When this information has to be manually searched for and provided by support teams, it can result in slower responses and repetitive work.

The goal of this project was to create a conversational system that allows customers to ask questions naturally and receive relevant information from the company's pharmaceutical knowledge base.

## The Solution

I built a conversational AI assistant connected to a centralized pharmaceutical knowledge base.

When a customer submits a question, the system:

1. Receives the customer's question.
2. Searches the knowledge base for relevant information.
3. Retrieves the most relevant context using vector search.
4. Passes the retrieved information to the AI model.
5. Generates a context-aware response for the customer.

This approach allows the AI assistant to provide responses based on the information contained in the connected knowledge base rather than relying solely on the model's general knowledge.

## How It Works

```text
Customer Question
       ↓
      n8n
       ↓
Knowledge Retrieval
       ↓
    Pinecone
       ↓
 Relevant Context
       ↓
    AI / LLM
       ↓
Customer Response
