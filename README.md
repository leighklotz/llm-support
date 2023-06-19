# llm-support

## llama.cpp
- My fork: `git clone https://github.com/leighklotz/llama.cpp`
- Original: `git clone https://github.com/ggerganov/llama.cpp`

## llama foundation model with llama-dl
- https://python.langchain.com/en/latest/integrations/ctransformers.html
- python3 convert.py models/65B/
- ./quantize ./models/65B/ggml-model-f16.bin ./models/30B/ggml-model-q4_0.bin q4_0

## HuggingFace Vicuna instead of foundation model

## vicuna
- https://huggingface.co/TheBloke/Wizard-Vicuna-30B-Uncensored-GGML
- ./main -t 10 -ngl 32 -m Wizard-Vicuna-30B.ggmlv3.q5_0.bin --color -c 2048 --temp 0.7 --repeat_penalty 1.1 -n -1 -p "### Instruction: Write a story about llamas\n### Response:"
- ./main -m ./models/vicuna_13B/ggml-vicuna-13b-4bit.bin -t 4 -c 2048 -n 2048 --color -i --reverse-prompt "### Human:" --in ' ' -p "### Human: What is the relation between llama and vicuna?\n### Assistant:"
## chatscripts
- git clone https://github.com/leighklotz/llama-chatscripts
- ./wizard-vicuna.sh
- uses /tmp to store cached prompt, maybe 100-200MB

# References
- https://finbarr.ca/how-is-llama-cpp-possible/
- https://github.com/facebookresearch/llama/blob/main/README.md
- https://medium.com/@jeremyarancio/exploring-llamas-family-models-how-we-achieved-running-llms-on-laptops-16bf2539a1bbhttps://medium.com/@jeremyarancio/exploring-llamas-family-models-how-we-achieved-running-llms-on-laptops-16bf2539a1bb
- https://medium.com/@martin-thissen/vicuna-on-your-cpu-gpu-best-free-chatbot-according-to-gpt-4-c24b322a193a
- https://news.ycombinator.com/item?id=35431575
- https://medium.com/@martin-thissen/vicuna-on-your-cpu-gpu-best-free-chatbot-according-to-gpt-4-c24b322a193a
- https://github.com/vicuna-tools/vicuna-installation-guide
- https://huggingface.co/TheBloke/Wizard-Vicuna-30B-Uncensored-GGML
- https://towardsdatascience.com/decoding-strategies-that-you-need-to-know-for-response-generation-ba95ee0faadc
- https://github.com/ggerganov/llama.cpp/pull/1684
- https://www.reddit.com/r/LocalLLaMA/wiki/index/
- https://github.com/melodysdreamj/WizardVicunaLM
- https://python.langchain.com/en/latest/integrations/ctransformers.html
