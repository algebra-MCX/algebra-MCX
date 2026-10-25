<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1F3BFF,100:0B1020&height=200&section=header&text=Chenxi%20Ma&fontSize=54&fontColor=ffffff&animation=fadeIn&fontAlignY=36&desc=LLM%20inference%20infrastructure%20%C2%B7%20GPU%20kernels%20%C2%B7%20distributed%20systems&descSize=16&descAlignY=58" width="100%" alt="Chenxi Ma" />

<a href="https://github.com/algebra-MCX"><img src="https://readme-typing-svg.demolab.com/?font=JetBrains+Mono&size=20&duration=3000&pause=1200&color=58A6FF&center=true&vCenter=true&width=760&height=44&lines=LLM+inference+infrastructure;MoE+expert+parallelism+%C2%B7+DBO+%C2%B7+NIXL+dispatch;GPU+kernels+%C2%B7+Triton+%C2%B7+CUDA+Graph;vLLM+contributor" alt="Typing animation" /></a>

<br/>

<a href="https://github.com/vllm-project/vllm/pulls?q=is%3Apr+author%3Aalgebra-MCX"><img src="https://img.shields.io/badge/vLLM-contributor-1F3BFF?style=for-the-badge&logo=github&logoColor=white" alt="vLLM contributor" /></a>
<a href="https://algebra-mcx.github.io/"><img src="https://img.shields.io/badge/Homepage-algebra--mcx.github.io-0B1020?style=for-the-badge" alt="Homepage" /></a>
<a href="https://www.zhihu.com/people/zhib1eiazpn"><img src="https://img.shields.io/badge/知乎-Chenxi%20Ma-0084FF?style=for-the-badge" alt="Zhihu" /></a>
<a href="https://x.com/Chenxi_Ma_ai"><img src="https://img.shields.io/badge/X-@Chenxi__Ma__ai-000000?style=for-the-badge&logo=x&logoColor=white" alt="X" /></a>

</div>

## What I work on

- **MoE serving:** expert parallelism, dispatch / combine, communication–compute overlap
- **vLLM:** MoE expert parallelism, dual-batch overlap (DBO) and NIXL dispatch in Model Runner V2
- **GPU kernels:** Triton fused kernels, CUDA Graph decode, tensor-core attention
- **Engines:** I read production inference engines closely, rebuild their core modules, and measure every change

## vLLM

I'm a contributor to [vLLM](https://github.com/vllm-project/vllm). My work focuses on MoE expert parallelism in Model Runner V2 (MRV2): correctness fixes under dual-batch overlap (DBO), and the performance of NIXL-based dispatch. Two of my DBO correctness fixes have been merged into `main`.

| PR | What it does | Status |
| --- | --- | --- |
| [#63476](https://github.com/vllm-project/vllm/pull/63476) | `[Bugfix][MRV2]` Report the first failed DBO microbatch | Merged |
| [#63372](https://github.com/vllm-project/vllm/pull/63372) | `[Bugfix][MRV2]` Keep routed-expert rows of every DBO microbatch | Merged |
| [#63485](https://github.com/vllm-project/vllm/pull/63485) | `[Perf][MoE]` Size NIXL dispatch from synchronized execution slices | In review |

## Projects

<!-- Repository counts are fetched from GitHub's API with a 300-second badge cache. GitHub's image proxy may add a delay. -->
<table>
<tr>
<td width="50%" valign="top">
<h3><a href="https://github.com/algebra-MCX/mini-DeepInfer">mini-DeepInfer</a></h3>
<p>A minimal, readable re-implementation of DeepInfer's core inference engine design.</p>
<p>
<a href="https://github.com/algebra-MCX/mini-DeepInfer/stargazers"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Frepos%2Falgebra-MCX%2Fmini-DeepInfer&amp;query=%24.stargazers_count&amp;label=Stars&amp;color=E3B341&amp;style=flat&amp;cacheSeconds=300" alt="mini-DeepInfer stars" /></a>
<a href="https://github.com/algebra-MCX/mini-DeepInfer/forks"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Frepos%2Falgebra-MCX%2Fmini-DeepInfer&amp;query=%24.forks_count&amp;label=Forks&amp;color=58A6FF&amp;style=flat&amp;cacheSeconds=300" alt="mini-DeepInfer forks" /></a>
</p>
</td>
<td width="50%" valign="top">
<h3><a href="https://github.com/algebra-MCX/MoEFlow">MoEFlow</a></h3>
<p>MoE expert parallelism: fused Triton kernels, NCCL all-to-all and CUDA Graph decode on B200.</p>
<p>
<a href="https://github.com/algebra-MCX/MoEFlow/stargazers"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Frepos%2Falgebra-MCX%2FMoEFlow&amp;query=%24.stargazers_count&amp;label=Stars&amp;color=E3B341&amp;style=flat&amp;cacheSeconds=300" alt="MoEFlow stars" /></a>
<a href="https://github.com/algebra-MCX/MoEFlow/forks"><img src="https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.github.com%2Frepos%2Falgebra-MCX%2FMoEFlow&amp;query=%24.forks_count&amp;label=Forks&amp;color=58A6FF&amp;style=flat&amp;cacheSeconds=300" alt="MoEFlow forks" /></a>
</p>
</td>
</tr>
</table>

- **[mini-DeepInfer](https://github.com/algebra-MCX/mini-DeepInfer)**: runs the real DeepSeek-V4.1-Flash on 4 × B200. Every optimization is written up in an issue with its baseline, profile, correctness tests and measured result. [Roadmap](https://github.com/algebra-MCX/mini-DeepInfer/issues/3).
- **[MoEFlow](https://github.com/algebra-MCX/MoEFlow)**: fused Triton kernels, 2× NCCL all-to-all and CUDA Graph decode for MoE expert parallelism on B200.

## Tech stack

<p>
<img src="https://skillicons.dev/icons?i=py,cpp,c,pytorch,linux,bash,git,docker,vscode" alt="Tech stack" />
</p>

## GitHub stats

<table>
<tr>
<td width="50%"><img src="https://github-readme-stats.vercel.app/api?username=algebra-MCX&show_icons=true&theme=github_dark&hide_border=true&include_all_commits=true&hide_rank=true" alt="GitHub stats: commits, PRs, issues, stars" width="100%" /></td>
<td width="50%"><img src="https://streak-stats.demolab.com/?user=algebra-MCX&theme=github-dark-blue&hide_border=true" alt="Contribution streak" width="100%" /></td>
</tr>
</table>

## Contribution graph

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/algebra-MCX/algebra-MCX/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/algebra-MCX/algebra-MCX/output/github-snake.svg" />
  <img alt="Contribution snake" src="https://raw.githubusercontent.com/algebra-MCX/algebra-MCX/output/github-snake.svg" />
</picture>

## Writing

- 知乎, series *解构 DeepInfer*: https://www.zhihu.com/people/zhib1eiazpn
- X: [@Chenxi_Ma_ai](https://x.com/Chenxi_Ma_ai)
- Blog: https://algebra-mcx.github.io/

<div align="center">

shannon20051127@gmail.com

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1F3BFF,100:0B1020&height=110&section=footer" width="100%" alt="" />

</div>
