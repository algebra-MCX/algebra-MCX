# Chenxi Ma · 马晨熙

**LLM inference systems**<br>
MoE expert parallelism, GPU scheduling, and distributed serving.

I'm a third-year undergraduate student and a research intern at [UW Systems Lab](https://syslab.cs.washington.edu/), advised by [Baris Kasikci](https://homes.cs.washington.edu/~baris/) and [Arvind Krishnamurthy](https://www.cs.washington.edu/people/faculty/arvind).

[Personal website ↗](https://tech-blog-chi.vercel.app/) · [Technical blog](https://tech-blog-chi.vercel.app/blog/) · [Learning](https://tech-blog-chi.vercel.app/learning/)

<img src="assets/inference-banner.jpg" alt="" width="1440" height="318">

## Top Projects

### <img src="https://tech-blog-chi.vercel.app/assets/vllm-logo.svg" width="22" height="22" alt=""> [vLLM](https://github.com/vllm-project/vllm)

I work on MoE expert parallelism in Model Runner V2, fixing expert routing under dual-batch overlap (DBO) and issues in NIXL-based dispatch.

[Selected vLLM contributions ↗](https://tech-blog-chi.vercel.app/#vllm)

### <img src="https://tech-blog-chi.vercel.app/assets/sglang-logo.svg" width="22" height="22" alt=""> [SGLang](https://github.com/sgl-project/sglang)

I work on expert-routing correctness under two-batch overlap (TBO), ensuring each token's routing record lands in the right row.

[Selected SGLang contributions ↗](https://tech-blog-chi.vercel.app/#sglang)

## Publications

### [TraceLab: Characterizing Coding Agent Workloads for LLM Serving](https://arxiv.org/abs/2606.30560)

Kan Zhu, Mathew Jacob, **Chenxi Ma**, Yi Pan, Stephanie Wang, Arvind Krishnamurthy, Baris Kasikci<br>
*arXiv preprint · 2026*

[Paper](https://arxiv.org/abs/2606.30560) · [Project](https://tracelab.cs.washington.edu/) · [Code](https://github.com/uw-syfi/TraceLab)
