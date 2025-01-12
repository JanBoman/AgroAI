# Agro AI 🌾

<div align="center">
  <img src="./docs/static/img/Agro_AI.png" alt="AGRO_AI Banner" width="100%" />
</div>

<div align="center">

📖 [Documentation](https://github.com/JanBoman/AgroAI)
</div>


**Agro AI** is a cutting-edge, decentralized agricultural intelligence solution forked from the powerful AI [elizaOS] (https://github.com/elizaOS/eliza). Leveraging the strengths of robust language models (Llama, Grok, OpenAI, Anthropic, etc.) and integrating Web3 capabilities, Agro AI revolutionizes agriculture by enabling smarter decision-making, seamless collaboration, and transparent data handling.

## ✨ **Key Features**

- 🛠️ **Full-featured Integrations**: Easily connect to Discord, Twitter, Telegram, and other communication platforms for real-time updates and conversations.
- 🔗 **Multi-Model Support**: Works seamlessly with top-performing models such as Llama, Grok, OpenAI, Anthropic, and more.
- 👥 **Multi-Agent and Collaboration Rooms**: Support for multiple AI agents and decentralized collaboration rooms.
- 📚 **Document Ingestion and Interaction**: Upload and interact with documents for AI-powered analysis and insights.
- 💾 **Retrievable Memory and Document Store**: Access previously analyzed data and insights at any time.
- 🚀 **Highly Extensible**: Build custom actions, clients, and workflows to suit your specific agricultural needs.
- ☁️ **Local and Cloud Model Support**: Choose between local deployment or cloud-based models, supporting Llama, OpenAI, Anthropic, Groq, and others.
- 📦 **Plug-and-Play Usability**: No complex setup required—just install and start reaping the benefits.

---

## 🎯 **Use Cases**

- 🤖 **Agro Chatbots**: Provide real-time insights and guidance to farmers, cooperatives, and stakeholders.
- 🕵️ **Autonomous Agro Agents**: Deploy intelligent agents that monitor weather patterns, soil data, and supply chain changes autonomously.
- 🌱 **Plant Health Monitoring and Disease Detection**: Use AI to monitor plant growth and detect early signs of diseases or nutrient deficiencies using IoT sensor data, satellite imagery, and drone footage. Trigger smart contract actions to alert stakeholders or even initiate automated solutions (like drone spraying or watering) to help cure affected plants.
- 📈 **Business Process Automation**: Optimize agricultural workflows, manage inventory, and handle logistics using smart, automated pipelines.
- 🎮 **Virtual Farm Assistants (NPCs)**: Enhance agricultural simulation games or virtual environments with realistic AI-driven non-player characters.
- 🧠 **Agro-Trading Insights**: Leverage AI to analyze market trends, predict pricing, and manage risk in decentralized commodity trading platforms.

---

## 🌐 **Web3 and Decentralization Benefits**

Agro AI harnesses Web3 innovations to ensure transparency, data ownership, and trust:

- **Data Sovereignty**: Farmers own their data and choose how it is shared and monetized.
- **Decentralized Collaborations**: Participate in DAO-driven initiatives and decentralized farming communities.
- **Supply Chain Transparency**: Ensure verifiable and immutable records from farm to fork.
- **Smart Contract Automation**: Trigger payouts, rewards, or alerts using on-chain smart contracts based on real-time AI insights.

Agro AI makes precision farming, transparent food systems, and autonomous agents a reality. By building on elizaos.com’s robust architecture, it provides an unparalleled platform for innovation and growth in the agricultural space.



## 🚀 Quick Start

### Prerequisites

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Note for Windows Users:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual) is required.

### Use the Starter (Recommended)

```bash
git clone https://github.com/JanBoman/AgroAI.git
cd agroai-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

Once the agent is running, you should see the message to run "pnpm start:client" at the end.
Open another terminal and move to same directory and then run below command and follow the URL to chat to your agent.

```bash
pnpm start:client
```

### Manually Start Agro AI (Only recommended if you know what you are doing)

```bash
# Clone the repository
git clone https://github.com/JanBoman/AgroAI.git

# Checkout the latest release
# This project iterates fast, so we recommend checking out the latest release
git checkout $(git describe --tags --abbrev=0)
```

### Edit the .env file

Copy .env.example to .env and fill in the appropriate values.

```
cp .env.example .env
```

Note: .env is optional. If you're planning to run multiple distinct agents, you can pass secrets through the character JSON
Note: .env is optional. If you're planning to run multiple distinct agents, you can pass secrets through the character JSON

### Automatically Start Agro AI

This will run everything to set up the project and start the bot with the default character.

```bash
sh scripts/start.sh
```

### Edit the character file

1. Open `packages/core/src/defaultCharacter.ts` to modify the default character. Uncomment and edit.

2. To load custom characters:
    - Use `pnpm start --characters="path/to/your/character.json"`
    - Multiple character files can be loaded simultaneously
3. Connect with X (Twitter)
    - change `"clients": []` to `"clients": ["twitter"]` in the character file to connect with X

### Manually Start Eliza

```bash
pnpm i
pnpm build
pnpm start

# The project iterates fast, sometimes you need to clean the project if you are coming back to the project
pnpm clean
```

#### Additional Requirements

You may need to install Sharp. If you see an error when starting up, try installing it with the following command:

```
pnpm install --include=optional sharp
```

### Community & contact

- [GitHub Issues](https://github.com/JanBoman/AgroAI). Best for: bugs you encounter using Agro AI, and feature proposals.
