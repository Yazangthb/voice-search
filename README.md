
# Audio/Video Search Project

A project that enables searching through audio and video files by identifying and displaying the segments where similar content is spoken. This project utilizes forced alignment, LexRank, speech recognition for auto-captioning, and text embeddings.

## Table of Contents

1. [Introduction:](#introduction)
2. [Installation:](#installation)
3. [Usage:](#usage)
4. [Project Overview:](#project-overview)
5. [Technologies Used:](#technologies-used)
6. [Contributing:](#contributing)
7. [License:](#license)

## Introduction

This project aims to enhance the accessibility and usability of audio and video content by allowing users to search for specific phrases or topics within the media. By leveraging advanced techniques such as forced alignment and text embeddings, the project provides an efficient way to locate relevant segments and auto-generate captions.

## Installation

To set up the project, follow these steps:
```bash
# Clone the repository
git clone https://github.com/username/audio-video-search.git
cd audio-video-search

# Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows use venv\Scriptsctivate

# Install required packages
pip install -r requirements.txt
```

## Usage

To use the project, run the main script that processes audio/video files and allows for searching through them:

```bash
python main.py --input <path_to_audio_or_video> --query "<search_phrase>"
```

This command will output the segments where the specified phrase is spoken along with the corresponding timestamps.

## Project Overview

### Key Features

- **Forced Alignment**: Aligns the spoken words with the audio/video timeline to accurately identify when phrases are spoken.
- **Speech Recognition**: Automatically generates captions for audio/video files using speech recognition technology.
- **LexRank**: Implements the LexRank algorithm to summarize and rank the most relevant segments based on the search query.
- **Text Embeddings**: Uses text embeddings to enhance the search capabilities, allowing for semantic understanding of the queries.

### Workflow

1. **Input Processing**: Users provide an audio or video file along with a search query.
2. **Auto-Captioning**: The audio is processed to generate captions using speech recognition.
3. **Forced Alignment**: The generated captions are aligned with the audio to create a timeline.
4. **Search Execution**: The system uses LexRank and text embeddings to find and rank relevant segments.
5. **Output**: The relevant timestamps and segments are displayed to the user.

## Technologies Used

- **Forced Alignment**: Gentle or similar tools for aligning audio with text.
- **Speech Recognition**: SpeechRecognition library for generating captions.
- **LexRank**: Implementation of the LexRank algorithm for text summarization.
- **Text Embeddings**: Use of models like BERT or Sentence Transformers for semantic search.

## Contributing

Contributions are welcome! If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and add new features or improvements.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.
