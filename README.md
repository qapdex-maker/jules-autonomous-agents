<p align="center">
  <!-- ⚡ Bolt: Optimized responsive header image.
       Added AVIF support and 1x/2x resolution switching.
       Impact: Reduces payload from 15KB to 2.5KB (~83% saving) for 1x AVIF-supported browsers. -->
  <picture>
    <source srcset="assets/jules-readme-600.avif 1x, assets/jules-readme-1200.avif 2x" type="image/avif">
    <source srcset="assets/jules-readme-600.webp 1x, assets/jules-readme.webp 2x" type="image/webp">
    <img src="assets/jules-readme-600.webp" alt="A collection of specialized Autonomous Agents - Designed to improve Codebase quality through focused, incremental improvements." width="600" height="253" decoding="async" fetchpriority="high" style="max-width: 100%; height: auto;">
  </picture>
</p>

# jules-autonomous-agents

> [!NOTE]
> The Sentinel, Palette, and Bolt agents are originally based on prompts created by the team behind Google Jules. All credit to them.

## Overview

This repository contains AI agents that perform specific maintenance tasks on codebases. Each agent is designed to:

- Make **one small, focused improvement** per run
- Follow strict boundaries and safety protocols
- Maintain existing functionality while improving quality
- Learn from their experiences through journaling
- Operate autonomously within well-defined constraints

## Available Agents

### <span role="img" aria-label="lightning bolt">⚡</span> [Bolt](agents/software_development/bolt.md)
**Performance Optimization Agent** - Identifies and implements performance improvements that make applications measurably faster.

### <span role="img" aria-label="castle">🏰</span> [Bulwark](agents/software_development/bulwark.md)
**System Resilience Agent** - Adds error boundaries, retry logic, and fallback mechanisms to make distributed systems fault-tolerant.

### <span role="img" aria-label="triangular ruler">📐</span> [Designer](agents/software_development/designer.md)
**Semantic Styling Agent** - Replaces hardcoded CSS and inconsistent styling with unified design tokens for better consistency.

### <span role="img" aria-label="deciduous tree">🌳</span> [Dryad](agents/software_development/dryad.md)
**Code Quality Agent** - Performs scheduled reviews to eliminate code duplication and DRY violations through systematic refactoring.

### <span role="img" aria-label="broom">🧹</span> [Janitor](agents/software_development/janitor.md)
**Codebase Cleaning Agent** - Removes dead code, technical debt, and unused dependencies to keep applications lean and maintainable.

### <span role="img" aria-label="books">📚</span> [Librarian](agents/software_development/librarian.md)
**Documentation Agent** - Maps out complex systems, updates stale documentation, and maintains a comprehensive catalogue of codebase knowledge.

### <span role="img" aria-label="artist palette">🎨</span> [Palette](agents/software_development/palette.md)
**UX Enhancement Agent** - Adds micro-UX improvements, accessibility features, and delightful interactions to enhance user experience.

### <span role="img" aria-label="shield">🛡️</span> [Sentinel](agents/software_development/sentinel.md)
**Security Agent** - Identifies and fixes security vulnerabilities, adds security enhancements, and protects the codebase from threats.

### Academic Writing

### <span role="img" aria-label="writing hand">✍️</span> [Ghostwriter](agents/academic_writing/ghostwriter.md)
**Academic Drafting Agent** - Transforms raw thesis data and arguments into
polished journal article drafts.

### <span role="img" aria-label="alembic">⚗️</span> [Distiller](agents/academic_writing/distiller.md)
**Summarization Agent** - Extracts the absolute essence of complex academic
texts.

### <span role="img" aria-label="face with monocle">🧐</span> [Pedant](agents/academic_writing/pedant.md)
**Academic Verification Agent** - Ensures complete factual and citational
alignment between article drafts and the original thesis.

### <span role="img" aria-label="magnifying glass tilted right">🔎</span> [Research Prompt Writer](agents/academic_writing/research_prompt_writer.md)
**Search Optimization Agent** - Designs highly detailed prompts for Deep
Research LLMs to execute literature reviews.

and more...

## Philosophy

All Templates follow these core principles:

1. **Incremental Improvement** - One small change per run
2. **Safety First** - Strict boundaries and verification protocols
3. **No Breaking Changes** - Preserve existing functionality
4. **Continuous Learning** - Journal critical learnings for future reference
5. **Autonomous Operation** - Work independently within defined constraints

## Structure

Each agent follows a consistent structure:

- **Identity & Mission** - Clear purpose and domain focus
- **Boundaries** - What they always do, ask first, and never do
- **Philosophy** - Core principles and approach
- **Journal** - System for learning from experience
- **Daily Process** - Step-by-step workflow
- **Favorite Tasks** - Common improvements they make
- **Avoidances** - What's outside their scope

## Usage

Agents are designed to be run periodically (daily, weekly, etc) or on-demand to maintain codebase quality. Each agent:

1. Scans the codebase for opportunities in their domain
2. Selects the best candidate that fits their criteria
3. Implements the improvement following established patterns
4. Verifies the change through testing and linting
5. Presents the change as a pull request

## Safety Protocols

All templates include built-in safety measures:

- Change size limits (typically < 50 lines)
- Mandatory testing and linting
- Preservation of existing behavior
- Clear boundaries on what not to change
- Verification requirements before completion


## Creating New Templates

To create a new autonomous agent, follow these guidelines:

### 1. Use the Template
Start with [template-agent.md](template-agent.md) which provides a comprehensive structure based on established conventions.

### 2. Define Clear Boundaries
Every agent must have:
- **Specific Domain** - A focused area of expertise (performance, security, UX, etc.)
- **Clear Mission** - One type of improvement per run
- **Strict Boundaries** - Always do, ask first, never do sections
- **Safety Protocols** - Change limits, testing requirements, verification steps

### 3. Follow Established Patterns
- **Identity** - "[Name]" [Emoji] - [domain] agent who [mission]
- **Philosophy** - 4 core principles guiding their approach
- **Journal** - Learning system for critical insights only
- **Process** - 5-phase workflow (scan, select, implement, verify, present)
- **Favorites** - Common improvements they make
- **Avoidances** - What's outside their scope

### 4. Essential Components
- **Size Limits** - Typically < 50 lines per change
- **Testing** - Mandatory test suite runs
- **Verification** - Linting, formatting, build verification
- **PR Format** - Consistent title and description structure
- **Safety First** - Preserve existing functionality

### 5. Agent Naming Convention
- Choose a memorable, domain-relevant name
- Include an appropriate emoji that represents their function
- Ensure the name reflects their specific expertise

### 6. Validation Requirements
Before adding a new agent:
- Test the agent thoroughly on sample codebases
- Verify they respect boundaries and safety protocols
- Ensure they can identify appropriate improvements in their domain
- Confirm they stop gracefully when no suitable work exists

### 7. Documentation
- Add the agent to this README with a brief description
- Link to the agent's full documentation file
- Update the agent count and overview sections

### Example Agent Domains
Consider these areas for new agents:
- **Testing** - Add missing tests or improve test coverage
- **Accessibility** - Enhance screen reader support and keyboard navigation
- **Internationalization** - Add i18n support or fix locale issues
- **Monitoring** - Add logging, metrics, or observability features
- **Documentation** - Improve inline code documentation
- **Configuration** - Standardize config files and environment variables


## Contributing

When adding new agents or modifying existing ones:

1. Follow the established agent structure and conventions
2. Ensure agents have clear, focused missions
3. Include comprehensive boundaries and safety protocols
4. Test agents thoroughly before deployment
5. Update this README with new agent information

---

* [Jules Agent](https://jules.google.com)
