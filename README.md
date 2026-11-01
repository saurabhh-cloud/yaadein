# Yaadein 🕯️

A quiet place to remember someone you love. Enter their name, favourite foods and songs, and a short memory, and a local AI model writes a warm remembrance you can edit, print or save as PDF, shown on a candlelit "ofrenda" card.

Made in the spirit of Día de los Muertos and the Hacktoberfest 2026 final theme, "Ghost in the Machine". Built after that challenge closed, so it is **not** a challenge entry.

**Open-source AI at the core:** Google's open-weight **Gemma** model runs on your own computer through **Ollama**. Nothing about your loved one is uploaded anywhere, and it works with the internet off.

## Run it
1. Install Ollama: https://ollama.com/download
2. `ollama pull gemma3:1b`
3. Start Ollama with the page allowed:
   - Windows PowerShell: `Stop-Process -Name "ollama*" -Force; $env:OLLAMA_ORIGINS="*"; ollama serve`
   - Mac/Linux: `OLLAMA_ORIGINS="*" ollama serve`
4. Open `index.html` in Chrome (or the GitHub Pages link) and click **Light a candle**.

The model is told to use only the facts you type and not to invent anything or pretend to be the person. Always read the text and fix anything that isn't true to them.

HTML, CSS, JavaScript, Gemma, Ollama.
