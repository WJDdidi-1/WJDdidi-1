### Hi, I'm WJDdidi-1.

I build small, sharp tools for people who run coding agents — the kind of tools that
answer one question well instead of five questions badly.

**中文**：我做一些「小而准」的工具，主要解决智能体（AI coding agent）上下文与插件
生态里的具体问题。下面每个项目都写清了「现在能跑什么、还没做什么」。

---

## What I'm working on

| Project | What it does | Why it exists |
| --- | --- | --- |
| **[ai-context-doctor](https://github.com/WJDdidi-1/ai-context-doctor)** <br>`npx ai-context-doctor` | Tells you which files in a repo would flood your agent's context, and writes the ignore rules that stop it. Ships a DeepSeek Harness panel (`dsh-aiignore`). | Agents read a 40 KB lockfile once and pay for it in every turn after. |
| **[dsh-plugin-toolkit](https://github.com/WJDdidi-1/dsh-plugin-toolkit)** <br>`npx dsh-plugin-toolkit verify .` | Preflight for DeepSeek Harness plugins: pack the tarball, install it, import the entry the loader mounts, mount the panel — before you tag a release. Also `init`, `dev`, `release`. | A plugin can install cleanly and still do nothing. I shipped five of those bugs; the checks now catch all five. |
| **[dsh-plugin-example](https://github.com/WJDdidi-1/dsh-plugin-example)** | A ~70-line plugin you can read in one sitting and copy. | Every plugin tutorial starts with a 400-line skeleton. |

```sh
npx ai-context-doctor --json          # what would flood the context
npx dsh-plugin-toolkit verify .       # will this plugin actually install?
```

---

## How I work

- **Every claim has a check behind it.** If a README says "tested", there is a test
  file you can run; if it says "works with X", CI runs X.
- **Write down the failure.** [Five plugins that installed and did nothing](https://github.com/WJDdidi-1/dsh-plugin-toolkit/blob/main/docs/why-it-exists.md)
  documents five real bugs — the exact error text, the root cause, and the check that
  catches each one now. Two of those were mine.
- **Say what is not built yet.** The READMEs separate *what runs today* from *what is
  planned*, because a README that promises more than the code is the most expensive
  kind of debt.

---

## Elsewhere

- Personal site: **[wjddidi-1.github.io](https://wjddidi-1.github.io)**

## Coursework and older projects

Public, and each README separates what runs from what was never finished:

| Project | What it is | State |
| --- | --- | --- |
| [Smart-Robotic-Car-with-LLM-Interaction](https://github.com/WJDdidi-1/Smart-Robotic-Car-with-LLM-Interaction) | "Hey car, come here" → intent → motion, in a simulator | 31 tests, path drawn from the run |
| [HRI_NaoHospital](https://github.com/WJDdidi-1/HRI_NaoHospital) | NAO receptionist: expression recognition, dialogue, Dijkstra routing | planner tested; robot parts need NAOqi |
| [NetworkFinal](https://github.com/WJDdidi-1/NetworkFinal) | Traffic classification with differential privacy | results table, including the worst ε |
| [GML-Machine-Learning-On-Graphs](https://github.com/WJDdidi-1/GML-Machine-Learning-On-Graphs) | ASL recognition from skeleton graphs (GNN) | pipeline only; no accuracy claimed |
| [chat-web](https://github.com/WJDdidi-1/chat-web) | Small chat UI with a documented event protocol | the CORS bug it fixed is written down |
| [TensorflowBasic](https://github.com/WJDdidi-1/TensorflowBasic) · [CPS](https://github.com/WJDdidi-1/CPS) · [Tips-for-Github](https://github.com/WJDdidi-1/Tips-for-Github) | Notes: TensorFlow basics, LTL specs, Git commands | cheat sheets, not tutorials |

<sub>Tools above are Apache-2.0 / Apache-2.0. Issues and pull requests are welcome.</sub>
