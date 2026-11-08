<!-- ═══════════════════════ HEADER ═══════════════════════ -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:00f5d4&height=220&section=header&text=AYUSH%20KAUSHIK&fontSize=56&fontColor=ffffff&fontAlignY=38&desc=Systems%20%C2%B7%20Compilers%20%C2%B7%20AI-Code%20Security&descSize=18&descAlignY=58&animation=fadeIn" width="100%" alt="header"/>

<a href="https://github.com/Ghrit-igl">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3200&pause=900&color=00F5D4&center=true&vCenter=true&width=720&lines=I+build+the+foundation+first.;Language+%E2%86%92+VM+%E2%86%92+Security+layer+%E2%86%92+Product.;Rust+%C2%B7+Python+%C2%B7+TypeScript;Intent+to+Silicon." alt="typing"/>
</a>

<br/>

<a href="https://adumate.in"><img src="https://img.shields.io/badge/SITE-adumate.in-00F5D4?style=for-the-badge&labelColor=0f0c29" alt="site"/></a>
<a href="https://www.linkedin.com/in/ayushh-kaushiq-1a950825a"><img src="https://img.shields.io/badge/LINKEDIN-connect-0077B5?style=for-the-badge&labelColor=0f0c29&logo=linkedin&logoColor=white" alt="linkedin"/></a>
<a href="https://youtube.com/@ayushkaushik08"><img src="https://img.shields.io/badge/YOUTUBE-How_Computers_Think-FF0000?style=for-the-badge&labelColor=0f0c29&logo=youtube&logoColor=white" alt="youtube"/></a>
<a href="https://x.com/o_Ayush_kaushik"><img src="https://img.shields.io/badge/X-@o__Ayush__kaushik-ffffff?style=for-the-badge&labelColor=0f0c29&logo=x&logoColor=white" alt="x"/></a>

</div>

<br/>

<!-- ═══════════════════════ WHOAMI ═══════════════════════ -->
```console
ayush@silicon:~$ whoami
Ayush Kaushik — systems & AI-security engineer, founder @ Adumate

ayush@silicon:~$ cat focus.txt
[1] Compilers & VMs      language design · IR · bytecode · codegen
[2] AI-code security     stop unsafe agent output BEFORE it touches disk
[3] Low-level systems    boot · memory · isolation

ayush@silicon:~$ cat philosophy.txt
Build the infrastructure from scratch. Then build products on top of it.

ayush@silicon:~$ status
● building   Noteer eval write-up · AAYU benchmarks
```

---

## 🧭 How my projects connect

```mermaid
flowchart LR
    A["🧠 AAYU<br/>language"] --> B["⚙️ silicon-vm<br/>bytecode VM"]
    B --> C["💻 yellow-flash-os<br/>RAM-only micro-OS"]
    A --> D["🛡️ Noteer<br/>AI-code guard"]
    D --> E["🚀 Adumate<br/>product layer"]
    B --> E

    classDef core fill:#302b63,stroke:#00f5d4,color:#fff,stroke-width:2px;
    class A,B,C,D,E core;
```

> One stack, built bottom-up: **language → runtime → OS → security → product.**

---

## 🔬 Selected work

<table>
<tr>
<td width="50%" valign="top">

### 🛡️ [Noteer](https://github.com/Ghrit-igl/Noteer)
**Pre-write guard for AI coding agents**

Agents write unreviewed code straight to disk. Noteer intercepts it first.

```
agent output
   ↓  Tree-sitter CST
   ↓  taint analysis
   ↓  verdict
write  ✅  /  block  ⛔
```

`Python` `Tree-sitter` `DPoP (RFC 9449)`

**Eval:** `<detection rate> · <false-positive rate> · <dataset>`
**Meta Global AI Developer Hackathon 2026:** `<submitted / result>`

</td>
<td width="50%" valign="top">

### 🧠 [AAYU / Intent-to-Silicon](https://github.com/Ghrit-igl/INTENT-TO-SILICON)
**Systems language in Rust**

```
source → lexer → parser → HIR
       → bytecode optimizer
       → Cranelift / LLVM
```

`Rust` `LLVM` `Cranelift`

**Status:** `<what compiles and runs today>`
**Bench:** `<workload · baseline · result>`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ⚙️ [silicon-vm](https://github.com/Ghrit-igl/silicon-vm)
**Bytecode VM · NaN-boxed 64-bit values**

| Benchmark | Result |
|:--|--:|
| `<fib(35)>` | `<ms>` |
| `<loop 1e8>` | `<ms>` |

`Rust` · JIT: `<status>`

</td>
<td width="50%" valign="top">

### 💻 [yellow-flash-os](https://github.com/Ghrit-igl/yellow-flash-os)
**Amnesic live micro-OS · runs fully in RAM**

x86_64 · Limine bootloader · QEMU

Boots: `<yes / screenshot>`
Implemented: `<paging · shell · ...>`

`Assembly` `C` `Python`

</td>
</tr>
</table>

---

## 🧰 Stack

<div align="center">

![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![LLVM](https://img.shields.io/badge/LLVM-262D3A?style=for-the-badge&logo=llvm&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=for-the-badge&logo=threedotjs&logoColor=white)
![QEMU](https://img.shields.io/badge/QEMU-FF6600?style=for-the-badge&logo=qemu&logoColor=white)

</div>

---

## 📡 Currently

| | |
|:--|:--|
| 🔨 **Building** | Noteer evaluation write-up, AAYU benchmark suite |
| 📚 **Studying** | B.Sc. Mathematics (Hons), BRABU · exp. 2027 |
| 🎬 **Teaching** | [How Computers Think — Zero to Research](https://youtube.com/@ayushkaushik08) |

<details>
<summary><b>🗺️ Roadmap (click to expand)</b></summary>

<br/>

- [ ] Noteer: publish evaluation + threat model
- [ ] AAYU: public benchmark table vs baselines
- [ ] silicon-vm: JIT tier
- [ ] yellow-flash-os: documented boot sequence

</details>

<details>
<summary><b>📬 Contact</b></summary>

<br/>

Open to collaborations on compilers, VMs and AI-code security.
📧 `<your public email>`

</details>

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00f5d4,50:302b63,100:0f0c29&height=120&section=footer" width="100%" alt="footer"/>
