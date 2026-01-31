# English Speaking Assessment System

A modern, browser-based English speaking assessment system that generates topics, records student responses, transcribes speech, and evaluates performance using **Puter.js AI-powered scoring** for dynamic, accurate assessments.

## Features

### AI Topic Generation
- Random English speaking topics for 1-minute responses
- Diverse range of conversation questions
- Instant topic generation with one click

### Speech Recording
- 60-second timed recording
- Real-time audio visualization
- Browser-based microphone access
- Countdown timer with visual feedback

### Real Speech Transcription
- Live speech-to-text using Web Speech API
- Real-time transcription as you speak
- Continuous recognition with interim results
- Word count and sentence analysis

### **AI-Powered Evaluation System** (NEW)
- **Dynamic, intelligent scoring** using Puter.js Claude AI
- Multi-dimensional scoring (fluency, vocabulary, grammar, relevance, pronunciation)
- **Personalized feedback** based on actual speech content
- Context-aware evaluation that varies based on speech quality
- Detailed strengths and weaknesses analysis
- Overall score calculation (0-100)
- **No more fixed scores** - each evaluation is unique!

### User Interface
- Modern, responsive dark theme
- Step-by-step assessment workflow
- Real-time status updates
- Visual feedback and progress indicators
- Mobile-friendly design

## Usage

1. **Open the Application**
   - Simply open `index.html` in a modern web browser (Chrome, Firefox, Edge, Safari)
   - No API keys or sign-up required - uses free Puter.js AI

2. **Generate a Topic**
   - Click "Generate Topic" to get a random English speaking question
   - Topics cover various subjects and difficulty levels

3. **Record Your Response**
   - Click "Start Recording" to begin your 60-second response
   - Speak clearly about the given topic
   - See your words transcribed in real-time as you speak
   - The timer will count down from 60 seconds
   - Audio visualization shows your speaking volume

4. **Get Your AI Evaluation**
   - Your speech is transcribed live as you speak
   - After recording, the **AI analyzes your actual transcribed response**
   - View your dynamic overall score (0-100) - varies based on quality!
   - Read detailed feedback including:
     - Score breakdown for each criterion
     - Specific strengths identified by AI
     - Areas for improvement
     - Personalized suggestions

## Assessment Criteria

The AI evaluates your English speaking skills based on:

1. **Fluency (0-100)**
   - Speaking pace and smoothness
   - Natural flow and rhythm
   - Minimal pauses and hesitations

2. **Vocabulary (0-100)**
   - Range and diversity of words used
   - Appropriate word choice
   - Use of advanced vocabulary

3. **Grammar (0-100)**
   - Correct sentence structure
   - Proper verb conjugation
   - Appropriate punctuation

4. **Relevance (0-100)**
   - Staying on topic
   - Addressing the question directly
   - Comprehensive coverage of the subject

5. **Pronunciation Clarity (0-100)**
   - Based on transcription quality indicators

## Technical Details

### Dependencies

- **Puter.js**: Free AI API for dynamic speech evaluation (no API keys needed!)
- **Web Speech API**: Real-time speech-to-text transcription
- **Web Audio API**: Audio recording and visualization
- **MediaRecorder API**: Browser-based audio recording
- **Modern Web APIs**: Microphone access, File API

### AI Evaluation Pipeline

1. Generate random English speaking topic
2. Record 60-second audio response
3. Transcribe speech to text in real-time using Web Speech API
4. Send transcription to Puter.js AI (Claude Sonnet 4.5)
5. AI analyzes content for fluency, vocabulary, grammar, and relevance
6. Receive dynamic JSON response with detailed evaluation
7. Display personalized score and feedback
8. **Fallback to local evaluation** if AI service is unavailable

### Browser Requirements

- Modern browser with JavaScript enabled (Chrome, Edge, or Safari recommended)
- Web Speech API support for transcription
- Microphone access requires HTTPS or localhost
- Web Audio API support
- Internet connection required for speech recognition and AI evaluation
- Approximately 50-100 MB available memory for processing

## Performance Tips

- Speak clearly and at a natural pace
- Stay focused on the given topic
- Use a variety of vocabulary
- Structure your response with clear sentences
- Practice regularly to improve your skills

## Scoring Guide

The AI provides honest, context-aware scoring:

- **80-95**: Excellent speakers with rich vocabulary and complex sentences
- **60-79**: Average speakers with good understanding
- **40-59**: Basic speakers with room for development
- **Below 40**: Needs significant improvement, short responses or many errors

## Limitations

- Speech recognition accuracy depends on microphone quality and speaking clarity
- Requires microphone permissions and Web Speech API support
- Performance can vary based on device capabilities
- Internet connection required for speech recognition and AI evaluation
- Best results with Chrome, Edge, or Safari browsers
- AI evaluation quality depends on transcription accuracy

## License

This project is provided as-is for educational and demonstration purposes.

## Credits

- AI evaluation powered by [Puter.js](https://puter.com) - Free AI API
- Uses Claude Sonnet 4.5 model for accurate speech assessment
