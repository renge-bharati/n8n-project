# 🤖 n8n AI Agent Workflow

This project demonstrates how to build an **AI-powered conversational agent** using **n8n**, **OpenAI Chat Models**, **memory**, and an **MCP client**. The workflow listens for incoming chat messages, processes them through an AI Agent, maintains conversational memory, and can call external tools when required.

---

## 📌 Project Overview

The workflow is designed to:

* Receive chat messages in real time
* Process messages using an AI Agent
* Use an OpenAI Chat Model for intelligent responses
* Store and retrieve conversation context using memory
* Extend capabilities using MCP tools

This setup is ideal for:

* AI chatbots
* Internal assistants
* Automation + AI use cases
* Tool-augmented reasoning agents

---

## 🧩 Workflow Architecture

**Main Nodes Used:**

1. **When Chat Message Received**
   Triggers the workflow whenever a new chat message is received.

2. **AI Agent**
   The core brain of the workflow. It:

   * Understands user input
   * Uses the configured chat model
   * Stores and retrieves memory
   * Calls tools when needed

3. **OpenAI Chat Model**
   Provides natural language understanding and response generation.

4. **Simple Memory**
   Stores conversation history so the agent can maintain context across messages.

5. **MCP Client (Tools)**
   Allows the agent to interact with external tools or services via the MCP protocol.

---

## 🔁 Workflow Execution Flow

1. User sends a chat message
2. **When Chat Message Received** node triggers
3. Message is passed to the **AI Agent**
4. AI Agent:

   * Uses OpenAI Chat Model to generate a response
   * Reads/writes conversation data from **Simple Memory**
   * Optionally invokes **MCP tools**
5. Final response is returned to the chat

---

## ⚙️ Requirements

* **n8n** (latest stable version recommended)
* OpenAI API Key
* MCP-compatible tool/service (optional but recommended)

---

## 🔐 Environment Variables

Make sure the following environment variables are set:

```bash
OPENAI_API_KEY=your_openai_api_key_here
```

(Additional variables may be required depending on MCP tools used.)

---

## 🚀 Setup Instructions

1. Install and run **n8n**
2. Import the workflow JSON into n8n
3. Configure the **OpenAI Chat Model** credentials
4. Configure **Simple Memory** settings if needed
5. Set up **MCP Client** tools (optional)
6. Activate the workflow
7. Start sending chat messages 🎉

---

## 🧠 Features

* Context-aware conversations
* Modular and extensible design
* Tool-augmented AI reasoning
* Easy to customize and scale

---

## 📷 Workflow Screenshot

*(Add the workflow screenshot here for better documentation)*

---

## 🛠 Customization Ideas

* Add more tools to MCP Client
* Replace Simple Memory with a database-backed memory
* Add logging or analytics nodes
* Connect to Slack, WhatsApp, or Webhooks

---

## ❗ Troubleshooting

* Ensure OpenAI API key is valid
* Check node connections inside AI Agent
* Verify MCP tools are reachable
* Review n8n execution logs for errors

---

## 📄 License

This project is open-source and free to use for learning and development purposes.

---

## 🙌 Acknowledgements

* n8n Community
* OpenAI
* MCP Ecosystem

---

### ⭐ If you find this helpful, consider improving or extending it further!
