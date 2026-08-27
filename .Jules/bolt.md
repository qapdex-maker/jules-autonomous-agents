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
