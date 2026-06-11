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

Track each submodule's latest commit on its configured branch (local only):

```bash
git submodule update --remote --recursive
```

Bump the pinned SHAs in this repo and commit:

```bash
git submodule update --remote --recursive && git add -u && git commit -m "Bump submodule SHAs"
```

## Submodules

| Directory | Upstream |
|-----------|----------|
| `ops-transformer` | https://gitcode.com/cann/ops-transformer.git |
| `ops-nn` | https://gitcode.com/cann/ops-nn.git |
| `op-plugin` | https://gitcode.com/Ascend/op-plugin.git |
| `asc-devkit` | https://gitcode.com/cann/asc-devkit.git |
| `pto-isa` | https://gitcode.com/cann/pto-isa.git |
| `cannbot-skills` | https://gitcode.com/cann/cannbot-skills.git |
| `cann-samples` | https://gitcode.com/cann/cann-samples.git |
| `cann-recipes-infer` | https://gitcode.com/cann/cann-recipes-infer.git |

## Also relevant repos, not added as submodule yet

| Type | Repo | Upstream |
|------|------|----------|
| More kernels | catlass | https://gitcode.com/cann/catlass |
| | ops-collections | https://gitcode.com/cann/ops-collections |
| | ops-math | https://gitcode.com/cann/ops-math |
| | sgl-kernel-npu | https://github.com/sgl-project/sgl-kernel-npu |
| Communication | hccl | https://gitcode.com/cann/hccl |
| | hcomm | https://gitcode.com/cann/hcomm |
| | shmem | https://gitcode.com/cann/shmem |
| | catccos | https://gitcode.com/cann/catccos |
| Framework | cann-recipes-train | https://gitcode.com/cann/cann-recipes-train |
| | torchtitan-npu | https://gitcode.com/cann/torchtitan-npu |
| | pytorch (Ascend) | https://gitcode.com/Ascend/pytorch |
| | vllm-ascend | https://github.com/vllm-project/vllm-ascend |
