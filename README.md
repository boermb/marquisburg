Systems programmer from Cape Town. I build compilers, runtimes, and language tooling, mostly from scratch, mostly in C99.

![C](https://img.shields.io/badge/C-00599C?style=flat&logo=c&logoColor=white)
![Haskell](https://img.shields.io/badge/Haskell-5D4F85?style=flat&logo=haskell&logoColor=white)
![C++](https://img.shields.io/badge/C++-9C033A?style=flat&logo=cplusplus&logoColor=white)

### [Mettle](https://github.com/The-Mettle-Project) - a systems programming language

My flagship project. A from-scratch systems language written in C99 with no LLVM dependency. The compiler is its own world:

- Custom IR, register allocator, and a native PE linker (no external assembler)
- AVX2 auto-vectorizer and a PTX backend for GPU codegen
- A borrow checker over raw pointers with zero false positives
- A GNN-based ML IR optimizer (`--ml-opt`) that found 54 verified expression simplifications the classical optimizer can't reach
- An explainable optimizer (`--explain`, `@simd!` contracts) and a full LSP

The backend is split into a standalone, frontend-agnostic library, [`mettle-core` / `libmtlc`](https://github.com/The-Mettle-Project), with a `calc` example, CI gate, and embedding docs. On top of it sits `m-c99`, a C99 compiler.

- MLIR crash fix merged upstream into llvm-project (will be doing some more work there in the future)

Compilers, IR design, code generation, GPU programming, LLM inference internals, and low-level systems work.
