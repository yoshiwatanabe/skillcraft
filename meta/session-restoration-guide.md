# SkillCraft Session Restoration Guide

**Last Updated**: July 10, 2025  
**Current Status**: Two learning subjects fully configured, ready for active learning  
**Repository**: yoshiwatanabe/skillcraft (main branch)

---

## 🎯 Quick Context Summary

### System Purpose
SkillCraft is an AI-powered personalized learning system using Git repositories and structured Markdown files. The system tracks learning progress, generates adaptive content, and maintains knowledge state across sessions.

### Current Learning Subjects
1. **LLM Fundamentals** (Technical, Japanese/English) - ACTIVE
2. **Retirement Planning** (Practical, English) - READY
3. **Design Patterns** (Technical, Planned) - PLACEHOLDER

### Session State
- **User Profile**: Microsoft software engineer, mid-career professional
- **Learning Preferences**: Interactive questioning, bilingual content (Japanese primary, English for efficiency)
- **Progress**: LLM baseline completed (31/68 points), retirement planning baseline ready
- **Next Actions**: Continue LLM Session 1 OR take retirement planning baseline

---

## 📁 Repository Structure Guide

```
skillcraft/
├── README.md                          # Main project overview
├── dashboard/                         # Learning dashboard (future web interface)
│   ├── index.html
│   └── assets/README.md
├── external/                          # External resources and links
│   ├── files/README.md
│   └── links/README.md
├── meta/                             # System configuration and design
│   ├── design-document.md            # Core system architecture
│   ├── optimization-opportunities.md # Performance improvements
│   ├── session-restoration-guide.md  # THIS FILE
│   ├── config/
│   │   └── system-config.yml
│   ├── dependencies/README.md
│   └── prompts/
│       └── learning-subject-setup-instruction.md
├── progress/                         # Cross-subject progress tracking
│   ├── README.md
│   ├── achievements/README.md
│   ├── assessments/README.md
│   ├── daily/README.md
│   └── timeline/README.md
└── subjects/                         # Individual learning subjects
    ├── README.md                     # Subject index
    ├── llm-fundamentals/            # ACTIVE SUBJECT
    │   ├── metadata.md              # Subject configuration
    │   ├── scope-definition.md      # Learning scope
    │   ├── knowledge-baseline.md    # Current knowledge state
    │   ├── learning-objectives.md   # Goals and timeline
    │   ├── initial-concepts.md      # Concept dependencies
    │   ├── assessments/
    │   │   ├── baseline-test.md     # 27-question assessment
    │   │   ├── baseline-results-2025-07-10.md  # User results (31/68)
    │   │   └── baseline-scoring.md  # Scoring methodology
    │   ├── content/
    │   │   ├── session-01-transformer-architecture.md     # Japanese
    │   │   └── session-01-transformer-architecture-en.md  # English
    │   └── progress/README.md
    ├── retirement-planning/         # READY SUBJECT
    │   ├── metadata.md              # Subject configuration
    │   ├── scope-definition.md      # Learning scope
    │   ├── knowledge-baseline.md    # Current knowledge state
    │   ├── learning-objectives.md   # Goals and timeline
    │   ├── initial-concepts.md      # Concept dependencies
    │   ├── assessments/
    │   │   └── baseline-test.md     # 25-question assessment (READY)
    │   ├── content/                 # (Empty - ready for generation)
    │   └── progress/README.md
    └── design-patterns/             # PLANNED SUBJECT
        └── (placeholder structure)
```

---

## 🔄 Context Restoration Commands

### Step 1: Repository Verification
```bash
# Verify current location and repository state
pwd
git status
git log --oneline -5
```

### Step 2: System Status Check
```bash
# Check repository structure
tree skillcraft/ -L 3

# Verify key files exist
ls -la skillcraft/subjects/*/metadata.md
ls -la skillcraft/subjects/*/assessments/baseline-test.md
```

### Step 3: Current Progress Review
Key files to read for context restoration:

1. **Core Configuration**:
   - `meta/design-document.md` - System architecture
   - `meta/session-restoration-guide.md` - This file

2. **LLM Fundamentals Status**:
   - `subjects/llm-fundamentals/metadata.md` - User profile and goals
   - `subjects/llm-fundamentals/assessments/baseline-results-2025-07-10.md` - Test results
   - `subjects/llm-fundamentals/content/session-01-*` - Next session materials

3. **Retirement Planning Status**:
   - `subjects/retirement-planning/metadata.md` - Subject scope
   - `subjects/retirement-planning/assessments/baseline-test.md` - Ready to take

---

## 📊 Current Learning State

### LLM Fundamentals Progress
- **Baseline Assessment**: COMPLETED (July 10, 2025)
- **Score**: 31 out of 68 points (46% - Initial Level)
- **Strengths**: Conceptual understanding of transformers, attention mechanisms
- **Gaps**: Technical implementation details, mathematical foundations
- **Next Session**: Transformer Architecture Deep Dive (materials prepared)
- **Language Preference**: Japanese primary, English for complex explanations

### Retirement Planning Progress
- **Subject Setup**: COMPLETED (July 10, 2025)
- **Baseline Assessment**: READY (25 questions, 25-35 minutes)
- **Focus Areas**: Tax accounts, insurance, investments, estate planning
- **Goal**: Effective financial advisor communication
- **Language**: English (as requested)

---

## 🚀 Session Resumption Instructions

### For AI Agent Context Restoration

When resuming this project with any AI agent, provide this context:

**System Identity**: "This is SkillCraft, an AI-powered personalized learning system. You are helping a Microsoft software engineer learn new subjects through structured, adaptive content."

**Current State**: "Two learning subjects are configured and ready:
1. LLM Fundamentals - baseline completed (31/68), Session 1 materials prepared
2. Retirement Planning - baseline test ready, no sessions started yet"

**User Preferences**: "Interactive questioning style, bilingual content (Japanese/English), structured learning with clear progress tracking"

**Immediate Options**: "User can continue LLM Session 1 (Transformer architecture), take retirement planning baseline test, or configure new subjects"

### Key Agent Commands for Resumption

1. **Read Current State**:
   ```
   read_file: subjects/llm-fundamentals/assessments/baseline-results-2025-07-10.md
   read_file: subjects/retirement-planning/metadata.md
   ```

2. **Verify Structure**:
   ```
   list_dir: subjects/
   file_search: **/*baseline-test.md
   ```

3. **Check Progress**:
   ```
   semantic_search: "baseline assessment results"
   grep_search: "COMPLETED|READY|ACTIVE" (in metadata files)
   ```

---

## 📋 User Preferences & Context

### Learning Style
- **Interaction**: Prefers interactive Q&A over passive reading
- **Questioning**: Detailed explanations when gaps identified
- **Language**: Japanese for familiar concepts, English for complex/technical topics
- **Progress**: Structured sessions with clear milestones

### Technical Background
- **Role**: Microsoft software engineer
- **Experience**: 15+ years in technology
- **Interests**: AI/ML systems, practical applications
- **Goals**: Deep technical understanding + practical implementation

### Personal Context
- **Family**: Planning financial future and education
- **Career**: Mid-level professional seeking advancement
- **Time**: Prefers efficient, focused learning sessions
- **Application**: Wants immediately applicable knowledge

---

## 🔧 System Configuration

### File Management
- **All paths**: Use absolute paths starting with `c:\Users\tsuyo\Repos\skillcraft`
- **New files**: Auto-create directories as needed
- **Naming**: Use ISO date format (YYYY-MM-DD) for time-stamped files
- **Language**: Japanese files use original names, English use `-en` suffix

### Assessment System
- **Baseline tests**: Comprehensive initial knowledge assessment
- **Progress tracking**: Session-by-session advancement
- **Scoring**: Understanding levels (Complete/Partial/Needs Learning)
- **Results storage**: `assessments/baseline-results-YYYY-MM-DD.md`

### Content Generation
- **Session materials**: Interactive, example-rich content
- **Bilingual support**: Primary language + English translation
- **Adaptive difficulty**: Based on baseline assessment results
- **Progress integration**: Builds on previous sessions

---

## 🎯 Next Session Planning

### Immediate Options for Next Session

1. **Continue LLM Fundamentals**:
   - File: `subjects/llm-fundamentals/content/session-01-transformer-architecture.md`
   - Status: Materials prepared, ready to begin
   - Focus: Self-attention mechanisms, positional encoding
   - Duration: 45-60 minutes

2. **Start Retirement Planning**:
   - File: `subjects/retirement-planning/assessments/baseline-test.md`
   - Status: 25-question assessment ready
   - Focus: Current knowledge evaluation
   - Duration: 25-35 minutes

3. **Add New Subject**:
   - Use template in `meta/prompts/learning-subject-setup-instruction.md`
   - Follow same 5-file structure (metadata, scope, baseline, objectives, concepts)
   - Suggested topics: Design patterns, system architecture, leadership skills

### Session Management
- **Begin**: Always confirm current context and user goals
- **Progress**: Track advancement through structured milestones
- **Adaptation**: Adjust difficulty and focus based on performance
- **Completion**: Update progress files and plan next session

---

## 💾 Backup & Recovery

### Critical Files for Complete Restoration
1. `meta/design-document.md` - System architecture
2. `meta/session-restoration-guide.md` - This restoration guide
3. `subjects/*/metadata.md` - All subject configurations
4. `subjects/*/assessments/baseline-results-*.md` - All test results
5. `subjects/*/content/session-*.md` - Generated learning materials

### Git Commit Strategy
- **Each session**: Commit progress and new content
- **Assessments**: Immediate commit after completion
- **System changes**: Separate commits for structure vs content
- **Restoration points**: Tag major milestones

---

**🔄 Quick Restoration Command**: 
"Load SkillCraft context: Microsoft engineer, 2 learning subjects (LLM Fundamentals baseline completed 31/68, Retirement Planning baseline ready), structured AI learning system, ready for next session."
