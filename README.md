<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0f0c29,50:302b63,100:00f5d4&height=260&section=header&text=AYUSH%20KAUSHIK&fontSize=62&fontColor=ffffff&fontAlignY=40&desc=Founder%20%C2%B7%20AI%20Systems%20Architect%20%C2%B7%20Security%20Researcher&descSize=17&descAlignY=62&animation=twinkling" width="100%" alt="header"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&duration=3000&pause=800&color=00F5D4&center=true&vCenter=true&width=800&lines=Provably+secure+AI+and+blockchain+systems.;Parse.+Analyze.+Verify.+Then+execute.;Securing+AI-written+code+in+under+2ms.;Intent+to+Silicon." alt="typing"/>

<br/><br/>

<a href="https://adumate.in"><img src="https://img.shields.io/badge/FOUNDER-Adumate-00F5D4?style=for-the-badge&labelColor=0f0c29"/></a>
<a href="https://www.linkedin.com/in/ayushh-kaushiq-1a950825a"><img src="https://img.shields.io/badge/LINKEDIN-connect-0077B5?style=for-the-badge&labelColor=0f0c29&logo=linkedin&logoColor=white"/></a>
<a href="https://youtube.com/@ayushkaushik08"><img src="https://img.shields.io/badge/YOUTUBE-How_Computers_Think-FF0000?style=for-the-badge&labelColor=0f0c29&logo=youtube&logoColor=white"/></a>
<a href="https://x.com/o_Ayush_kaushik"><img src="https://img.shields.io/badge/X-@o__Ayush__kaushik-ffffff?style=for-the-badge&labelColor=0f0c29&logo=x&logoColor=white"/></a>

</div>

<br/>

```console
ayush@silicon:~$ whoami
Ayush Kaushik — founder @ Adumate · AI systems architect · security researcher

ayush@silicon:~$ cat thesis.txt
 Autonomous systems (AI agents, blockchains, runtimes) fail at the seams.
 I build the infrastructure from scratch and verify it before it executes.

ayush@silicon:~$ cat research_areas.txt
 [1] AI-code & agent security      stop unsafe agent output before it lands
 [2] Blockchain & crypto security  invariants · consensus · smart-contract safety
 [3] Compilers & VMs               language design · IR · bytecode · codegen
 [4] Autonomous agent systems      multi-agent engineering · orchestration

ayush@silicon:~$ status
 ● shipped    Noteer → Meta Global AI Developer Hackathon 2026 (submitted)
 ● building   Noteer evaluation write-up · AAYU benchmarks
 ● studying   B.Sc. Mathematics (Hons), BRABU · exp. 2027
```

---

## 🧭 Research map

```mermaid
flowchart TB
    T["🎯 Thesis<br/>verify autonomous systems before they execute"]

    subgraph AI["AI & agent security"]
        N["🛡️ Noteer<br/>pre-write code guard + API shield"]
    end
    subgraph BC["Blockchain & crypto security"]
        L["⛓️ neuro-ledger<br/>autonomous blockchain + smart contracts"]
        Q["🔐 quantum-sim<br/>BB84 QKD · Grover"]
    end
    subgraph SYS["Compilers & systems"]
        A["🧠 AAYU"] --> V["⚙️ silicon-vm"]
        OS["💻 yellow-flash-os"]
    end
    subgraph AG["Agent systems"]
        B["🤖 brain-os<br/>multi-agent engineering engine"]
    end

    T --> N
    T --> L
    T --> A
    T --> B
    N -.secures.-> B
    A -.targets.-> V

    classDef n fill:#1b1740,stroke:#00f5d4,color:#fff,stroke-width:2px;
    class T,N,L,Q,A,V,OS,B n;
```
<sub>Edit the arrows to match your real dependencies.</sub>

---

## 🛡️ Flagship — [Noteer](https://github.com/Ghrit-igl/Noteer)
### Dual-pillar AI security: guard code at write time, defend APIs at runtime

<div align="center">

![Latency](https://img.shields.io/badge/CST_scan_median-0.771_ms-00F5D4?style=for-the-badge&labelColor=0f0c29)
![P95](https://img.shields.io/badge/P95-1.583_ms-00F5D4?style=for-the-badge&labelColor=0f0c29)
![Tests](https://img.shields.io/badge/automated_tests-270%2B-00F5D4?style=for-the-badge&labelColor=0f0c29)
![Hackathon](https://img.shields.io/badge/Meta_Global_AI_Hackathon-2026_submission-0081FB?style=for-the-badge&labelColor=0f0c29)

</div>

**Problem.** AI coding agents write unreviewed code straight to disk, and models hallucinate package names that attackers can register ("slopsquatting", USENIX Security 2025). Autonomous crawlers also harvest proprietary APIs.

```mermaid
flowchart LR
    A["AI agent"] --> B["Tree-sitter CST"] --> C["Taint + slopsquatting checks"]
    C --> D["Llama 3.3 ranked fixes"] --> E["Exploit sandbox"] --> F["Clean commit"]
    G["Hostile crawler"] --> H["Edge proxy"] --> I["Llama 3.2 classifier"] --> J["Deception tarpit"]
    F --> K[("Merkle audit store")]
    J --> K
```

| Pillar | Metric | Result | Scope |
|:--|:--|--:|:--|
| Guard | CST scan latency, median / P95 | **0.771 ms / 1.583 ms** | Tree-sitter parse |
| Guard | Insecure rate on bundled demo cases | **100% → 0%** | Sandbox-verified, *not* full CyberSecEval |
| Shield | Precision / recall / F1 | **100% / 100% / 1.000** | **24 labeled sessions**, in-house testbench |
| Shield | Proprietary fields leaked | **0** | Schema minimization + honeypot |
| Shield | Edge proxy P50 latency | **9.61 ms** | Live HTTP testbench |

<sub>Shield results come from a small self-built session set. Next: larger independent evaluation + full CyberSecEval run.</sub>

`Python` `TypeScript` `Tree-sitter` `Meta Llama 3.2 / 3.3` `DPoP (RFC 9449)` `Docker`

---

## ⛓️ Blockchain & crypto security

| Project | What it is | Verification evidence |
|:--|:--|:--|
| [neuro-ledger](https://github.com/Ghrit-igl/neuro-ledger) | Single-file autonomous blockchain with smart contracts | `<property tests / fuzzing / invariants checked: list them>` |
| [quantum-sim](https://github.com/Ghrit-igl/quantum-sim) | Quantum circuit simulator: Bell states, Grover, BB84 QKD | `<test against known analytical results>` |
| [cyber-sentinel](https://github.com/Ghrit-igl/cyber-sentinel) | Autonomous SIEM and packet inspector | `<benchmark / test method>` |

**Security approach:** threat-model first → state the invariants → test them (property-based + fuzzing) → publish the evidence.

<!-- UNCOMMENT WHEN YOU HAVE REAL, PUBLIC REPORTS (audits, contests, bounties, CVEs, CTFs):

### Security research log
| Target | Scope | Category | Result | Report |
|:--|:--|:--|:--|:--:|
| `<protocol>` | `<contracts>` | Audit / Contest / Bounty / CVE | `<severity or rank>` | [link](...) |

Profiles: [Code4rena](...) · [Sherlock](...) · [Cantina](...) · [Immunefi](...)
-->

---

## 🤖 AI systems architecture

| Project | Architecture |
|:--|:--|
| [brain-os](https://github.com/Ghrit-igl/brain-os) | Autonomous multi-agent software-engineering engine. `<agents · orchestration · eval results>` |
| [Noteer](https://github.com/Ghrit-igl/Noteer) | Guard layer for agent output (above) |

---

## ⚙️ Compilers & systems

```mermaid
flowchart LR
    S["Source"] --> P["Lexer · Parser"] --> H["HIR"] --> O["Bytecode optimizer"] --> V["silicon-vm"]
    H --> CL["Cranelift"] --> N["Native"]
    H --> LL["LLVM"] --> N
```

| Project | Role | Evidence |
|:--|:--|:--|
| [AAYU / Intent-to-Silicon](https://github.com/Ghrit-igl/INTENT-TO-SILICON) | Systems language in Rust | `<what compiles today · benchmark vs baseline>` |
| [silicon-vm](https://github.com/Ghrit-igl/silicon-vm) | Bytecode VM, 64-bit NaN-boxing | `<test count · benchmark>` |
| [yellow-flash-os](https://github.com/Ghrit-igl/yellow-flash-os) | Amnesic RAM-only micro-OS (x86_64, Limine, QEMU) | `<boot screenshot>` |

---

## 🚀 Founder

**[Adumate](https://adumate.in)** — AI API rotation and service-discovery platform.
`<users / uptime / requests handled — only real numbers>`

**Teaching:** [How Computers Think — Zero to Research](https://youtube.com/@ayushkaushik08), from silicon gates to neural architectures.

---

<!-- UNCOMMENT WHEN YOU HAVE WRITING / PAPERS:

## 📝 Research notes
| Title | Topic | Link |
|:--|:--|:--|
| `<Noteer evaluation>` | AI-code security | [link](...) |
-->

## 🗺️ Roadmap

```mermaid
timeline
    title Next
    Now : Noteer evaluation on a larger independent set : AAYU benchmark suite
    Next : Full CyberSecEval run for Noteer Guard : Property-based tests and fuzzing for neuro-ledger
    Later : Noteer threat-model write-up : First public security report
```

---

## 📡 Live activity <sub>(auto-updated)</sub>

<!--START_SECTION:activity-->
<!--END_SECTION:activity-->

<details>
<summary><b>🎓 Background</b></summary>

<br/>

B.Sc. Mathematics (Hons), BRABU, expected 2027 · self-taught in systems programming and ML.

</details>

<details>
<summary><b>🤝 Open to</b></summary>

<br/>

AI-security research collaboration · blockchain security · compilers and VMs.
📧 `<your public email>`

</details>

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00f5d4,50:302b63,100:0f0c29&height=140&section=footer" width="100%" alt="footer"/>
