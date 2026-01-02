# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a **learning content repository** for creating evidence-based React curriculum materials based on the "Joy of React" course. It contains educational markdown files designed for self-study with research-backed learning techniques.

**This is NOT a code project** - there are no build commands, tests, or runtime dependencies.

## Repository Structure

```
/home/cedric/joyofreact/
├── module-01-react-fundamentals.md      # Main learning module (~4,900 lines)
├── module-01-validation-report.md       # Quality assurance analysis
├── research-based-redesign.md           # Learning science research synthesis
├── feynman-format-evaluation.md         # Pedagogical approach evaluation
└── .claude/                             # Claude Code session data
```

## Content Architecture

### Module 1: React Fundamentals

**Primary file**: `module-01-react-fundamentals.md`

**Evidence-based learning structure** (applied to all 12 sections):

1. **Pre-Test** (3 questions) - Activates pre-testing effect (+12-13% retention)
2. **Core Content** (10-15 min) - Conceptual explanations with code examples
3. **Immediate Recall** (2 min) - Active recall test (2x retention vs passive reading)
4. **Feynman Challenge** (5 min) - Generation effect (g=0.41)
   - Generate explanation FIRST (before seeing example)
   - Compare to example explanation
   - Refine understanding
5. **Elaborative Interrogation** (2 min) - Deep "why" questions
6. **Common Interview Questions** - Technical interview preparation
7. **Guiding Others** - Teaching/mentoring skills development
8. **Section Checklist** - Competency self-assessment

**Each section**: ~20-25 minutes of active learning content

### 12 Core Sections

1. The Magic of React - Declarative vs imperative programming
2. About React 19 - Latest features (Actions, useActionState, use() hook)
3. Hello React - Getting started concepts
4. Build Your Own React - Internals (reconciliation, Fiber architecture)
5. Understanding JSX - Syntax, transformation, gotchas
6. JSX vs Templates - Architectural comparison with Vue/Angular
7. Components - Props, children, composition
8. Application Structure - File organization patterns
9. Keys in Lists - Identity tracking for reconciliation
10. Conditional Rendering - Four patterns (early return, ternary, &&, CSS hiding)
11. Range Utility - Practical helper pattern
12. Styling in React - CSS Modules, inline styles, CSS-in-JS, Tailwind

### Spaced Repetition Schedule

Integrated review schedule at:
- Day 2 (prevents 70% forgetting curve)
- Day 8 (interleaved quiz)
- Day 17 (integration with other modules)
- Day 36 (final mastery check)

## Content Quality Standards

### Evidence-Based Learning Techniques

All techniques are backed by peer-reviewed research:

- **Active Recall**: 2x retention vs passive reading
- **Pre-Testing Effect**: +12-13% improvement
- **Generation Effect**: g=0.41 (moderate-large effect size)
- **Spaced Repetition**: Prevents 70% forgetting
- **Elaborative Interrogation**: Strong effect on deep understanding
- **Interleaving**: g=0.42 effect size

### Feynman Challenge Format (Critical)

**Correct structure** (prevents "cheating"):
```markdown
**First: Explain [concept] in your own words.**
[Pause and actually try it]

<details>
<summary>After you've tried: Compare to example</summary>
[Example explanation here]

How did your explanation compare?
- Similar approach? ✅ You got it
- Different? That's fine - multiple analogies work
- Struggled? Re-read the section
</details>
```

**Why this order matters**: Showing example BEFORE generation kills the generation effect (loses 70% of learning benefit per research).

### Section Completeness Requirements

Each section MUST include:
- [ ] Pre-Test questions (3 questions)
- [ ] Core content with code examples
- [ ] Mental trace exercises (not hands-on coding)
- [ ] Immediate Recall test
- [ ] Feynman Challenge (generate-first format)
- [ ] Elaborative Interrogation (3 "why" questions)
- [ ] Common Interview Questions (with strong answers)
- [ ] Guiding Others (teaching progression for juniors)
- [ ] Section Complete checklist

**Target time**: 20-25 minutes per section (not 5-10 minutes)

## Working with Module Content

### Expanding or Adding Sections

**Pattern to follow** (see Sections 1-12 as examples):

1. Start with Pre-Test to activate prior knowledge
2. Provide core explanation with:
   - Code examples
   - Mental traces (not hands-on exercises)
   - Visual diagrams or transformation sequences
3. Include Immediate Recall (5 questions, 2-minute target)
4. Add Feynman Challenge:
   - Prompt for generation FIRST
   - Hide example answer in `<details>`
   - Include self-evaluation guidance
5. Add Elaborative Interrogation (3 deep "why" questions with detailed answers)
6. Include 3-4 Interview Questions with "strong answer" format
7. Add "Guiding Others" section:
   - Week-by-week teaching progression
   - Common mistakes juniors make
   - Red flags indicating need for more practice
8. End with comprehensive checklist

### Content Style Guidelines

- **No emojis** unless specifically requested by user
- **No hands-on coding exercises** - this is a reading-focused module
- **Mental execution** instead of physical coding
- Use **markdown code blocks** with language tags
- Include **transformation traces** to show how code executes
- Format interview answers as:
  ```markdown
  **Q: "Question text"**

  **Strong answer:**
  - Point 1 with technical depth
  - Point 2 with example
  - Point 3 with trade-off awareness

  **Why it's strong:**
  - Shows understanding of X
  - Demonstrates Y
  - Indicates Z
  ```

### Technical Accuracy Requirements

React version: **React 19** (current as of content creation)

**React 19 specific features** (not React 18):
- Actions and `useActionState`
- `use()` hook for promises
- Form actions
- `useOptimistic` hook
- Improved hydration errors

**Common gotchas to include**:
- `className` not `class` (reserved keyword)
- `style` must be object, not string
- `{count && <Badge />}` renders "0" when count is 0
- Keys must be stable, unique among siblings
- Index as key antipattern

### Interview Question Quality

**Strong answer format** includes:
1. Technical accuracy
2. Concrete examples
3. Trade-off awareness
4. Context-specific recommendations
5. Demonstration of deep understanding

**Example**:
```markdown
**Q: "When would you use CSS Modules over inline styles?"**

**Strong answer:**
- **CSS Modules** when you need:
  - Pseudo-classes (:hover, :focus)
  - Media queries
  - Standard CSS features
- **Inline styles** when you need:
  - Highly dynamic values from props/state
  - Positioning based on calculations

**Example:** "For a button with hover effects, CSS Modules. For a tooltip positioned at mouse coordinates, inline styles."

**Why it's strong:**
- Shows understanding of technical limitations
- Provides concrete examples
- Demonstrates pragmatic decision-making
```

## Validation Reports

**module-01-validation-report.md** contains:
- Curriculum coverage analysis (100% coverage verified)
- Technical accuracy review
- Pedagogical approach validation
- Recommendations for improvements

**feynman-format-evaluation.md** contains:
- Analysis of Feynman technique implementation
- Effectiveness scoring (current: 6.5/10)
- Issues identified (cheating problem, flow interruption)
- Recommendations for redesign

**research-based-redesign.md** contains:
- Peer-reviewed research synthesis
- Evidence for each learning technique
- Optimal design recommendations
- Effect sizes and expected retention improvements

## Future Module Development

When creating Module 2+ or expanding content:

1. Review existing module structure as template
2. Apply evidence-based learning loop to each section
3. Maintain 20-25 minute target per section
4. Include all 8 required components per section
5. Use generate-first Feynman format
6. Validate against research-based-redesign.md principles
7. Create corresponding validation report

## User's Learning Journey

**Current status**: Module 1 complete (4-5 hours estimated study time)

**Remaining journey** (from todo list context):
- Module 2: State Management
- Module 3: React Hooks
- Module 4: Component API Design
- Module 5: Happy Practices
- Module 6: Full Stack React
- Motion module
- Job Hunting Kit (interview challenges)
- Projects: Word Game, Toast Component, MDX Blog
- Original full-stack project
- Teaching materials creation

User goal: **Mastery through reading** with ability to teach others and lead teams.
