# Agentic-AI-Video-Summarizer-Phidata-Google-Gemini-
An intelligent tool that automatically summarizes video content using a pipeline of audio extraction, transcription (via Whisper), and AI summarization (via Google Gemini). Powered by Phidata, it runs an LLM-based agent to process video input and output concise summaries—perfect for lectures, podcasts, or long YouTube videos.


# Phidata Video AI Summarizer Agent 🎥🎤🖬

A Streamlit-based multimodal AI agent that summarizes and analyzes video content using Google Gemini and web search tools.

---

## Features

- **Video Upload:** Supports `.mp4`, `.mov`, and `.avi` files.
- **AI-Powered Analysis:** Uses Google Gemini 2.0 Flash Exp for video understanding.
- **Web Context:** Integrates DuckDuckGo search for supplementary information.
- **Interactive UI:** Built with Streamlit for easy use.

---

## Requirements

- Python 3.9 or higher
- [Streamlit](https://streamlit.io/)
- [google-generativeai](https://pypi.org/project/google-generativeai/)
- [python-dotenv](https://pypi.org/project/python-dotenv/)
- `phi` package (must be obtained separately; not available on PyPI)
- Google API Key (for Gemini)

---

## Setup

1. **Clone this repository:**
   ```bash
   git clone <your-repo-url>
   cd Agentic-AI-Video-Summarizer-Phidata-Google-Gemini-
   ```

2. **Create and activate a virtual environment:**
   ```bash
   python -m venv video-env
   video-env\Scripts\activate   # On Windows
   # source video-env/bin/activate   # On macOS/Linux
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   *(Create a `requirements.txt` with the following:*
   ```
   streamlit
   google-generativeai
   python-dotenv
   # phi (install separately, see below)
   ```
   *)

4. **Install the `phi` package:**
   - If you have access to the `phi` package, install it as instructed by the provider.
   - Example (if you have a wheel file):  
     ```
     pip install path\to\phi.whl
     ```
   - If you do not have the package, contact the code provider.

5. **Set up your `.env` file:**
   ```
   GOOGLE_API_KEY=your_google_api_key_here
   ```

---

## Usage

1. **Run the Streamlit app:**
   ```bash
   streamlit run app.py
   ```

2. **Upload a video file** and enter your query in the text area.

3. **Click "Analyze Video"** to receive AI-powered insights and summaries.

---

## Notes

- The `phi` package is required and must be obtained separately.
- This app is for educational and research purposes.

---

## License

Specify your license here.

---

## Acknowledgments

- [Streamlit](https://streamlit.io/)
- [Google Generative AI](https://ai.google.dev/)
- [DuckDuckGo](https://duckduckgo.com/)