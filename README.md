# AI Voice Assistant

It is an advanced AI voice assistant app built with Flutter, integrating OpenAI's GPT and DALL-E APIs to provide both text and image responses based on voice input.

## Features

- Voice input recognition
- Text-to-speech output for non-image responses
- Integration with OpenAI's GPT for text-based responses
- Integration with DALL-E API for image generation
- Automatic detection of image vs. non-image requests
- Dynamic response handling (text or image)

## Getting Started

### Prerequisites

- Flutter SDK
- Dart
- OpenAI API key

### Installation

1. Clone the repository and setup project

2. Create a `lib/secrets.dart` file and add your OpenAI API key:
```
const String openAIApiKey = 'your_api_key_here';
```

## Usage

1. Launch the app on your device.
2. Tap the microphone icon to start voice input.
3. Speak your query or request clearly.
4. The app will process your input and determine whether you're requesting an image or a text response.
5. For text responses, the app will use text-to-speech to read out the answer.
6. For image requests, the app will display the generated image on the screen.

## Architecture

The app uses a modular architecture with the following key components:

1. Voice Input Handler: Manages speech-to-text conversion
2. Intent Classifier: Determines whether the user request is for an image or text response
3. OpenAI GPT Client: Handles text-based queries and responses
4. DALL-E Client: Manages image generation requests
5. Text-to-Speech Engine: Converts text responses to speech
6. UI Controller: Manages the app's user interface and response display
