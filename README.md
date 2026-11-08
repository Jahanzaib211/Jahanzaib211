# Jahanzaib Ali

**Founder & Systems Engineer at [AliLabsX](https://alilabsx.com).** Lahore. I build self-hosted AI systems: agent teams, agent sandboxes, local inference, and the commerce platform that pays for them.

I taught myself to build from scratch, and AliLabsX is where that work ships. Everything here is built to run on your own hardware, to refuse when it can't prove it is safe, and to leave evidence you can check.

---

### What I'm building

**[Nova Bots](https://github.com/Jahanzaib211/nova-bots)**: a self-hosted team of long-lived AI bots ([bots.alilabsx.com](https://bots.alilabsx.com)).
Forked from DS Bot (Apache-2.0, by Fei2411), then extended with a multi-tenant portal (HMAC-signed sessions, token tiers, a fail-closed engine gate, one engine container per account), host-folder mounts and a hardened desktop CSP. My own bot team (Tech Lead, Security Reviewer, QA, Gatekeeper) fixes bugs in the product through PRs that carry their evidence. See the [repair log](https://github.com/Jahanzaib211/nova-bots/blob/docs/repair-log/docs/repair-log.md).

**[Nova](https://github.com/Jahanzaib211/nova)**: the agent's computer ([nova.alilabsx.com](https://nova.alilabsx.com)).
A computer-use agent with sub-agents, memory and a sandbox per thread, plus a live view of its Files, Terminal, Editor, Browser, Activity and Review. Built on DeerFlow (MIT) with LangGraph and LangChain.

**[Loco](https://github.com/Jahanzaib211/loco)**: a local inference lab behind one endpoint.
Routing is deterministic. VRAM-gated admission refuses a model with measured numbers instead of running out of memory. Long-term memory only changes when you approve it, and the lab UI has no dependencies.

**Storeloom** (private, commercial): the commerce platform for every kind of brand.
A multi-tenant store and site builder. Each site gets its own database and file store, and it comes with templates, a visual editor, apps, custom domains with automatic HTTPS, and paid publishing.

<details>
<summary>More from the lab</summary>

- **[Exora](https://github.com/Jahanzaib211/exora)**: a self-hosted B2B prospecting CRM. It works from public sources, and every field records where it came from.
- **[Project X](https://github.com/Jahanzaib211/project-x)**: a brokerage core built in dependency order. CI won't promote a module until its upstream modules pass their financial-invariant gates.
- **[Ali Kernel](https://github.com/Jahanzaib211/ali-kernel)**: a single-binary Rust gateway that serves an OpenAI-compatible API, with tools, RAG memory and binary attestation.

</details>

---

### Partner

**Apex Global Tech Solutions**: I also work with Apex as its Platform Engineer.

### How I build

- **Fail closed.** If the GPU can't be measured, Loco admits no model. If a session isn't entitled, Nova Bots gives no engine access. A missing check is treated as a "no".
- **Evidence over claims.** Every "done" names the command that ran and what it printed. Changes go through branches and PRs, never straight to `main`.
- **Agents that ship PRs.** The Nova Bots team reviews, tests and opens pull requests against its own codebase, and a human approves every merge.
- **Self-hosted by default.** Your data stays on your machine, models are your own, and nothing is silently substituted.
- **Credit upstream.** Forks and borrowed designs are named in the README and `NOTICE`.

### Stack

`TypeScript` `JavaScript / Node` `Python` `Rust` · `LangGraph / LangChain` `FastAPI` `Express` `Next.js` · `PostgreSQL` `SQLite` · `Docker` `nginx` `Electron` · local LLMs (`llama.cpp`, OpenAI-compatible APIs)

### Contact

[alilabsx.com](https://alilabsx.com) · [LinkedIn](https://www.linkedin.com/in/jahanzaib-ali-labsx) · [Jahanzaib@alilabsx.com](mailto:Jahanzaib@alilabsx.com)
