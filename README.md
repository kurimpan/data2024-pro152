  # data2024-pro152
  日本語 | [English](readme_en.md)

第152回プログラミング研究発表会の実験に使用したデータセットです。
## データセットの紹介
HumanEval合計164問を対象に10種類のモデルを用いて正答率を算出し、正答率が高い問題(easy), 低い問題(hard), 中間の問題(middle)にカテゴリ分けし、それぞれの難易度から10問ずつ選定を行った。
- humaneval_10_easy.jsonl: 正答率 約68%
- humaneval_10_middle.jsonl: 正答率 約46%
- humaneval_10_hard.jsonl: 正答率 約15%
## 各データセットの形式
HumanEvalと同様の形式である。
- `task_id`: identifier for the data sample
- `prompt`: input for the model containing function header and docstrings
- `canonical_solution`: solution for the problem in the prompt
- `test`: contains function to test generated code for correctness
- `entry_point`: entry point for test
## 難易度分類のために使用したモデル
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

実験環境等でモデル評価結果が変化する場合があります。
