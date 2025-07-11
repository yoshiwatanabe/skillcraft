# Dependencies

This directory tracks learning dependencies and prerequisite relationships between concepts.

## Dependency Types

- **Concept Dependencies**: What concepts must be understood before others
- **Skill Dependencies**: What skills are needed for specific topics
- **Tool Dependencies**: What tools/software are required
- **Knowledge Prerequisites**: Background knowledge requirements

## File Format

Dependencies are tracked in YAML format for easy AI agent processing:

```yaml
subject: electronics-basics
dependencies:
  concept_a:
    prerequisites: [basic_math, physics_fundamentals]
    enables: [circuit_analysis, component_selection]
```

## File Naming Convention

- `{subject}-concept-dependencies.yml`
- `{subject}-skill-dependencies.yml`
- `{subject}-tool-requirements.yml`

*Dependency mappings will be created as learning paths are established.*
