# LLM Debate + Judge Pipeline

Name: Varla Ananya Reddy  
Student ID: RQL987  
Course: CS-5823  

This project implements a debate system using LLMs with:
- Debater A (YES)
- Debater B (NO)
- Judge
- Multi-judge panel (bonus)

System Architecture

The system consists of:
Debater A (Proponent) — argues in favor (YES)
Debater B (Opponent) — argues against (NO)
Judge — evaluates the debate and produces a final verdict
Multi-Agent Judge Panel (Bonus) — ensemble of judges for improved reliability

Methodology
- Initial Response Generation
- Both debaters independently respond to the question
Multi-Round Debate
- Agents exchange arguments for multiple rounds
- Context from previous rounds is passed forward
Judgment Phase
- A judge analyzes the entire debate transcript
Produces:
 Analysis
 Final Answer
 Confidence Score
Multi-Judge Aggregation (Bonus)
- Multiple judges evaluate the debate independently
- Final decision determined via majority voting


Experiments:
We conducted experiments across:
- 50 questions using Direct QA (baseline)
- 3 questions using the debate pipeline
- 1 question using multi-agent jury evaluation

Key Features

- Multi-round debate reasoning
- Context-aware argumentation
- Baseline comparison (Direct QA)
- Multi-agent ensemble decision making
- Robust error handling for API limitations
