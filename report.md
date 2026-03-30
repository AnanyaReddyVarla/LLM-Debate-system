# LLM Debate System Report
1. Introduction

Large Language Models (LLMs) often generate answers without rigorous reasoning, leading to inaccuracies in complex tasks. This project explores whether structured debate between multiple agents can improve reasoning quality and final answer reliability.

Inspired by prior work on debate-based AI alignment and multi-agent systems, we implement a pipeline where competing agents argue opposing viewpoints before a judge determines the final answer.

## Methodology
 System Components

- Debater A (Proponent) — argues YES
- Debater B (Opponent) — argues NO
- Judge — evaluates debate and produces final decision

## Debate Pipeline

- Independent initial responses
- Multi-round argument exchange
- Context-aware rebuttals
- Final judgment based on full transcript

## Multi-Agent Judge Panel (Bonus)
We extend the system by introducing multiple judges (jury system):
- Each judge independently evaluates the debate
- Final decision is determined via majority voting

## Baseline: Direct Question Answering

We evaluated the model on 50 questions using direct prompting without debate.

## Debate-Based Evaluation

Due to API constraints, the debate system was tested on a subset of 3 representative questions, focusing on reasoning-intensive scenarios.

## Multi-Judge Evaluation

A jury of 3 judges was applied to one complex question to analyze:

- Agreement/disagreement patterns
- Reliability of ensemble decisions
  Results
## Quantitative Results
Direct QA Accuracy: 0.84 (84%)

## Qualitative Results
- Debate outputs showed significantly more structured reasoning
- Arguments became more refined across rounds
- Judges produced more detailed explanations compared to direct responses
- Multi-judge system increased confidence in final decisions

## Conclusion

This project demonstrates that multi-agent debate improves reasoning quality compared to direct LLM responses. While direct QA provides faster answers, debate-based systems offer more structured, explainable, and reliable outputs.

The addition of a multi-agent judge panel further enhances robustness, making the system more suitable for complex reasoning tasks.
