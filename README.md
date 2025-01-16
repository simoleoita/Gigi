# GIGI 🤖 A Fork of Eliza

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Gigi Banner" width="100%" />
</div>

<div align="center">

📖 [Documentation](https://elizaos.github.io/eliza/) | 🎯 [Examples](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 README Translations

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Persian](./README_FA.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md) | [Tagalog](./README_TG.md) | [Polski](./README_PL.md) | [Arabic](./README_AR.md) | [Hungarian](./README_HU.md) | [Srpski](./README_RS.md) | [Română](./README_RO.md) | [Nederlands](./README_NL.md) | [Ελληνικά](./README_GR.md)

## 🚩 Overview

<div align="center">
  <img src="./docs/static/img/eliza_diagram.png" alt="Gigi Diagram" width="100%" />
</div>

## ✨ Features

- 🛠️ Full-featured Twitter integration
- 🔗 Support for various models (Llama, Grok, OpenAI, Anthropic, Gemini, etc.)
- 👥 Multi-agent and room support
- 📚 Easily ingest and interact with your documents
- 💾 Retrievable memory and document store
- 🚀 Highly extensible - create your own actions and clients
- 📦 Just works!

## Video Tutorials

[AI Agent Dev School](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 Use Cases

- 🤖 Chatbots
- 🕵️ Autonomous Agents
- 📈 Business Process Handling
- 🎮 Video Game NPCs
- 🧠 Trading

## 🚀 Quick Start

### Prerequisites

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Note for Windows Users:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual) is required.

### Use the Starter (Recommended)

Bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start

### Manually Start Gigi (Only recommended if you know what you are doing)

#### Checkout the latest release

bash
Clone the repository
git clone https://github.com/elizaos/eliza.git
This project iterates fast, so we recommend checking out the latest release
git checkout $(git describe --tags --abbrev=0)
If the above doesn't checkout the latest release, this should work:
git checkout $(git describe --tags git rev-list --tags --max-count=1)

#### Edit the .env file

Copy `.env.example` to `.env` and fill in the appropriate values.
bash
cp .env.example .env

Note: `.env` is optional. If you're planning to run multiple distinct agents, you can pass secrets through the character JSON.

#### Start Gigi

bash
pnpm i
pnpm build
pnpm start
The project iterates fast, sometimes you need to clean the project if you are coming back to the project
pnpm clean



### Interact via Browser

Once the agent is running, you should see the message to run `pnpm start:client` at the end. Open another terminal, move to the same directory, and then run the following command to chat with your agent:


bash
pnpm start:client



Then read the [Documentation](https://elizaos.github.io/eliza/) to learn how to customize your Gigi.

----

### Automatically Start Gigi

The start script provides an automated way to set up and run Gigi:


bash
sh scripts/start.sh


For detailed instructions on using the start script, including character management and troubleshooting, see our [Start Script Guide](./docs/docs/guides/start-script.md).

> **Note**: The start script handles all dependencies, environment setup, and character management automatically.

----

### Modify Character

1. Open `packages/core/src/defaultCharacter.ts` to modify the default character. Uncomment and edit as needed.

2. To load custom characters:
    - Use `pnpm start --characters="path/to/your/character.json"`
    - Multiple character files can be loaded simultaneously.

3. Connect with X (Twitter):
    - Change `"clients": []` to `"clients": ["twitter"]` in the character file to connect with X.

---

#### Additional Requirements

You may need to install Sharp. If you see an error when starting up, try installing it with the following command:


bash
pnpm install --include=optional sharp


---

### Start Gigi with Gitpod

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

---

### Community & Contact

- [GitHub Issues](https://github.com/elizaos/eliza/issues). Best for: bugs you encounter using Gigi, and feature proposals.
- [Discord](https://discord.gg/ai16z). Best for: sharing your applications and hanging out with the community.

## Contributors

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)


