# cann-repos

CANN-related GitCode repos bundled as submodules.

**Install Git LFS first** — [`asc-devkit`](https://gitcode.com/cann/asc-devkit.git) uses LFS; without it, large files will be pointer stubs.

```bash
git lfs install   # after installing git-lfs (apt/brew)
```

## Clone

```bash
git clone --recurse-submodules https://github.com/learning-chip/cann-repos.git
```

If you already cloned without submodules, or after `git pull`:

```bash
git submodule update --init --recursive
```

Track each submodule's latest commit on its configured branch (local only; does not update pinned SHAs in this repo):

```bash
git submodule update --remote --recursive
```

## Submodules

| Directory | Upstream |
|-----------|----------|
| `cann-recipes-infer` | https://gitcode.com/cann/cann-recipes-infer.git |
| `cann-samples` | https://gitcode.com/cann/cann-samples.git |
| `ops-transformer` | https://gitcode.com/cann/ops-transformer.git |
| `ops-nn` | https://gitcode.com/cann/ops-nn.git |
| `op-plugin` | https://gitcode.com/Ascend/op-plugin.git |
| `asc-devkit` | https://gitcode.com/cann/asc-devkit.git |
| `pto-isa` | https://gitcode.com/cann/pto-isa.git |
| `cannbot-skills` | https://gitcode.com/cann/cannbot-skills.git |

## Also relevant repos, not added as submodule yet

| Repo | Upstream |
|------|----------|
| catlass | https://gitcode.com/cann/catlass |
| cann-recipes-train | https://gitcode.com/cann/cann-recipes-train |
| torchtitan-npu | https://gitcode.com/cann/torchtitan-npu |
| ops-math | https://gitcode.com/cann/ops-math |
| ops-collections | https://gitcode.com/cann/ops-collections |
| pytorch (Ascend) | https://gitcode.com/Ascend/pytorch |
| vllm-ascend | https://github.com/vllm-project/vllm-ascend |
| sgl-kernel-npu | https://github.com/sgl-project/sgl-kernel-npu |
