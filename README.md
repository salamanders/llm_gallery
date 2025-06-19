How well do modern small models perform in a single-shot task running on old hardware?

## Prompt

"1-page HTML demo showcasing the single most advanced WebGPU feature available in latest Chrome browser"

## Command Line

`llama-cli -m {the model file} -ngl 28 --ubatch-size 512 --batch-size 256 --threads 4 --flash-attn --temp 0 -p "1-page HTML demo showcasing the single most advanced WebGPU feature available in latest Chrome browser"`

## Hardware

* 1080ti with 11GiB of VRAM
* 4 core CPU

# Results

* [devstralQ4_0](https://html-preview.github.io/?url=https://github.com/salamanders/llm_gallery/blob/main/devstralQ4_0.html)
* [Ophiuchi-Qwen3-14B-Instruct.i1-Q4_K_M](https://html-preview.github.io/?url=https://github.com/salamanders/llm_gallery/blob/main/Ophiuchi-Qwen3-14B-Instruct.i1-Q4_K_M.html): Lots of repeats in the thinking, but eventually produced a result.
* [qwen2.5-coder-7b-instruct-q6_k](https://html-preview.github.io/?url=https://github.com/salamanders/llm_gallery/blob/main/qwen2.5-coder-7b-instruct-q6_k.html): TBD
* Qwen3-14B-NEO-Imatrix-Max-D_AU-IQ4_XS-imat: Got stuck in an infinite loop.

Hosted models for comparison:

* [Gemini 2.5 Pro + Canvas Mode](https://html-preview.github.io/?url=https://github.com/salamanders/llm_gallery/blob/main/gemini_2.5_pro.html): Boids -- runs, but nothing shows up.
* [Gemini 2.5 Flash + Canvas Mode](https://html-preview.github.io/?url=https://github.com/salamanders/llm_gallery/blob/main/gemini_2.5_flash.html): Nothing shows up.