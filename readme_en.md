# data2024-pro152
This dataset was used in the experiments reported in the paper 'Hallucination Detection on Code Generation with SelfCheckGPT'.

## Dataset Overview
Using a total of 164 HumanEval problems and 10 models, we calculated the pass rates and categorized the problems into those with high accuracy (easy), low accuracy (hard), and intermediate accuracy (middle). 
Then, 10 problems were selected from each difficulty level.

- humaneval_10_easy.jsonl: Pass rate approximately 68%
- humaneval_10_middle.jsonl: Pass rate approximately 46%
- humaneval_10_hard.jsonl: Pass rate approximately 15%
  
## Format of Each Dataset
The format is the same as that of HumanEval.

- `task_id`: identifier for the data sample
- `prompt`: input for the model containing function header and docstrings
- `canonical_solution`: solution for the problem in the prompt
- `test`: contains function to test generated code for correctness
- `entry_point`: entry point for test
  
## Models Used for Difficulty Classification
- GPT-4o-mini: gpt-4o-mini-2024-07-18
- Llama3: meta-llama/Meta-Llama-3-8B-Instruct
- Gemma2: google/gemma-2-2b-it
- Phi-3.5: microsoft/Phi-3.5-mini-instruct
- Qwen2.5-Coder: Qwen/Qwen2.5-1.5B-Instruct
- CodeLlama: meta-llama/CodeLlama-7B-Instruct-hf
- OpenCoder: infly/OpenCoder-8B-Instuct
- LLM-jp-3: llm-jp/llm-jp-3-1.8b-instruct
- Llama-3-Swallow: tokyotech-llm/Llama-3-Swallow-8B-Instruct-v0.1
- chico: NaoS2/tinycodellama-jp-0.6b-20k-2

Model evaluation results may vary depending on the experimental environment.
