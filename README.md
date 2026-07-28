<div align="center">

<a href="https://github.com/devfrankduah">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&duration=3500&pause=800&color=6366F1&center=true&vCenter=true&width=720&lines=Hey%2C+I'm+Frank+%F0%9F%91%8B;AI%2FML+Engineer;Building+LLMs+from+first+principles;Agentic+AI+%C2%B7+LLM+Eval+%26+Safety+%C2%B7+Edge+AI;Always+shipping.+Always+learning." alt="Typing SVG" />
</a>

<br />

<a href="https://www.frankduah.me"><img alt="Portfolio" src="https://img.shields.io/badge/Portfolio-6366F1?style=for-the-badge&logo=vercel&logoColor=white" /></a>
<a href="https://www.linkedin.com/in/devfrankduah"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="https://github.com/devfrankduah"><img alt="GitHub" src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
<img alt="Views" src="https://komarev.com/ghpvc/?username=devfrankduah&style=for-the-badge&color=6366F1&label=PROFILE+VIEWS" />

</div>

<br />

## About Me

```ts
const frank = {
  role:       "AI/ML Engineer",
  background: "Software Engineering & DevOps",
  focus:      ["LLMs from first principles", "Agentic AI", "LLM Eval & Safety", "Edge AI"],
  building:   "AI agents, LLM tooling, and eval/red-teaming systems",
  learning:   ["Advanced ML", "Distributed Systems", "Cloud Architecture"],
  philosophy: "Build from first principles, then ship with tests.",
};
```

- Building the **LLM stack from scratch, no frameworks**: a transformer with hand-derived gradients, LoRA/DoRA/QLoRA fine-tuning, a byte-level BPE tokenizer, an MCP server, and an agent red-teamer. The code is public, see below.
- Going deep on **LLMs, agentic AI, LLM evaluation & safety**, and **edge AI**
- Open source: **second-highest contributor to [llm-exe](https://github.com/llm-exe/llm-exe)** ([my merged PRs](https://github.com/llm-exe/llm-exe/pulls?q=is%3Apr+author%3Adevfrankduah+is%3Amerged))
- Ask me about **LLMs, agentic AI, RAG, evaluation, MLOps, AWS**, or **DevOps**

<br />

## Tech Stack

<div align="center">

**Languages**

[![My Skills](https://skillicons.dev/icons?i=python,ts,js,dart,java,c,cpp,html,css,bash)](https://skillicons.dev)

**ML & AI**

[![My Skills](https://skillicons.dev/icons?i=pytorch,tensorflow,sklearn,opencv)](https://skillicons.dev)

**Frameworks & Libraries**

[![My Skills](https://skillicons.dev/icons?i=react,nextjs,vue,nuxtjs,nodejs,express,flutter,tailwind,redux)](https://skillicons.dev)

**Databases & Platforms**

[![My Skills](https://skillicons.dev/icons?i=postgres,mysql,mongodb,firebase,supabase,prisma)](https://skillicons.dev)

**Cloud & Tools**

[![My Skills](https://skillicons.dev/icons?i=aws,docker,git,github,githubactions,vercel,netlify,figma,postman,vscode)](https://skillicons.dev)

</div>

<br />

## Featured Projects

<div align="center">
<table>
<tr>
<td align="center" width="50%" valign="top">

<br />

### Glassbox

<p><sub><i>A Transformer Built From Scratch in NumPy</i></sub></p>

<p align="left"><sub>No PyTorch, no autograd. Forward <strong>and</strong> backward passes for attention, LayerNorm, RMSNorm, GELU, SwiGLU, RoPE, softmax, and cross-entropy are all hand-derived and gradient-checked to <strong>1e-8</strong>. Ships both GPT-2 and Llama-style architectures in one codebase, trains on a CPU, generates with a KV-cache, and renders attention heatmaps so the internals are visible. 39 tests.</sub></p>

<p>
  <img src="https://skillicons.dev/icons?i=python" height="28" />
</p>

<a href="https://github.com/devfrankduah/glassbox"><img src="https://img.shields.io/badge/Source-181717?style=for-the-badge&logo=github&logoColor=white" /></a>

<br /><br />

</td>
<td align="center" width="50%" valign="top">

<br />

### Forge

<p><sub><i>LoRA, DoRA & QLoRA From Scratch</i></sub></p>

<p align="left"><sub>Efficient fine-tuning implemented by hand, forward and backward, gradient-checked to <strong>1e-8</strong>. Includes DoRA (weight-decomposed LoRA, 2024) and QLoRA-style int8 quantization for a roughly 4x smaller frozen base, plus adapter save/load/hot-swap and honest held-out perplexity eval. The base model is provably untouched. 59 tests.</sub></p>

<p>
  <img src="https://skillicons.dev/icons?i=python" height="28" />
</p>

<a href="https://github.com/devfrankduah/forge"><img src="https://img.shields.io/badge/Source-181717?style=for-the-badge&logo=github&logoColor=white" /></a>

<br /><br />

</td>
</tr>
<tr>
<td align="center" width="50%" valign="top">

<br />

### Crucible

<p><sub><i>Adversarial Stress-Tester for LLM Agents</i></sub></p>

<p align="left"><sub>Point it at any agent and it runs hostile and edge-case attacks aligned with the OWASP LLM Top 10 (prompt injection, jailbreaks, secret-leakage, hallucination, robustness, over-refusal), then reports per-category hold rates over N trials plus a severity-weighted risk score. Includes a CI gate that fails a build when an agent gets measurably less safe. Zero dependencies, 61 tests.</sub></p>

<p>
  <img src="https://skillicons.dev/icons?i=python" height="28" />
</p>

<a href="https://github.com/devfrankduah/crucible"><img src="https://img.shields.io/badge/Source-181717?style=for-the-badge&logo=github&logoColor=white" /></a>

<br /><br />

</td>
<td align="center" width="50%" valign="top">

<br />

### ML-Latency-Aware-Execution-Engine

<p><sub><i>RL Trade Execution</i></sub></p>

<p align="left"><sub>RL agent that minimises crypto slippage on large orders, using a Double DQN with a dueling architecture and prioritized experience replay alongside classical models. Trained on real Binance data across 3 assets and validated against 98M tick-level trades. Implements the Almgren-Chriss market-impact model, with 17 ablation studies and 176 unit tests.</sub></p>

<p>
  <img src="https://skillicons.dev/icons?i=python,pytorch" height="28" />
</p>

<a href="https://github.com/devfrankduah/ML-Latency-Aware-Execution-Engine"><img src="https://img.shields.io/badge/Source-181717?style=for-the-badge&logo=github&logoColor=white" /></a>

<br /><br />

</td>
</tr>
<tr>
<td align="center" width="50%" valign="top">

<br />

### llm-exe

<p><sub><i>Open-Source Contributor · <a href="https://llm-exe.com">llm-exe.com</a></i></sub></p>

<p align="left"><sub>Second-highest contributor to this upstream TypeScript framework for building LLM applications, across workflow automation, CI/CD hardening, release pipeline improvements, and docs-sync infrastructure.</sub></p>

<p>
  <img src="https://skillicons.dev/icons?i=ts,githubactions" height="28" />
</p>

<a href="https://github.com/llm-exe/llm-exe"><img src="https://img.shields.io/badge/Upstream-6366F1?style=for-the-badge&logo=github&logoColor=white" /></a>
<a href="https://github.com/llm-exe/llm-exe/pulls?q=is%3Apr+author%3Adevfrankduah+is%3Amerged"><img src="https://img.shields.io/badge/My%20merged%20PRs-181717?style=for-the-badge&logo=github&logoColor=white" /></a>

<br /><br />

</td>
<td align="center" width="50%" valign="top">

<br />

### Opening Soon

<p><sub><i>The Rest of the From-Scratch Stack</i></sub></p>

<p align="left"><sub><strong>Cleave</strong>, a byte-level BPE tokenizer with a provably lossless Unicode round-trip, exported to a dependency-free in-browser tokenizer. <strong>Winnow</strong>, an MCP server written without an SDK (JSON-RPC 2.0 over stdio) that compacts documents to Markdown and scans them for prompt injection. <strong>Device-Aware RAG Agent</strong>, routing between cloud, quantized on-device GGUF, and fully offline modes.</sub></p>

<p>
  <img src="https://skillicons.dev/icons?i=python" height="28" />
</p>

<sub><i>Write-ups at <a href="https://www.frankduah.me">frankduah.me</a></i></sub>

<br /><br />

</td>
</tr>
</table>
</div>

<br />

##  GitHub Stats 

<div align="center">  
  <a href="https://github.com/devfrankduah">    
    <img height="175" src="https://github-readme-stats.vercel.app/api?username=devfrankduah&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&rank_icon=github&card_width=450" />  
  </a>  
  <a href="https://github.com/devfrankduah">    
    <img height="175" src="https://github-readme-streak-stats.herokuapp.com/?user=devfrankduah&theme=tokyonight&hide_border=true&card_width=450" />  
  </a>
</div> 
<div align="center">  
  <img height="175" src="https://github-readme-stats.vercel.app/api/top-langs/?username=devfrankduah&layout=compact&theme=tokyonight&hide_border=true&langs_count=8&card_width=450" />  
<img height="175" src="https://github-profile-trophy.vercel.app/?username=devfrankduah&theme=tokyonight&no-frame=true&no-bg=true&column=3&row=2&margin-w=10&margin-h=10" />
</div>

<br />
<br />

## Contribution Activity

<div align="center">
  <img width="100%" src="https://github-readme-activity-graph.vercel.app/graph?username=devfrankduah&bg_color=1A1B27&color=A78BFA&line=6366F1&point=F472B6&area=true&area_color=6366F1&hide_border=true&custom_title=Contribution%20Graph%20%7C%20Last%2030%20days&title_color=E4E4E7&height=300" />
</div>

<br />
<br /> 

## Dev Quote 

<div align="center">  <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight" /></div> <br />


<div align="center">
  <sub>From <a href="https://github.com/devfrankduah">devfrankduah</a>, thanks for stopping by.</sub>
</div>
