# kilocode-rules

Opinionated configuration for [Kilo Code](https://kilocode.ai/) — a local AI coding agent in VS Code. This repo contains system prompts, rules, and custom mode setups that shape how Kilo Code interacts with your codebase.

---

## ⚠️ Disclaimers

* This setup is **opinionated**. If you're looking for stable or beginner-friendly templates, start here - [rules_template](https://github.com/Bhartendu-Kumar/rules_template).
* Want to use a similar setup with **Roo Code** or **Cline**? That link works for those too.
* Designed for **solo dev workflows**, not teams.
* Changes often; no stability guaranteed.

---

## ⚙️ What This Repo Contains

- `rules/` & `rules-*` – structured prompts for behavior control
- `system-prompt-*` – main system instructions
- `modes.yaml` – custom modes (`Chat`, `Write`, `MCP`)
- Bun-based runtime setup (see [Why Bun?](#why-bun))
- Minimal dependencies, zero TypeScript scaffolding

This repo assumes you know what you're doing. Defaults are heavily customized and may break at any time.

---

## 📦 How to Use These Rules

1. Clone into your project root:

```bash
cd your-project-root
git clone https://github.com/shanefully-done/kilocode-rules.git
````

2. Rename the directory so Kilo Code can detect it:

```bash
mv kilocode-rules .kilocode
```

3. Kilo Code will automatically detect `.kilocode` and apply the rules.

---

## 🧠 Modes: Chat, Write, MCP

This setup includes three custom modes:

* `Chat` – The default mode. All prompts should *start* and *end* in this mode.
* `Write` – Optimized for content or code generation. Use sparingly.
* `MCP` – Model Context Protocol integration. Advanced; use only if you're bridging external context.

> Mode configurations are in [`modes.yaml`](./modes.yaml).
> See Kilo Code’s [Custom Modes Guide](https://kilocode.ai/docs/features/custom-modes#custom-mode-configuration-json-format) for full specs.

---

## ⚡ Why Bun?

This repo is configured to run under [Bun](https://bun.sh/) instead of npm or pnpm:

* Faster install and runtime
* Native TypeScript + file watcher
* Cleaner scripts

If you're not using Bun, install it first:

```bash
curl -fsSL https://bun.sh/install | bash
```

---

## 🙏 Credits

* Base prompt structure and configuration largely forked from [`rules_template`](https://github.com/Bhartendu-Kumar/rules_template)

---

## 🧪 Tips

* Keep prompts minimal and specific.
* Always route back to `Chat` mode to avoid dead-end threads.
* Disable conflicting VS Code extensions (like Copilot) for clean integration.
