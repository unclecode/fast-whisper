# 🎙️ YouTube Audio Transcriber

Welcome to the **YouTube Audio Transcriber**! This handy script allows you to transcribe audio from various sources including microphone input, audio files, and YouTube videos. It's powered by FastAPI and Groq for high-quality transcriptions. 🌟

## 🎥 Example: The Hunt for Gollum

With the exciting news of the new Lord of the Rings trilogy coming in December 2026, let's use an example from "The Hunt for Gollum": [Watch on YouTube](https://www.youtube.com/watch?v=5gL9Ctwmc_g) 📺

## 🎥 Video Tutorial

For a detailed explanation, check out the video tutorial here: [YouTube Video](https://www.youtube.com/watch?v=5gL9Ctwmc_g). In this video, we walk you through the process of setting up the transcription server and using both the open-source and Groq methods.

## 🚀 Features

- **Microphone Mode**: Record and transcribe audio directly from your microphone.
- **Audio File Mode**: Transcribe audio files from your local machine.
- **YouTube URL Mode**: Download and transcribe audio from YouTube videos.
- **Save YouTube Audio**: Optionally save the downloaded YouTube audio as an MP3 file.
- **Two Engines**: Choose between `fast` (FastAPI) and `groq` (Groq API) transcription engines.

## 📦 Installation

Make sure you have the required packages:

```
pip install pyaudio pytube pydub requests colorama groq
```

You may also need `ffmpeg` for audio conversions:

```
sudo apt-get install ffmpeg
```

## 🔧 Usage

```
python script.py --help
```

### 🎤 Microphone Mode

```
python script.py
```

### 📁 Audio File Mode

```
python script.py --audio-file path/to/your/audiofile.wav --engine fast > transcript.txt
python script.py --audio-file path/to/your/audiofile.wav --engine groq > transcript.txt
```

### 📺 YouTube URL Mode

```
python script.py --youtube-url "https://www.youtube.com/watch?v=5gL9Ctwmc_g" --engine fast > transcript.txt
python script.py --youtube-url "https://www.youtube.com/watch?v=5gL9Ctwmc_g" --engine groq > transcript.txt
```

To save the downloaded audio using the YouTube video's title:

```
python script.py --youtube-url "https://www.youtube.com/watch?v=5gL9Ctwmc_g" --engine fast --save-audio > transcript.txt
```

## 🧑‍💻 Launch Your Own Transcription Server

You can also launch your own high-quality transcription server using the open-source `fast-whisper` model. Check out the Jupyter notebook provided in this repository for a step-by-step guide on how to do this.

In the notebook, we demonstrate how to run the server in Google Colab and use ngrok to create a public URL for your server, allowing you to use it in your application.

### Steps:
1. **Run the Notebook**: Open the Jupyter notebook and run the cells to launch the server.
2. **Set Up ngrok**: Use ngrok to create a public URL for your server.
3. **Use the URL**: Integrate the URL into your application to access the transcription service.

This method allows you to have your own speech-to-text generator for free! 🎉

## 🗣️ Using Groq for Fast Transcription

For a faster transcription service, you can use Groq's API. They provide a high-speed service which you can integrate into your application. Refer to the script for details on how to set up and use Groq.

## 📣 Contribute

We love contributions! Feel free to fork this project, submit pull requests, and share your improvements. Let's make this tool even better together! 🛠️

## 🌟 Star the Project

If you found this project useful, please give it a star ⭐ on GitHub!

## 🐦 Follow Me

Stay updated and follow me on X (formerly Twitter): [@unclecode](https://x.com/unclecode) 🐦

---

Happy transcribing! 🎧✨