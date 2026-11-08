<!-- ═══════════════════════════ HERO ═══════════════════════════ -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0f0c29,50:302b63,100:00f5d4&height=260&section=header&text=AYUSH%20KAUSHIK&fontSize=62&fontColor=ffffff&fontAlignY=40&desc=Systems%20%C2%B7%20Compilers%20%C2%B7%20AI-Code%20Security&descSize=18&descAlignY=62&animation=twinkling" width="100%" alt="header"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3000&pause=800&color=00F5D4&center=true&vCenter=true&width=760&lines=I+build+the+foundation+first.;Language+%E2%86%92+VM+%E2%86%92+OS+%E2%86%92+Security+%E2%86%92+Product.;Parse.+Analyze.+Verify.+Then+write+to+disk.;Intent+to+Silicon." alt="typing"/>

<br/><br/>

<a href="https://adumate.in"><img src="https://img.shields.io/badge/SITE-adumate.in-00F5D4?style=for-the-badge&labelColor=0f0c29"/></a>
<a href="https://www.linkedin.com/in/ayushh-kaushiq-1a950825a"><img src="https://img.shields.io/badge/LINKEDIN-connect-0077B5?style=for-the-badge&labelColor=0f0c29&logo=linkedin&logoColor=white"/></a>
<a href="https://youtube.com/@ayushkaushik08"><img src="https://img.shields.io/badge/YOUTUBE-How_Computers_Think-FF0000?style=for-the-badge&labelColor=0f0c29&logo=youtube&logoColor=white"/></a>
<a href="https://x.com/o_Ayush_kaushik"><img src="https://img.shields.io/badge/X-@o__Ayush__kaushik-ffffff?style=for-the-badge&labelColor=0f0c29&logo=x&logoColor=white"/></a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=Ghrit-igl&label=PROFILE+VIEWS&color=302b63&style=for-the-badge" alt="views"/>

</div>

<br/>

<!-- ═══════════════════════════ TERMINAL ═══════════════════════════ -->
```console
ayush@silicon:~$ whoami
Ayush Kaushik — systems & AI-security engineer · founder @ Adumate

ayush@silicon:~$ cat research_agenda.txt
 [1] Compilers & VMs       language design · HIR · bytecode · JIT · codegen
 [2] AI-code security      block unsafe agent output BEFORE it touches disk
 [3] Low-level systems     boot · paging · memory isolation · amnesic OS
 [4] Verification          taint flows · invariants · formal checks

ayush@silicon:~$ cat philosophy.txt
 Build the infrastructure from scratch.
 Then build the product on top of it.

ayush@silicon:~$ status
 ● building   Noteer evaluation · AAYU benchmark suite
 ● studying   B.Sc. Mathematics (Hons), BRABU · exp. 2027
 ● teaching   How Computers Think — Zero to Research (YouTube)
```

---

## 🧭 The stack, bottom-up

```mermaid
flowchart TB
    subgraph L1["Layer 1 · Language"]
        A["🧠 AAYU<br/>Intent-to-Silicon language"]
    end
    subgraph L2["Layer 2 · Runtime"]
        B["⚙️ silicon-vm<br/>NaN-boxed bytecode VM"]
    end
    subgraph L3["Layer 3 · System"]
        C["💻 yellow-flash-os<br/>RAM-only micro-OS"]
    end
    subgraph L4["Layer 4 · Security"]
        D["🛡️ Noteer<br/>pre-write AI-code guard"]
    end
    subgraph L5["Layer 5 · Product"]
        E["🚀 Adumate"]
    end
    A --> B --> C
    B --> E
    D --> E

    classDef n fill:#1b1740,stroke:#00f5d4,color:#fff,stroke-width:2px;
    class A,B,C,D,E n;
```

<sub>Edit the arrows to match your real dependencies. A wrong diagram is worse than none.</sub>

---

## 🔬 Flagship #1 — [Noteer](https://github.com/Ghrit-igl/Noteer)
### Pre-write security gate for AI coding agents

**Problem.** Coding agents write code to disk before anyone reviews it. That code can contain injection paths, unsafe calls and hallucinated packages.
**Approach.** Intercept the agent's output, parse it into a CST, run taint analysis, and only then allow the write.

```mermaid
sequenceDiagram
    autonumber
    participant AG as 🤖 AI Agent
    participant NT as 🛡️ Noteer
    participant CST as 🌳 Tree-sitter CST
    participant TA as 🔎 Taint Engine
    participant FS as 💾 Disk

    AG->>NT: proposed code
    NT->>CST: parse (<N> languages)
    CST-->>NT: syntax tree
    NT->>TA: source → sink analysis
    TA-->>NT: findings
    alt clean
        NT->>FS: write ✅
    else risky
        NT-->>AG: blocked ⛔ + reason
    end
```

| Metric | Result | Dataset / Method |
|:--|:--:|:--|
| Detection rate | `<%>` | `<dataset>` |
| False-positive rate | `<%>` | `<dataset>` |
| Latency per file | `<ms>` | `<hardware>` |
| Languages | `<N>` | Tree-sitter grammars |

**Built for:** Meta Global AI Developer Hackathon 2026 · Result: `<submitted / placed>`
`Python` `Tree-sitter` `DPoP (RFC 9449)` `Llama`

---

## ⚙️ Flagship #2 — [AAYU / Intent-to-Silicon](https://github.com/Ghrit-igl/INTENT-TO-SILICON)
### A systems language in Rust

```mermaid
flowchart LR
    S["📄 Source"] --> LX["Lexer"] --> P["Parser"] --> H["HIR"]
    H --> O["Bytecode<br/>optimizer"]
    O --> V["silicon-vm"]
    H --> CL["Cranelift"]
    H --> LL["LLVM"]
    CL --> N["⚡ Native"]
    LL --> N
```

```text
// <paste a REAL 6–10 line AAYU snippet here. Code speaks louder than adjectives.>
```

| Benchmark | AAYU | Baseline | Notes |
|:--|:--:|:--:|:--|
| `<fib(35)>` | `<ms>` | `<Python/Lua ms>` | `<machine>` |
| `<loop 1e8>` | `<ms>` | `<…>` | `<…>` |

**Status:** `<what compiles and runs today, plainly>`

---

## 🧱 More systems work

<table>
<tr>
<td width="50%" valign="top">

### [silicon-vm](https://github.com/Ghrit-igl/silicon-vm)
64-bit IEEE-754 **NaN-boxing**, bytecode VM in Rust.
JIT: `<status>` · Tests: `<N>`

`Rust`

</td>
<td width="50%" valign="top">

### [yellow-flash-os](https://github.com/Ghrit-igl/yellow-flash-os)
Amnesic **volatile-RAM** live micro-OS. x86_64, Limine, QEMU.
Boots: `<yes + screenshot>` · Implemented: `<paging / shell / …>`

`Assembly` `C` `Python`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### [aayu-mobile-ide](https://github.com/Ghrit-igl/aayu-mobile-ide)
Touch-first web IDE for AAYU. React 19 · TypeScript · Monaco.

`TypeScript` `PWA`

</td>
<td width="50%" valign="top">

### [portfolio](https://github.com/Ghrit-igl/portfolio)
Interactive 3D portfolio. React 19 · Three.js · Vite.

`TypeScript` `Three.js`

</td>
</tr>
</table>

---

## 🧰 Toolbox

<div align="center">

![Rust](https://img.shields.io/badge/Rust-000?style=for-the-badge&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![LLVM](https://img.shields.io/badge/LLVM-262D3A?style=for-the-badge&logo=llvm&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Three.js](https://img.shields.io/badge/Three.js-000?style=for-the-badge&logo=threedotjs&logoColor=white)
![QEMU](https://img.shields.io/badge/QEMU-FF6600?style=for-the-badge&logo=qemu&logoColor=white)

</div>

---

## 🗺️ Roadmap

```mermaid
timeline
    title Where this is going
    Now : Noteer evaluation write-up : AAYU benchmark suite
    Next : silicon-vm JIT tier : Documented boot sequence for yellow-flash-os
    Later : Noteer threat model paper : AAYU language spec v1
```

---

## 📡 Live activity <sub>(auto-updated)</sub>

<!--START_SECTION:activity-->
<!--END_SECTION:activity-->

<div align="center">

<img src="https://raw.githubusercontent.com/Ghrit-igl/Ghrit-igl/output/github-snake-dark.svg" alt="contribution snake" width="100%"/>

</div>

---

<details>
<summary><b>🎓 Background</b></summary>

<br/>

- B.Sc. Mathematics (Hons), BRABU — expected 2027
- Self-taught in systems programming and ML
- Creator of the YouTube series *How Computers Think — Zero to Research*

</details>

<details>
<summary><b>🤝 Open to</b></summary>

<br/>

Collaboration on compilers, VMs, AI-code security and verification.
📧 `<your public email>`

</details>

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00f5d4,50:302b63,100:0f0c29&height=140&section=footer" width="100%" alt="footer"/>
