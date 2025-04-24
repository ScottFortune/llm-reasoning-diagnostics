# LLM Reasoning Diagnostics

## Progress So Far

- Loaded and normalized datasets from MATH and GSM8K for benchmarking.
- Generated model outputs using GPT-4o-mini with LangChain integration.
- Extracted numerical answers from model outputs for comparison with ground truth.
- Evaluated model responses to identify correctness and flagged discrepancies.
- Saved processed results to CSV files for further analysis.

TODO:

- Take model outputs from MATH or GSM8K-style problems
- Classify failures: e.g., numeric mistake, step omission, logic flaw, hallucinated answer
- Write a diagnostic script that flags these failure types

Tools to use:
- transformers, datasets, OpenAI API, LangChain, FastAPI

## LangChain Integration

- Use LangChain for managing LLM prompts and chaining tasks.
- Example: Prompt GPT-4 with LangChain and process outputs.

## Benchmarks (Not todo right now)

- Collect or generate questions requiring logic, recursion, state tracking, etc.
- Add expected output + reasoning steps
- Evaluate mulitple LLMs (GPT-4, Claude, etc.) with structured prompts
- Track hallucination rate or false confidence answers
