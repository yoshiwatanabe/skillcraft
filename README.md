# SkillCraft - AI-Powered Learning System

An AI agent-centered learning support system that provides personalized education through conversation-based interactions with Claude Code, GitHub Copilot, and Gemini CLI.

## Overview

SkillCraft is designed to revolutionize independent learning by:
- Providing completely personalized learning experiences
- Using AI agents as the primary interface (no traditional web portal)
- Managing all data through Git repositories and text files
- Offering advanced understanding assessment and progress tracking

## Core Features

### 🤖 AI-Agent Centered
- **Claude Code**: Main AI agent interface
- **GitHub Copilot**: VS Code integration
- **Gemini CLI**: Command-line operations

### 📚 Learning Content Management
- Structured concept organization
- Dependency graph creation
- Multi-format content (text, interactive HTML/JS, audio)

### 📊 Understanding Assessment
- Multiple choice questions
- Conversational assessment
- Historical progress tracking

### 🎯 Personalization
- Understanding level visualization
- Automated tutorial generation
- Weakness detection and focused support

## Project Structure

```
/
├── subjects/           # Learning domains (electronics, history, etc.)
├── progress/           # Learning progress and assessment data
├── content/           # Generated tutorials and explanations
├── meta/              # System management and configuration
├── external/          # External resource management
└── dashboard/         # Human-readable UI components
```

## Development Phases

### 🐣 Crawl Phase (Initial)
- Basic subject registration and structuring
- Simple multiple-choice assessments
- HTML/JS progress dashboard
- Basic test recording

### 🚶 Walk Phase (Intermediate)
- Conversational understanding checks
- AI tutorial generation
- Timeline visualization
- External resource integration

### 🏃 Run Phase (Advanced)
- Advanced personalization
- Multi-domain correlation analysis
- Audio content support
- Automated system improvements

## Getting Started

1. **Setup**: The directory structure is already created
2. **Configuration**: Edit `meta/config/system-config.yml` as needed
3. **Add Subjects**: Create learning content in `subjects/` directories
4. **Start Learning**: Interact with AI agents to begin your learning journey

## Technical Stack

- **Data Management**: Git repository + text files (Markdown, YAML, JSON)
- **AI Integration**: MCP (Model Context Protocol)
- **Interface**: AI agents (no traditional web interface)
- **Local Processing**: Local LLM + API-connected AI models
- **Environment**: Windows + WSL Ubuntu, VS Code

## Philosophy

This system prioritizes AI agent efficiency over human file manipulation. The file structure and naming conventions are optimized for AI scanning and processing, with human-readable interfaces provided only where necessary.

---

*Created: July 10, 2025*
*Version: 1.0*
