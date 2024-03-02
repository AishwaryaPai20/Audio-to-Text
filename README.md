# Audio to Text

This code utilizes the Whisper library from OpenAI to convert audio files into text. It leverages the Medium English model for speech recognition.

## Installation

To install the Whisper library, run the following command:

```bash
!pip install git+https://github.com/openai/whisper.git
```

Additionally, ensure that ffmpeg is installed on your system:

```bash
!sudo apt update && sudo apt install ffmpeg
```

## Usage

To transcribe an audio file, follow these steps:

Ensure the audio file you want to transcribe is in the working directory. For example, let's assume your audio file is named harvard.wav.
Execute the following command to transcribe the audio:

```bash
!whisper "harvard.wav" --model medium.en
```

## Output

After running the transcription command, you might find the following files generated:

* harvard.json: Contains the transcription output in JSON format.
* harvard.vtt: Represents the transcription as WebVTT (Web Video Text Tracks) format, commonly used for displaying timed text tracks along with video or audio content.
* harvard.txt: Contains the transcription output in plain text format.
* harvard.vsv: This file might represent the transcription output in a custom or specific format.
* harvard.stt: Represents the transcription output, possibly tailored for speech recognition or processing.
