# Roblox CFG Dumper

A specialized external tool for dumping control flow related offsets from Roblox Hyperion.

Designed for analyzing execution paths and extracting important internal offsets used by the Hyperion protection system.

---

## Overview

The CFG Dumper focuses on reconstructing control flow structures inside the Roblox client.

It analyzes how functions branch and interact, allowing accurate extraction of offsets that are otherwise difficult to locate manually.

---

## How It Works

The dumper operates externally and relies on pattern-based analysis combined with control flow tracing.

### Core process:

- Attaches to Roblox process (`RobloxPlayerBeta.exe`)
- Scans memory for known Hyperion patterns
- Identifies control flow structures (functions, jumps, branches)
- Reconstructs execution paths
- Extracts offsets from key instructions
- Outputs structured offset data

---

## Techniques Used

- Pattern scanning
- Control Flow Graph (CFG) reconstruction
- Instruction tracing
- Signature matching
- Offset resolution via instruction analysis

---

## Features

- External (no injection)
- Hyperion-focused analysis
- Accurate offset extraction
- Fast scanning
- Structured output

---

## Example Output

```txt
Hyperion::CheckFunction -> 0x7FF6XXXXXX
Hyperion::ValidateCall -> 0x7FF6XXXXXX
