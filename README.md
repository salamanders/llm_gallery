How well do modern small models perform in a single-shot task running on old hardware?

## Prompt

"1-page HTML demo showcasing the single most advanced WebGPU feature available in latest Chrome browser"

## Command Line

`llama-cli -m {the model file} -ngl 28 --ubatch-size 512 --batch-size 256 --threads 4 --flash-attn --temp 0 -p "1-page HTML demo showcasing the single most advanced WebGPU feature available in latest Chrome browser"`

## Hardware

* 1080ti with 11GiB of VRAM
* 4 core CPU

# Results

* [Gemini 2.5 Pro + Cancas Mode](gemini_2.5_pro.html): Boids
* [devstralQ4_0](devstralQ4_0.html)
* [Ophiuchi-Qwen3-14B-Instruct.i1-Q4_K_M](Ophiuchi-Qwen3-14B-Instruct.i1-Q4_K_M.html): Lots of repeats in the thinking, but eventually produced a result.
* [qwen2.5-coder-7b-instruct-q6_k](qwen2.5-coder-7b-instruct-q6_k.html)