# Whisper Transcript Generator MVP (Google Colab)

This is an MVP (Minimum Viable Product) for generating transcripts from audio or video using OpenAI's Whisper API. This notebook is designed to run in Google Colab with a T4 GPU for optimized performance. It allows users to transcribe audio or video content into text, which is then formatted into a downloadable Word document.

## Features:
- **Transcription from multiple sources:** Supports transcription from YouTube videos, Panopto (manual upload), and direct audio file uploads.
- **Automatic metadata generation:** Includes course details such as course name, code, week number, platform, and week topic in the generated transcript.
- **Formatted output:** The transcript is outputted in a well-structured Word document (.docx), ready for use in academic or professional settings.
- **Google Colab friendly:** Easily run the notebook in Google Colab, no local setup required.
- **GPU-accelerated performance:** Optimized to run with the T4 GPU for faster transcription.

## How to Use:
1. Open this notebook in <a href="https://colab.research.google.com/github/<your-github-username>/<your-repo-name>/blob/main/whisper_transcript_generator.ipynb" target="_blank">Google Colab</a>.
2. Select **Runtime > Change runtime type** and set the hardware accelerator to **GPU** (T4).
3. Install the required libraries (see the notebook for installation commands).
4. Upload an audio file or provide a YouTube URL for the video/audio you wish to transcribe.
5. Click the "Generate Transcript" button to create the transcript and download it as a Word document.

## Requirements:
- **Google Colab** (for running the notebook).
- **T4 GPU** (recommended for better performance).
- Audio file (MP3 format) or YouTube video URL.
- Internet access (for YouTube video processing).

## Installation (if running locally):
If you want to run this notebook locally, you can install the required libraries using the following commands:

```bash
pip install whisper python-docx yt-dlp pypandoc
pip install git+https://github.com/openai/whisper.git
sudo apt update && sudo apt install -y ffmpeg pandoc
