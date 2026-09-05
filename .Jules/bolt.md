# Bolt ⚡ Journal - Critical Learnings Only

## 2026-07-09 - Prompt Token Optimization

**Learning:** In a repository consisting primarily of agent prompts,
performance can be measured by token efficiency and clarity. Redundant bullet
points and multi-line descriptions in prompt files increase context window usage
without adding actionable intelligence.
**Action:** Streamline prompt instructions by grouping similar items and
removing "illustrative-only" sections that instructions already tell the agent
to ignore.

## 2026-07-10 - Streamlining Large Prompt Definitions

**Learning:** Large agent files like `sentinel.md` (>10KB / ~2.7k tokens)
contained extensive duplicate listing of security examples across multiple
priority categories and verbose code examples. Condensing code snippets and
grouping priority lists can achieve >60% token reduction while fully retaining
all critical security directives and guidelines.
**Action:** When optimizing prompt files, replace verbose repeated lists with
concise categorized bullet points and compact TypeScript examples.

## 2026-07-11 - Optimizing Academic Prompt Efficiency

**Learning:** Academic writing agent prompts often contain redundant step-by-step
summaries in process and delivery sections. Consolidating negative constraints and
merging daily process steps into single high-density list items reduces token overhead
by ~35% (~119 lines to ~105 lines, or ~772 words to ~490 words) while preserving
all safety rules and behavioral expectations.
**Action:** Streamline multi-step process lists and category items into compact,
dense sentences when tuning prompt files.

## 2026-08-30 - Standardizing Agent Prompt Structure for Token Efficiency

**Learning:** Unformatted agent prompt files (like `typist.md`) often contain
redundant spacing, loose headers, and unconstrained line lengths.
Restructuring them into standardized 80-character wrapped Markdown with
concise bullet points reduces word count by ~30% (~778 to 546 words) while
maintaining full instructional clarity and adding security directives.
**Action:** When optimizing agent prompts, convert unformatted long lines into
standard structured Markdown with high-density bullet points.

## 2026-09-01 - Optimizing Navigation Agent Prompt Density

**Learning:** Unwrapped prompt definitions like `cartographer.md` contained
loose formatting, excessive spacing, and verbose explanations.
Refactoring into standardized 80-character line wrapped Markdown with concise
bullet points and added security guidelines reduces word count by ~34%
(~730 to 483 words) while maintaining full instructional coverage.
**Action:** Streamline verbose routing agent descriptions and convert loose lists
into compact bullet points.
