---
title: Nikola Tesla Chat
emoji: ⚡
colorFrom: blue
colorTo: indigo
sdk: gradio
sdk_version: 6.0.0
app_file: app.py
pinned: false
python_version: 3.11
short_description: Chat with Nikola Tesla - Knowledge limited to 1856-1943
---

# ⚡ Chat with Nikola Tesla

An AI-powered chatbot that lets you converse with Nikola Tesla, the legendary inventor and electrical engineer. Tesla's knowledge is strictly limited to discoveries, science, and technology that existed during his lifetime (1856–1943).

> **Note**: Tesla's personality, speech patterns, and behavioral traits are carefully crafted through a custom system prompt, designed to authentically capture the essence of the historical figure while maintaining strict historical accuracy.

## 🔬 What You Can Ask Tesla About

- **Electricity & Electromagnetism**: AC/DC current, Tesla coils, transformers
- **Wireless Technology**: Radio waves, wireless energy transmission
- **Inventions**: Induction motors, turbines, mechanical oscillators
- **Physics**: Maxwell's equations, early atomic theory, classical mechanics
- **Early 20th Century Science**: Relativity concepts (Einstein era)

## 🚫 What Tesla Won't Know

Tesla has no knowledge of:

- Modern computers, AI, or the internet
- Quantum mechanics breakthroughs post-1943
- Space missions or modern astronomy
- Contemporary events, technologies, or scientific discoveries

## 💡 Example Questions

- "Explain the difference between AC and DC current"
- "Tell me about your wireless energy transmission experiments"
- "What are your thoughts on radio waves?"
- "How does the Tesla coil work?"
- "What do you think about quantum computers?" (He'll tell you he doesn't know!)

## 🛠️ Tech Stack

- **LLM**: Google Gemini 2.5 Flash via LangChain
- **Framework**: Gradio
- **Hosting**: Hugging Face Spaces

## ⚙️ Setup & Configuration

### Environment Variables

This app requires the following environment variables:

- `GEMINI_API_KEY`: Your Google Gemini API key (get it from [Google AI Studio](https://makersuite.google.com/app/apikey))
- `TESLA_SYSTEM_PROMPT`: The system prompt that defines Tesla's personality and knowledge constraints

### Local Development

1. Clone the repository
2. Create a `.env` file in the root directory:
   ```
   GEMINI_API_KEY=your_api_key_here
   TESLA_SYSTEM_PROMPT=your_system_prompt_here
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the app:
   ```bash
   python app.py
   ```

### Hugging Face Spaces

When deploying to Hugging Face Spaces, add the environment variables in your Space's **Settings** → **Variables and secrets** section.

## 📝 License

MIT License

---

**Try it now**: [Chat with Tesla](https://huggingface.co/spaces/HexByte-lab/nikola-tesla-chat)
