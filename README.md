# Hi, I'm Chenxi Ma 👋

**LLM inference infrastructure · GPU kernels · distributed systems**
Based in Beijing. I build and write about how large models are served fast.

## What I work on

- **MoE serving:** expert parallelism, dispatch / combine, communication–compute overlap
- **GPU kernels:** Triton fused kernels, CUDA Graph decode, tensor-core attention
- **Engines:** I read production inference engines closely, rebuild their core modules, and measure every change

## vLLM

I contribute to [vLLM](https://github.com/vllm-project/vllm), mainly on the MRV2 / DBO path for MoE and NIXL dispatch. Two of my PRs have been approved by maintainers and are on their way into `main`.

| PR | What it does | Status |
| --- | --- | --- |
| [#63476](https://github.com/vllm-project/vllm/pull/63476) | `[Bugfix][MRV2]` Report the first failed DBO microbatch | Approved, auto-merge enabled |
| [#63372](https://github.com/vllm-project/vllm/pull/63372) | `[Bugfix][MRV2]` Keep routed-expert rows of every DBO microbatch | Approved |
| [#63485](https://github.com/vllm-project/vllm/pull/63485) | `[Perf][MoE]` Size NIXL dispatch from synchronized execution slices | In review |

All my vLLM PRs: [`author:algebra-MCX`](https://github.com/vllm-project/vllm/pulls?q=is%3Apr+author%3Aalgebra-MCX)

## Projects

- **[mini-DeepInfer](https://github.com/algebra-MCX/mini-DeepInfer)**: a minimal, readable re-implementation of DeepInfer's core inference engine design. Runs the real DeepSeek-V4.1-Flash on 4 × B200. Every optimization is written up in an issue with its baseline, profile, correctness tests and measured result. [Roadmap](https://github.com/algebra-MCX/mini-DeepInfer/issues/3).
- **[MoEFlow](https://github.com/algebra-MCX/MoEFlow)**: MoE expert parallelism for vLLM, with fused Triton kernels, 2× NCCL all-to-all and CUDA Graph decode on B200.

## Writing

- 知乎, series *解构 DeepInfer*: https://www.zhihu.com/people/zhib1eiazpn
- X: [@Chenxi_Ma_ai](https://x.com/Chenxi_Ma_ai)
- Blog: https://algebra-mcx.github.io/

## Contact

shannon20051127@gmail.com
