# FFmpeg-Starter

This repository serves as a starter guide for using FFmpeg, a comprehensive multimedia processing tool. It includes examples of common tasks such as video conversion, audio extraction, and video compression.

## Prerequisites

- FFmpeg installed on your computer

## Installation

Download and install FFmpeg from the official website:

- [FFmpeg Official Download](https://ffmpeg.org/download.html)

Ensure that FFmpeg is in your system's PATH so that it can be accessed from any command line interface.

## Basic Usage Examples

### 1. Convert video from one format to another

```bash
ffmpeg -i input.mp4 output.avi
```

### 2. Extract audio from video

```bash
ffmpeg -i input.mp4 -q:a 0 -map a output.mp3
```

### 3. Compress video

```bash
ffmpeg -i input.mp4 -vcodec libx265 -crf 28 output.mp4
```

### 4. Merge audio and video

```bash
ffmpeg -i video.mp4 -i audio.mp3 -c:v copy -c:a aac -strict experimental output.mp4
```

## Contributing

Contributions that enhance the examples, extend the functionality, or improve the documentation are welcome. Please fork the repository, create a new branch, and submit a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.
