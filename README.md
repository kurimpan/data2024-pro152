# データセットの説明
HumanEvalの全件を、以下の10個のLLMに回答させた際のpass@1の結果より、モデル全体の正解率が約68%(easy)、約46%(middle)、約15%(hard)となるよう10問ずつ問題を選定しました。
ただし、実験環境等でモデル評価結果が変化する場合があります。ご了承ください。

## 選定に用いたモデル

- GPT-4o-mini：gpt-4o-mini-2024-07-18
- Llama3：meta-llama/Meta-Llama-3-8B-Instruct
- Gemma2：google/gemma-2-2b-it
- Phi-3.5：microsoft/Phi-3.5-mini-instruct
- Qwen2.5-Coder：Qwen/Qwen2.5-1.5B-Instruct
- CodeLlama：meta-llama/CodeLlama-7B-Instruct-hf
- OpenCoder：infly/OpenCoder-8B-Instuct
- LLM-jp-3：llm-jp/llm-jp-3-1.8b-instruct
- Llama-3-Swallow：Llama-3-Swallow-8B-Instruct-v0.1
- chico：NaoS2/tinycodellama-jp-0.6b-20k-2
