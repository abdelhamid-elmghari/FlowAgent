FlowAgent - AI Workflow Automation with n8n
Task

FlowAgent is an AI-powered automation workflow built using n8n. The objective of this project is to design a simplified and modular system inspired by OpenClow, capable of handling multi-source inputs, processing different media types, and executing intelligent actions through a central AI agent.

Description

FlowAgent is a visual, scalable AI workflow that connects messaging platforms, media processing, and external tools into one unified system.

The workflow starts by receiving messages from platforms such as WhatsApp and Telegram. It then filters and routes the data depending on the content type, including text, audio, images, and documents.

Audio messages are transcribed into text, images are analyzed using vision models, and documents are parsed for relevant insights. A context builder enriches each request using stored user data, allowing the system to generate more accurate and personalized outputs.

At the core of the system is a main AI agent that processes all inputs and decides the appropriate actions. FlowAgent can also interact with external services such as Google Drive, Gmail, and Google Calendar to store files, send emails, and manage events.

The entire workflow is built visually in n8n, making it easy to customize, extend, and maintain without requiring complex backend development.

Installation

To get started with FlowAgent, first clone the repository from GitHub to your local machine.

Install n8n using npm or run it with Docker depending on your environment. Once n8n is running, import the workflow JSON file provided in this repository.

After importing the workflow, configure all required credentials including messaging APIs (WhatsApp, Telegram), AI services, and Google integrations (Drive, Gmail, Calendar).

Ensure all environment variables and API keys are correctly set before activating the workflow.

Usage

After activation, FlowAgent automatically listens for incoming messages from connected platforms.

When a message is received, the workflow identifies the content type and routes it through the appropriate processing path. For example, voice messages are converted to text, images are analyzed, and documents are processed for structured information.

The AI agent uses this processed data along with user context to generate responses or trigger actions such as sending emails, saving documents, or scheduling calendar events.

FlowAgent can be extended easily by adding new nodes, integrating APIs, or modifying the AI logic to fit different use cases like customer support, automation assistants, or productivity tools.
