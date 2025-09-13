# 🐍 Serpentes VM

**Serpentes** is an experimental virtual machine for Python, inspired by how GraalVM broadened the JVM.  

It is **not a CPython replacement** — CPython remains Python’s reference interpreter.  
Instead, Serpentes explores a unified, async-first bytecode and sandboxed execution model that runs in two modes:

- **Server:** as an optional runtime for ASGI servers (e.g. Uvicorn, Hypercorn), providing an async-native execution engine for Python web apps.
- **Client:** as a standalone WASM runtime in the browser, powering [Garter](https://github.com/serp-hq/garter), a sandboxed Python dialect.

---

## ✨ Features
- **Unified Bytecode** – derived from Python 3.13, extended with:
  - Async-first instructions
  - Sandboxed opcodes
  - Monadic types
- **Profiles** –
  - **Full Profile**: for Python apps on the server
  - **Sandbox Profile**: for Garter in the browser
- **sRPC (Serpentes RPC)** – built-in mechanism for safe client ↔ server calls.
- **Rust Core** – the VM is implemented in Rust for safety and performance.
- **Dual Targets**:
  - Native binary for server integration with Uvicorn/ASGI
  - WASM build for browser sandbox execution

---

## 📖 Motivation
Python dominates on the server, but struggles to reach the browser.  
Serpentes aims to unify these environments by:
- Providing a common bytecode for both Python and Garter
- Enabling secure sandbox execution in the browser
- Offering async-first semantics that map cleanly to modern event loops
- Allowing drop-in use with ASGI servers

---

## 📚 Resources
- [Org Home (Serp-HQ)](https://github.com/serp-hq)

---

## 🤝 Contributing
We’re in early design stages. Contributions are welcome in:
- VM prototyping in Rust
- ASGI server integration
- WASM runtime experimentation
- Spec drafting and discussion

👉 Join the conversation in [Discussions](https://github.com/serp-hq/serpentes/discussions).

---

## 📜 License
MIT License. See [LICENSE](LICENSE) for details.