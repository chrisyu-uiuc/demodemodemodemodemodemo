# English Speaking Assessment System

A modern, browser-based English speaking assessment system that generates topics, records student responses, transcribes speech, and evaluates performance using AI-powered scoring.

## Features

- **AI Topic Generation**
  - Random English speaking topics for 1-minute responses
  - Diverse range of conversation questions
  - Instant topic generation with one click

- **Speech Recording**
  - 60-second timed recording
  - Real-time audio visualization
  - Browser-based microphone access
  - Countdown timer with visual feedback

- **Speech Transcription**
  - Automatic speech-to-text conversion
  - Real-time transcription display
  - Word count and sentence analysis

- **AI Evaluation System**
  - Multi-dimensional scoring (fluency, vocabulary, grammar, relevance)
  - Overall score calculation (0-100)
  - Detailed performance feedback
  - Personalized improvement suggestions

- **User Interface**
  - Modern, responsive dark theme
  - Step-by-step assessment workflow
  - Real-time status updates
  - Visual feedback and progress indicators
  - Mobile-friendly design

## Usage

1. **Open the Application**
   - Simply open `index.html` in a modern web browser (Chrome, Firefox, Edge, Safari)

2. **Generate a Topic**
   - Click "Generate Topic" to get a random English speaking question
   - Topics cover various subjects and difficulty levels

3. **Record Your Response**
   - Click "Start Recording" to begin your 60-second response
   - Speak clearly about the given topic
   - The timer will count down from 60 seconds
   - Audio visualization shows your speaking volume

4. **Get Your Results**
   - After recording, your speech will be transcribed
   - The AI evaluates your response across multiple dimensions
   - View your overall score (0-100)
   - Read detailed feedback on your performance
   - Receive personalized suggestions for improvement

## Assessment Criteria

The system evaluates your English speaking skills based on:

1. **Fluency (30%)**
   - Speaking pace and smoothness
   - Natural flow and rhythm
   - Minimal pauses and hesitations

2. **Vocabulary (25%)**
   - Range and diversity of words used
   - Appropriate word choice
   - Use of advanced vocabulary

3. **Grammar (25%)**
   - Correct sentence structure
   - Proper verb conjugation
   - Appropriate punctuation

4. **Relevance (20%)**
   - Staying on topic
   - Addressing the question directly
   - Comprehensive coverage of the subject

## Technical Details

### Dependencies

- **Web Audio API**: Audio recording and visualization
- **MediaRecorder API**: Browser-based audio recording
- **Modern Web APIs**: Microphone access, File API

### Assessment Pipeline

1. Generate random English speaking topic
2. Record 60-second audio response
3. Transcribe speech to text
4. Analyze transcription for evaluation metrics
5. Calculate scores across multiple dimensions
6. Generate detailed feedback and suggestions

### Browser Requirements

- Modern browser with JavaScript enabled
- Microphone access requires HTTPS or localhost
- Web Audio API support
- Approximately 50-100 MB available memory for processing

## Performance Tips

- Speak clearly and at a natural pace
- Stay focused on the given topic
- Use a variety of vocabulary
- Structure your response with clear sentences
- Practice regularly to improve your skills

## Limitations

- Accuracy depends on microphone quality
- Requires microphone permissions
- Performance can vary based on device capabilities
- Internet connection required for full functionality

## License

This project is provided as-is for educational and demonstration purposes.
