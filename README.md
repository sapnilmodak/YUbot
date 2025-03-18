# YUbot - AI-Powered YouTube Summarization & Response Bot

## 📌 Overview
**YUbot** is an AI-powered tool designed to summarize YouTube videos and provide key insights efficiently. It extracts relevant content from long-form videos and YouTube Shorts, offering users a concise and informative summary. The project integrates advanced NLP techniques, leveraging models like **Gemma** for summarization and text-to-video generation.

## ✨ Features
- 📌 **YouTube Video Summarization** - Extracts main points from long videos.
- 🎯 **Shorts Transcript Crawler** - Fetches and analyzes YouTube Shorts transcripts.
- 🧠 **AI-Driven Insights** - Uses advanced NLP to summarize and generate responses.
- 🎬 **Text-to-Video Generation** - Converts summarized text into AI-generated video responses.
- 🚀 **FastAPI Backend** - Ensures efficient and scalable API performance.

## 🏗️ Tech Stack
- **Backend**: FastAPI, Python
- **NLP Models**: Gemma, Hugging Face Transformers
- **Web Scraping**: YouTube API, Custom Subcrawler
- **Deployment**: Docker, Streamlit (for UI)

## 🔧 Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/sapnilmodak/YUbot.git
   cd YUbot
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Set up environment variables:
   - Create a `.env` file and add your **YouTube API key**.
   - Example:
     ```env
     YOUTUBE_API_KEY=your_api_key_here
     ```
5. Run the FastAPI server:
   ```bash
   uvicorn main:app --reload
   ```
6. (Optional) Launch the Streamlit UI:
   ```bash
   streamlit run app.py
   ```

## 🚀 Usage
- Send a YouTube video URL to the API endpoint to receive a summarized response.
- Use the crawler to extract insights from Shorts.
- Generate AI-powered video responses.

## 📌 API Endpoints
| Method | Endpoint | Description |
|--------|------------|-----------------|
| `POST` | `/summarize` | Summarizes a given YouTube video |
| `GET` | `/shorts` | Extracts key points from YouTube Shorts |
| `POST` | `/generate-video` | Converts text summary to AI-generated video |

## 🎯 Future Improvements
- ✅ Improve video response quality using **Sora-like AI models**.
- ✅ Enhance summarization with **multimodal processing**.
- ✅ Deploy scalable **serverless functions**.

## 🤝 Contributing
Feel free to contribute! Open an issue or submit a pull request.

## 📜 License
This project is licensed under the **MIT License**.

## 🌟 Support
If you find this project useful, please ⭐ the repo!

