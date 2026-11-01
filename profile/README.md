## Cubyte

Cubyte builds AI agents that run on your own infrastructure and take over the
recurring investigative work that eats your team's time. Your data stays
in-house, and you stay in control.

### Agents

| | |
|---|---|
| **[Collie](https://github.com/cubyte-nl/collie)** | An SRE agent for Linux hosts and Kubernetes clusters. It diagnoses problems over SSH and `kubectl` and, when authorised, fixes them. [More on cubyte.nl](https://cubyte.nl/collie/) |
| **[MOLE](https://github.com/cubyte-nl/mole)** | A security reconnaissance agent. It maps DNS, ports, services, TLS and the web tier of authorised targets, with vulnerability scanning as an explicit opt-in. [More on cubyte.nl](https://cubyte.nl/mole/) |

Both are built on [agent-core](https://github.com/cubyte-nl/agent-core), a shared
Go core for the agent loop, tool registry and LLM client.

### How they stay in bounds

- **Scope is enforced, not suggested.** Every tool call is checked against a
  recorded boundary before it runs, and the check fails closed.
- **The model acts only through tools.** The harness validates and executes
  each call, so the model can't bypass the gate.
- **Bring your own LLM.** Agents work with any OpenAI-compatible endpoint,
  including one you host yourself.
- **Every step is logged.** You can read back what an agent did and why.

### Work with us

Cubyte also offers consulting on Kubernetes, observability and self-hosted AI,
as well as tech lead roles and training. Based in Almelo, the Netherlands.

[cubyte.nl](https://cubyte.nl) · [Consulting](https://cubyte.nl/advies/) · [sven.mollinga@cubyte.nl](mailto:sven.mollinga@cubyte.nl)
