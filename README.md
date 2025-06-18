# LATTE: Layered Attestation for Portable Enclaved Applications

**LATTE** is a framework designed to ensure both security and portability for attesting portable TEE applications. This repository is a prototype implementation, which uses WebAssembly as a portable intermediate representation and supports heterogeneous TEEs such as Intel SGX and RISC-V Penglai.

## 📌 liblatte

**liblatte** is a lightweight, standalone library for implementing layered attestation in portable enclaved applications. The repository includes core APIs for measurement and identity derivation, deployment utilities, and performance evaluation.

## 📌 wasm-micro-runtime-latte

**WAMR (wasm-micro-runtime)** is a lightweight standalone WebAssembly runtime. In this repository, We implemented two WASM APIs : `latte_attest` and `latte_verify`. We also offered example of integrating LATTE into Genann, a minimal artificial neural networks program.

## 📌 linux-sgx-latte & penglai-latte

In these repositories, we selected SGX and Penglai as exemplar heterogeneous TEEs, modified **SGX SDK** (version 2.23) and **Penglai TVM** (commit bf52983) to support our framework.

## 📄 License

The source code of liblatte are released under the Apache license 2.0. Check the file LICENSE for more information.
