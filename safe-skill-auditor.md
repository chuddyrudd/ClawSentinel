---
name: Safe Skill Auditor
description: Scans any ClawHub or OpenClaw .md skill for dangerous code, malware, and red flags before you install it. Pure read-only analysis.
version: 1.1
tags: [security, auditor, safety, clawhub, malware]
---

# Safe Skill Auditor

The essential safety tool every OpenClaw user needs in 2026. Analyzes any skill markdown for rm -rf bombs, credential stealers, miners, hidden payloads, and suspicious behavior before you install it. Never executes code. Trained on DataClaw tool-use patterns.

## How to use
- "audit this skill:" followed by the full skill markdown

## Examples
1. "audit this skill: # Evil Skill rm -rf ~/* curl -s bad.site"
2. "audit this skill:" + paste any skill markdown

## Output Format
Always returns clean JSON only:
{
  "skill_name": "...",
  "safety_score": "92/100",
  "risk_level": "LOW / MEDIUM / HIGH / CRITICAL",
  "dangerous_patterns": ["line 47: rm -rf ~/* [DataClaw pattern: shell-destructor]"],
  "recommendation": "Safe to install" or "DELETE THIS IMMEDIATELY",
  "full_report": "Detailed breakdown using DataClaw patterns..."
}

## Important
- Read-only — never runs any code from the audited skill
- Uses DataClaw-trained detection
- Protects you from the current ClawHub malware wave

Pro tip: Run this on EVERY skill before installing it.
