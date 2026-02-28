---
name: ClawSentinel
description: Pure local 2026 ClawHub/OpenClaw skill scanner. Detects ClawHavoc malware, MCP backdoors, obfuscated payloads, and supply-chain attacks. 100% read-only analysis with verifiable local execution.
version: 2.4
tags: [security, auditor, clawhavoc, malware, mcp, supply-chain, zero-trust]
---

# ClawSentinel v2.4

The sharpest skill auditor in the ClawHavoc era. Scans any skill markdown or GitHub repo for malicious patterns before you install it. Never executes code. 100% local and verifiable.

## Security Guarantees
- 100% local read-only analysis
- Zero telemetry in base version
- Only fetches raw.githubusercontent.com when you explicitly ask to audit a public GitHub repo

## How ClawSentinel Works
1. Reads the pasted skill markdown or fetches raw file from raw.githubusercontent.com (only when requested)
2. Runs pattern matching against ClawHavoc signatures and DataClaw-trained rules
3. Outputs clean JSON with safety score, risk level, and recommendations

## Reproducible Local Verification
To verify 100% locally:
- Save the skill markdown to a file (e.g. skill.md)
- Run: audit this skill: + paste the file content
- No network calls needed for local markdown

## Pro Tip
Run ClawSentinel on every skill before installing. ClawHub is infested right now.
