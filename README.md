# 🚀 Day 10: From Chatbot to Agentic AI - Giving the Model "Hands"

## 📌 Project Overview
Today marked a massive leap in my AI architecture. I upgraded my n8n workflow from a standard conversational LLM to an **Autonomous Agentic AI**. By integrating external "Tools," the AI can now make real-time decisions, fetch live internet data, and perform complex calculations. It is no longer just predicting text; it is taking action.

## ⚙️ Tools & Architecture Integrated
* **The Brain:** n8n AI Agent powered by Groq (Llama 3).
* **Tool 1 (Calculator):** Bypassed the LLM's natural inability to perform accurate math by giving it a dedicated computation node.
* **Tool 2 (Wikipedia API):** Granted the AI access to the world's largest encyclopedia to fetch real-world, factual data instead of hallucinating.
* **System Prompting:** Engineered instructions to force the AI to autonomously route the user's query to the correct tool based on context.

## 🚧 Challenges Faced & Solutions
1. **Isolated Tool Testing Error:**
   * *Issue:* Attempted to manually execute the Wikipedia tool node within n8n and received an error prompting for a "Query". 
   * *Solution:* Realized an architectural truth about Agentic AI—tools are not meant to be triggered manually by the developer. The AI Agent must act as the orchestrator. I stopped manual UI testing, deployed the flow, and let the AI autonomously generate the query and trigger the tool via Telegram. It worked flawlessly.

## 🎯 Result
I can now text my Telegram bot complex math problems or ask for historical facts, and it autonomously chooses the right tool, executes the task, and returns the formatted answer.
