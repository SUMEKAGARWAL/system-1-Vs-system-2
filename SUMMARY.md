Qwen (Tongyi Qianwen) is a family of large language models (LLMs) and large multimodal models developed by Alibaba Cloud.

System One models are a class of AI models built to make fast, structured, and probabilistic decisions (such as classification, scoring, or routing) directly from input data instead of generating conversational prose


How System One Models Work vs. Traditional LLMs (System 2)


Feature	System One Models (e.g., Jev)	Traditional LLMs (System 2)
Primary Output	Typed choices, numeric scores, or true/false probabilities	Free-form text, code, or chat responses
Sampling Method	Parallel (generates all outputs in a single, fast query)	Sequential (generates one token at a time)
Training Method	RLCD (Reinforcement Learning for Calibrated Decisions)	RLHF or RLVR (Human feedback or verifiable rewards)
Speed & Cost	Extremely fast (70–500 ms) and low cost	Slower and more expensive per request
Hallucination Risk	Outputs are strictly typed and bounded to preset options	Prone to text hallucinations and format errors

Jev: Developed by TypeSafe AI, Jev was the first public System One model released in September 2026. It evaluates structured state and returns choices, scores, or probabilities without generating text

Laya
Multilingual, non-autoregressive System 1 decision model. Give it a state (text, email, ticket, or JSON) and typed questions; it returns typed answers with mathematically calibrated probabilities in a single forward pass (~33 ms) across 100+ languages. Trained with reinforcement learning against strictly proper scoring rules (RLCD), so reporting honest probabilities is the only way to maximise reward. It never generates text, so there is nothing to parse and nothing to hallucinate.
