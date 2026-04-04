# Coordinator-Worker-Delegator Model

## Chapter 7: Hierarchical Task Decomposition in Multi-Agent Systems

This repository contains the implementation code for Chapter 7 of "Design of Agentic Systems with Case Studies."

## Overview

The Coordinator-Worker-Delegator pattern is a hierarchical architecture for multi-agent systems that handles tasks exceeding any single agent's coordination capacity.

### Three Roles
- **Coordinator**: Strategic oversight, task decomposition, result synthesis
- **Delegator**: Domain-scoped routing and load distribution  
- **Worker**: Specialized task execution

### Three Failure Modes
1. **Context Loss**: Information degrades through delegation chains (p^n preservation)
2. **Coordinator Bottleneck**: Results arrive faster than synthesis capacity (R_in > R_out)
3. **Delegation Oscillation**: Tasks bounce between Delegators with overlapping domains

## Running the Demo

### Option 1: Google Colab (Recommended)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1U4Dt_pNR_lLI1a74aGOKBci2njfD5Yzd)

### Option 2: Local
```bash
pip install nest-asyncio matplotlib
jupyter notebook Chapter7_Demo.ipynb
```

## Key Insight

> Architecture is the leverage point, not the model. Each failure mode is caused by architectural decisions, not model limitations. Swapping GPT-4 for Claude won't fix these failures—only changing the architecture will.

## Author

**Hritik Ram**  
Northeastern University | INFO 7375: Prompt Engineering for Generative AI

## License

MIT
```

---

## 📝 requirements.txt CONTENT
```
nest-asyncio
matplotlib
