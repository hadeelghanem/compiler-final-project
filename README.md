# 🧠 Principles of Compilation – Final Project

This repository contains my final project for the **Principles of Compilation** course.  
The project implements a **Scheme-to-Assembly compiler**, written in **OCaml**, with supporting assembly routines for runtime operations.

---

## 📘 Overview

The compiler translates a subset of the Scheme programming language into x86 Assembly.  
It includes code generation, primitive procedure support, and runtime handling through assembly-level implementations.

The project builds upon the assignments from previous stages of the course and combines them into a complete compiler pipeline.

---

## 🧩 Project Structure

| File | Description |
|------|--------------|
| `compiler.ml` | The main compiler file — includes parsing, semantic analysis, and code generation. |
| `pc.ml` | Parser combinator utilities used for the lexical and syntactic analysis. |
| `prologue-1.asm` | First assembly segment – defines macros and runtime setup before generated code. |
| `prologue-2.asm` | Second assembly segment – includes additional runtime definitions. |
| `epilogue.asm` | Final assembly segment – defines primitive operations and final runtime behavior. |
| `init.scm` | Contains definitions for built-in Scheme functions that are prepended to user code. |
| `makefile` | Automates the build process for compiling the compiler and assembling output. |

---

## ⚙️ How to Build and Run

### 1. Build the Compiler
To compile and link all components, run:
```bash
make
