# Hi, I'm Marquis

Systems programmer from Cape Town. I build compilers, runtimes, and language tooling, mostly from scratch, mostly in C99.

## What I'm building

### [Mettle](https://github.com/The-Mettle-Project) - a systems programming language

My flagship project: a from-scratch systems language written in C99 with no LLVM dependency. The compiler is its own world:

- Custom IR, register allocator, and a native PE linker (no external assembler)
- AVX2 auto-vectorizer and a PTX backend for GPU codegen
- A borrow checker over raw pointers with zero false positives
- A GNN-based ML IR optimizer (`--ml-opt`) that found 54 verified expression simplifications the classical optimizer can't reach
- An explainable optimizer (`--explain`, `@simd!` contracts) and a full LSP

The backend is split into a standalone, frontend-agnostic library, [`mettle-core` / `libmtlc`](https://github.com/The-Mettle-Project), with a `calc` example, CI gate, and embedding docs. On top of it sits `m-c99`, a C99 compiler.

## Upstream and open source

- MLIR crash fix merged upstream into llvm-project (set up a full Windows MSVC build of llvm-project for it)

## Tools of the trade

![C](https://img.shields.io/badge/C-00599C?style=flat&logo=c&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=flat&logo=php&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Vulkan](https://img.shields.io/badge/Vulkan-A41E22?style=flat&logo=vulkan&logoColor=white)

Compilers, IR design, code generation, GPU programming, LLM inference internals, and low-level systems work.

## Stats

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=marquisburg&layout=compact&langs_count=8&cache_seconds=86400)

## Off the clock

Member of the SAWMGA and 3 time tournament winner on my Clydesdale-Boerperd, Wallace. StarCraft 2 (Protoss) and Overwatch 2 (Reinhardt). Four dachshunds.
