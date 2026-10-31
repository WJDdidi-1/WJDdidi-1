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
- Coursework and older experiments are public too — robotics, graph ML, network
  simulation — each with the README saying what is real and what was never finished.

<sub>Tools above are MIT / Apache-2.0. Issues and pull requests are welcome.</sub>
