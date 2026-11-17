# Less yak shaving. More things that work.

An agent can write a thousand lines before lunch. Cool. Did anyone need them?

That's the question I keep coming back to — in coding tools, automation, and robots that eventually have to deal with the real world.

### A few hills I'll die on

**Context is a budget. Spend it like it's yours.**  
Dumping the whole repo into a model isn't a strategy. It's a very expensive way to say “good luck, bestie.”

**The best feature might be a deleted feature.**  
If a tool quietly fixes the annoying part and gets out of the way, that's a W. Every background job does not need its own dashboard cinematic universe.

**Autonomy needs boundaries.**  
Give an agent a clear goal, a way to check its work, and a stopping point. “Keep improving” is how you wake up to six abstractions and a settings page nobody asked for.

**Ship small. Bring receipts.**  
A demo gets attention. A reproducible result earns trust. If it only works on my machine, the plot is still developing.

**Reality gets the final code review.**  
A robot doesn't care how convincing the explanation sounds. Neither does a broken install. Measure what happened, learn from the failure, try again.

### Turning those takes into tools

| Rabbit hole | Something to try |
| --- | --- |
| Agents eating context like it's an all-you-can-eat buffet | [**ai-context-doctor**](https://github.com/WJDdidi-1/ai-context-doctor) — find context-heavy files and generate ignore rules. |
| Plugins that install successfully and then do absolutely nothing | [**dsh-plugin-toolkit**](https://github.com/WJDdidi-1/dsh-plugin-toolkit) — check the package and loader path before release day becomes debugging day. |
| Tutorials that need a tutorial | [**dsh-plugin-example**](https://github.com/WJDdidi-1/dsh-plugin-example) — a small plugin to read, copy, and mess with. |

```sh
npx ai-context-doctor --json
npx dsh-plugin-toolkit verify .
```

### Still curious, still tinkering

Language becoming action. Humans staying in the loop. Systems that know when to stop.  
The interesting bit is where a neat idea meets a messy constraint.

Some earlier rabbit holes: [language-guided robot simulation](https://github.com/WJDdidi-1/Smart-Robotic-Car-with-LLM-Interaction), [human–robot interaction](https://github.com/WJDdidi-1/HRI_NaoHospital), and [learning on graphs](https://github.com/WJDdidi-1/GML-Machine-Learning-On-Graphs). Check each repo for what actually runs.

---

Got a reproducible bug, a simpler approach, or a take worth challenging? Open an issue. I'm listening.

[Elsewhere on the web ↗](https://wjddidi-1.github.io)
