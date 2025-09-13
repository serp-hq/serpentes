# 🐍 Serpentes VM

**Serpentes** is a unified virtual machine for executing both **Python** and **Garter** code.  
It defines a shared bytecode, execution semantics, and host API bindings — ensuring compatibility across servers, desktops, and browsers.

---

## ✨ Features
- **Unified Bytecode** – Derived from Python 3.13, extended with:
  - Async-first instructions
  - Monadic types
  - Sandbox opcodes
- **Profiles** –  
  - **Full Profile**: for Python on server/desktop  
  - **Sandbox Profile**: for Garter in the browser
- **Built-in sRPC** – Secure RPC for browser ↔ server calls.
- **WebAssembly-first** – Runs in WASM or native runtimes.

---

## 📖 Motivation
Python’s current VM (CPython) is powerful but not portable.  
With the rise of **Garter** (Python in the browser), we need a common runtime to:  
- Eliminate mismatches between server and client execution.  
- Provide standard RPC and sandboxing.  
- Enable long-term cross-environment optimizations.  

---

## 📚 Resources
- [Draft PEP: Serpentes](https://github.com/serp-hq/serp-serpentes/blob/main/PEP_YYYY_Serpentes.pdf)  
- [Org Home (Serp-HQ)](https://github.com/serp-hq)  

---

## 🤝 Contributing
We’re in early design stages. Contributions are welcome in:  
- Spec drafting  
- VM prototyping  
- WASM runtime experimentation  

👉 Join the conversation in [Discussions](https://github.com/serp-hq/serp-serpentes/discussions).  

---

## 📜 License
MIT License. See [LICENSE](LICENSE) for details.
