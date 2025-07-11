# Learning Subjects

This directory contains the structured learning content for different subjects. Each subject has its own subdirectory with organized concepts, dependencies, and learning materials.

## Available Subjects

### 🤖 LLM Fundamentals
**Directory**: `llm-fundamentals/`
- Large Language Model fundamentals and architecture
- Transformer mechanisms and attention
- Training processes and optimization
- Target level: Intermediate (customized for Microsoft Engineer)
- **Status**: ✅ Active - Currently learning

### 💻 Design Patterns
**Directory**: `design-patterns/`
- Software design patterns and principles
- Object-oriented design concepts
- Best practices in software architecture
- Target level: Intermediate to Advanced
- **Status**: 📋 Planned - Future learning subject

## Subject Structure

Each subject directory contains its own complete learning environment:

```
{subject-name}/
├── metadata.md                 # Subject configuration and goals
├── scope-definition.md         # Learning boundaries and focus areas
├── knowledge-baseline.md       # Initial knowledge assessment
├── learning-objectives.md      # Structured learning goals
├── initial-concepts.md         # Concept hierarchy and dependencies
├── content/                    # Subject-specific learning materials
│   ├── session-*.md            # Learning sessions and tutorials
│   └── explanations/           # Detailed concept explanations
├── assessments/                # Subject-specific tests and evaluations
│   ├── baseline-test.md        # Initial knowledge test
│   ├── progress-checks/        # Regular assessment materials
│   └── results/                # Test results and analysis
└── progress/                   # Subject-specific progress tracking
    ├── session-logs/           # Individual session records
    └── milestones/             # Achievement tracking
```

This structure ensures each subject is self-contained while maintaining consistency across all learning domains.

## Adding New Subjects

To add a new learning subject:
1. Create a new directory with a descriptive name (kebab-case)
2. Add basic structure files (concepts, dependencies, resources)
3. Update this README with the new subject information
4. Configure AI agents to recognize the new subject area

---
*Last updated: July 10, 2025*
