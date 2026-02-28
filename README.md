# ClawSentinel 
[![ClawHub](https://clawhub.ai/badge/chuddyrudd/clawsentinel)](https://clawhub.ai/chuddyrudd/clawsentinel) 
[![Version](https://img.shields.io/badge/version-2.4-blue)](https://github.com/chuddyrudd/ClawSentinel) 
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

**The sharpest skill auditor in the ClawHavoc era.** Scans any ClawHub or OpenClaw `.md` skill for malware, backdoors, obfuscated payloads, and supply-chain attacks — **100% local, read-only, never executes code**.

## Features
- Detects ClawHavoc campaign signatures
- MCP/A2A/x402 wallet drain detection
- Advanced obfuscation & social engineering checks
- GitHub repo auditing (raw.githubusercontent.com only)
- Clean JSON output with safety score + recommendations

## Installation
```bash
clawhub install chuddyrudd/clawsentinel
```

## Usage
```
audit this skill: [paste markdown here]
```

## Security Guarantees
- 100% local read-only analysis
- Only fetches raw.githubusercontent.com when explicitly requested
- Zero telemetry

## License
MIT
