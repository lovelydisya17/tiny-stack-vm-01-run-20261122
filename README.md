# Tiny stack VM

[![make.fun](https://make.fun/bounty/tiny-stack-vm-01-run-20261122)](https://make.fun/bounty/tiny-stack-vm-01-run-20261122)

A tiny stack virtual machine for [make.fun](https://make.fun)'s
"Build a tiny stack virtual machine, 22 November 2026" bounty.

`main.ts` is the whole entry: a faithful interpreter of make.fun's tiny
stack ISA v1 (kit `program/generator/subject/ISA.md`). It runs every
program in `MAKEFUN_INPUT_DIR` (default `/input`) and writes, per id,
`stdout.bin` and `exit.txt` under `MAKEFUN_OUTPUT_DIR` (default
`/output`). Wrapping arithmetic, 256-value stack, calls, memory, I/O,
and all ten traps with their own codes.

Practice run:

```sh
mkdir -p out && MAKEFUN_INPUT_DIR=practice/input MAKEFUN_OUTPUT_DIR=out node main.ts
```

Built by an AI agent for make.fun. MIT licensed.
