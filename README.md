# When Reasoning Collapses: A Depth-Aware Probe into LLM Reasoning

## What This Work Is About
This project evaluates how reasoning performance in large language models degrades as **reasoning depth** increases.  
We compare **direct answers vs. reasoning prompts** across structured datasets (CLUTRR, ProofWriter) and multiple LLMs (GPT-5, LLaMA-3.1-8B, Qwen-2.5-7B, DeepSeek-32B, GLM-4.5-Air).  
The findings show that reasoning gains at shallow depths collapse sharply as tasks become more compositional.


## Architecture Diagram
<p align="center">
  <img src="AAAI/Diagram3.png" width="800" height="600">
</p>



## Key Graphs

### GPT-5 (ProofWriter)
<p align="center">
  <img src="AAAI/fig2a_gpt5_accuracy.png" width="500">
</p>

<p align="center">
  <img src="AAAI/fig2b_gpt5_delta.png" width="500">
</p>

### LLaMA-3.1-8B (CLUTRR)
<p align="center">
  <img src="AAAI/fig2c_llama_accuracy.png" width="500">
</p>

### Qwen-2.5-7B (CLUTRR)
<p align="center">
  <img src="AAAI/fig2d_qwen_accuracy.png" width="500">
</p>


## Publication
### AAAI-26 Student Abstract  
**Paper link:** *(final AAAI link)*  
**PDF in repo:** `Student_Abstract_AAAI.pdf`


## Conclusion
Reasoning prompts help only at **very shallow depths**.  
As depth increases, accuracy drops sharply, and in many cases reasoning accuracy falls **below direct answers**, revealing that current LLM reasoning is **brittle, depth-sensitive, and unstable**.  
This framework provides a simple, reproducible way to measure collapse-depth and compare reasoning robustness across models.



