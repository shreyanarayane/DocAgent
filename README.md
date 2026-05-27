# Drafter

Drafter is a conversational writing assistant that lives in your terminal. It remembers what you write, updates it when you ask, and saves the final document to a file – all through natural conversation.

You talk to Drafter, and Drafter talks back. When you give it text, it stores that text. When you change your mind, you just tell it the new version. When you're done, you say “save” and give a filename. The agent calls the right tools by itself, shows you what it did, and finishes cleanly.

## What Drafter does

- **Remembers** – the document stays in memory while you work.
- **Updates** – every time you provide new content, Drafter replaces the old document with the complete new version.
- **Saves** – writes the current document to a `.txt` file (adds `.txt` if you forget).
- **Ends** – after a successful save, the conversation stops automatically.

## How you run it

You need Python 3.9 or newer, a Groq API key (free at console.groq.com), and a few packages. Put your code in a file named `drafter.py`. Next to it, create a `.env` file that contains exactly `GROQ_API_KEY=your_key_here`. Then open a terminal in that folder, create a virtual environment if you like, and install the dependencies with:

`pip install langgraph langchain langchain-groq python-dotenv`

After that, just type `python drafter.py`. Drafter will greet you and wait for your first instruction.

## What you see when you use it

Once running, the agent prints its messages and any tool calls. A typical session looks like this (the actual text will vary, but the flow is always the same):

