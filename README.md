# 🧠 EchoMind

An intelligent voice-based training ecosystem that simulates real client interactions using advanced AI technology. EchoMind empowers psychology students to master active listening techniques through natural conversations while receiving instant, personalized feedback on their therapeutic communication skills.

## Overview

EchoMind transforms psychology education through immersive, AI-driven conversational training. Our platform provides a safe, scalable environment that bridges the gap between theoretical knowledge and practical therapeutic skills. Students engage in natural conversations with AI-powered client personas while receiving real-time feedback on active listening techniques—from basic paraphrasing to complex emotional mirroring.

## Key Features

### Voice-First Interaction
- **Polish Speech Recognition**: Seamless voice input using OpenAI Whisper optimized for Polish language
- **Natural Conversations**: Dynamic dialogue flow with AI-powered client personas
- **Real-Time Processing**: Low-latency speech-to-text and response generation

### Intelligent Feedback System
- **Active Listening Analysis**: Evaluation of paraphrasing, emotional reflection, and therapeutic techniques
- **Instant Feedback**: Real-time guidance on conversation quality and technique usage
- **Progress Tracking**: Comprehensive session analytics and skill development monitoring

### Dynamic Client Personas
- **Diverse Backgrounds**: Multiple client profiles with varying personalities and communication styles
- **Authentic Scenarios**: Realistic conversational patterns and emotional responses
- **Expandable Library**: Easy addition of new personas through prompt templates

### Educational Focus
- **Safe Learning Environment**: Controlled scenarios appropriate for student training
- **Session Logging**: Detailed conversation records for review and analysis
- **Instructor Analytics**: Progress reports and performance insights for educators

## Technology Stack

### Core AI/ML
- **OpenAI Whisper**: Polish speech recognition with high accuracy
- **LangChain**: LLM orchestration and conversation management
- **GPT-4o/GPT-4o Mini**: Dynamic dialogue generation and persona simulation
- **Python 3.10+**: Core application development

### Infrastructure
- **Docker**: Containerization for consistent deployment across environments
- **UV Package Manager**: Modern Python dependency management
- **python-dotenv**: Environment configuration and API key management

### Development Tools
- **LangSmith**: LLM monitoring, debugging, and optimization
- **pytest**: Unit testing framework
- **black**: Code formatting and style consistency

## Project Structure

```
echomind/
├── app/
│   ├── main.py                 # Application entrypoint and UI loop
│   ├── speech_to_text.py       # Voice input + Whisper transcription
│   ├── conversation.py         # LangChain + LLM conversation logic
│   ├── evaluation.py           # Active listening evaluator
│   ├── prompts/                # Prompt templates for LLM personas
│   │   ├── client_persona_1.txt
│   │   └── client_persona_2.txt
│   └── config.py               # Environment and runtime settings
├── tests/
│   ├── test_speech_to_text.py  # Unit tests for speech module
│   ├── test_conversation.py    # Unit tests for dialogue manager
│   └── test_evaluation.py      # Unit tests for evaluation engine
├── EchoMind Textbook/          # Technical documentation
│   ├── 🧠 EchoMind Technical Playbook.md
│   ├── Chapters/               # Detailed technical chapters
│   └── Additional materials/   # Supplementary documentation
├── Dockerfile                  # Docker configuration
├── docker-compose.yml          # Multi-service Docker setup
├── requirements.txt            # Python dependencies
├── pyproject.toml              # UV project configuration
├── .env                        # API keys and settings (not in git)
├── .gitignore                  # Git ignore rules
└── README.md                   # This file
```


## Getting Started

### Prerequisites

- **Docker**: Version 20.10 or higher (includes Docker Compose)
- **Git**: For cloning the repository
- **Python 3.10+**: For local development outside Docker (optional)
- **UV Package Manager**: Modern Python dependency management
- **Hardware**: Minimum 8GB RAM, 20GB free disk space

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Solvro/ml-psycho.git
   cd ml-psycho
   ```

2. **Set up environment variables:**
   Create a `.env` file in the project root:
   ```bash
   cp .env.example .env
   ```

   Edit `.env` and add your API keys:
   ```env
   OPENAI_API_KEY=your-openai-key-here
   WHISPER_MODEL=medium
   LANGUAGE=pl
   ```

   - Get your OpenAI API key from [platform.openai.com](https://platform.openai.com/)
   - The `.env` file is ignored by git to protect your sensitive keys

3. **Install dependencies using UV:**
   ```bash
   uv sync
   ```

4. **Build the Docker image (recommended):**
   ```bash
   docker build -t echomind .
   ```

### Running EchoMind

**Using Docker Compose (recommended):**
```bash
docker-compose up
```

**Using Docker directly:**
```bash
docker run --rm -it --env-file .env echomind
```

**For local development:**
```bash
python app/main.py
```

## Development Roadmap

### Phase 1: Foundation (MVP)
- ✅ Voice-first interaction with Polish speech recognition
- ✅ Rule-based active listening evaluation
- ✅ Session analytics and logging
- 🚧 Basic client personas and conversation flow

### Phase 2: Enhancement
- 🔜 ML-powered evaluation with custom models
- 🔜 Expanded persona library and scenario diversity
- 🔜 Progress tracking and gamification systems

### Phase 3: Immersion (VR)
- 📋 Meta Quest 2 VR platform integration
- 📋 Photorealistic avatars with body language
- 📋 Spatial audio and multimodal feedback

### Phase 4: Ecosystem
- 📋 Multi-language support for international markets
- 📋 LMS integration and third-party APIs
- 📋 Research platform with anonymized data insights

## Partnership

**KN Solvro (Wrocław University of Technology)**
- Technical development and AI/ML implementation
- Platform architecture and scalability
- Student-led innovation with industry mentorship

**Human Tech (SWPS University)**
- Psychology education domain expertise
- Pedagogical framework validation
- Academic partnerships and user research

## Documentation

For detailed technical documentation, see the [EchoMind Technical Playbook](./EchoMind%20Textbook/🧠%20EchoMind%20Technical%20Playbook.md):

- [Overview](./EchoMind%20Textbook/Chapters/1.%20Overview.md) - Project vision and strategic objectives
- [System Architecture](./EchoMind%20Textbook/Chapters/2.%20System%20Architecture.md) - Technical design and components
- [Development Environment](./EchoMind%20Textbook/Chapters/3.%20Development%20Environment.md) - Setup and configuration
- [Team Roles & Collaboration](./EchoMind%20Textbook/Chapters/4.%20Team%20Roles%20&%20Collaboration.md) - Workflow and responsibilities

## Ethical Framework

**Privacy & Data Protection**
- GDPR-compliant data handling
- Temporary audio processing with automatic deletion
- Anonymized analytics protecting student identity

**Educational Responsibility**
- Content excludes clinical mental health scenarios
- Age-appropriate interactions and feedback
- Transparent AI decision-making processes

**Accessibility & Inclusion**
- Multi-device compatibility for diverse backgrounds
- Inclusive persona representation
- Support for different learning needs

## Contributing

We welcome contributions from the community! Please see our contributing guidelines and code of conduct.

For questions, issues, or feature requests, please open an issue on GitHub.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

_EchoMind represents the future of practical psychology education—where cutting-edge AI technology meets pedagogical excellence to create transformative learning experiences._