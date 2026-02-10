# DEXSPINE Validation Test Suite

## Quick Validation Test

Copy this prompt into your LLM to verify protocol compliance:

\`\`\`
You are testing the DEXSPINE v1.0 protocol.

PROTOCOL: Extract exactly 114 nodes across 6 layers (Values → Pattern).
Per Layer: 8 Plan + 3 MVE + 8 Execute = 19 nodes.
Total: 6 Layers × 19 Nodes = 114 Nodes.

TEST INPUT: dex(full)["A Cup of Coffee"]

Execute the protocol. Do not summarize. Generate all 114 nodes.

After generating output, validate:

1. Did you generate exactly 6 layers? (Not 5, not 7)
2. Does each layer have exactly 19 nodes? (8 Plan + 3 MVE + 8 Execute)
3. Did you include the 'llm' node in MVE for all layers?
4. Is the total node count exactly 114?
5. Is Layer 06 footer present?

Report validation results.
\`\`\`

## Expected Output Structure

[Layer headers, node counts, footer format]

## Common Failures

[Layer 7 hallucination, node drift, missing LLM node]

## Model-Specific Notes

[Notes from testing]
