# 💬 Terminal Chatbot with OpenAI GPT-3.5 & Conversation History

This repository demonstrates a terminal-based conversational agent built using the official Python OpenAI API (`gpt-3.5-turbo`) that tracks message context across dialogue turns.

## 🚀 Overview

The script maintains an active dialogue session by appending user inputs into an in-memory history list. This conversation buffer is injected alongside each subsequent query prompt so the language model retains multi-turn conversational context.

## 🧠 Workflow & Structure

1. Authentication: Configures OpenAI access via your private API key (`openai.api_key`).
2. Interaction Loop: Runs an interactive CLI loop (`while True`) that accepts user prompts until explicitly terminated via commands like `exit` or `q`.
3. Context Memory: Stores historical queries into `history_list` and supplies both the recent message and past context to the completion API.
4. Model Response: Decodes and displays the generated assistant reply using `ChatCompletion`.

## 🛠️ Tech Stack
- Python
- OpenAI Python SDK (`openai`)

## 💻 Installation & Usage

1. Install dependencies:
pip install openai

2. Set up your API key inside the script or export it as an environment variable:
openai.api_key = "YOUR_ACTUAL_API_KEY"

3. Run the script:
python chatbot_gpt.py

4. Chat in the terminal and type `exit` or `q` to terminate the session.
