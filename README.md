<div align="center">

```
╔══════════════════════════════════════════════════════════════════════════╗
║                                                                          ║
║    ██████╗██╗  ██╗ █████╗ ██████╗  ██████╗                              ║
║    ╚════██╗██║  ██║██╔══██╗██╔══██╗██╔═████╗                            ║
║     █████╔╝███████║███████║██║  ██║██║██╔██║                            ║
║    ██╔═══╝ ██╔══██║██╔══██║██║  ██║████╔╝██║                            ║
║    ███████╗██║  ██║██║  ██║██████╔╝╚██████╔╝                            ║
║    ╚══════╝╚═╝  ╚═╝╚═╝  ╚═╝╚═════╝  ╚═════╝                            ║
║                                                                          ║
║         zero-knowledge privacy for autonomous AI agents                  ║
║                        on Base L2                                        ║
║                                                                          ║
╚══════════════════════════════════════════════════════════════════════════╝
```

</div>

```bash
zhad0@protocol:~$ whoami
```

```
zhad0
privacy infrastructure for the agentic web
building on Base — encrypting the machine economy
```

```bash
zhad0@protocol:~$ cat mission.txt
```

```
AI agents trade, vote, lend, and bridge on-chain.
Every intent is visible. Every strategy is exposed.
MEV bots drain them before execution lands.

ZHAD0 fixes this.

AES-256-GCM encryption shields intent payloads.
RISC Zero ZK proofs verify validity without revealing content.
Ghost Relayers execute on Base with zero leakage.

The agent acts. The chain settles. Nobody watches.
```

```bash
zhad0@protocol:~$ ls -la repos/
```

```
drwxr-xr-x  zhad0-sdk          TypeScript SDK + CLI · @zhad0/sdk
drwxr-xr-x  zhad0-app          React web app · zhad0.io
drwxr-xr-x  zhad0-api          Express 5 + Drizzle ORM API server
drwxr-xr-x  zhad0-eliza        ElizaOS plugin · @zhad0/eliza-plugin
drwxr-xr-x  zhad0-virtuals     Virtuals Protocol adapter · @zhad0/virtuals-adapter
drwxr-xr-x  zhad0-docs         Whitepaper · SDK ref · API ref · Governance
```

```bash
zhad0@protocol:~$ zhad0 status --verbose
```

```
┌─────────────────────────────────────────────────────────────────┐
│  ZHAD0 Protocol — Status                                         │
├──────────────────────────────────┬──────────────────────────────┤
│  AES-256-GCM encryption          │  ● LIVE                      │
│  Intent hash fingerprinting      │  ● LIVE                      │
│  ElizaOS plugin                  │  ● LIVE                      │
│  Virtuals Protocol adapter       │  ● LIVE                      │
│  REST API (Base Sepolia)         │  ● LIVE                      │
│  ZK proofs (RISC Zero)           │  ○ mainnet pending           │
│  Ghost Relay network             │  ○ mainnet pending           │
│  Base L2 execution               │  ○ mainnet pending           │
└──────────────────────────────────┴──────────────────────────────┘
```

```bash
zhad0@protocol:~$ npm install @zhad0/sdk
```

```
added 1 package in 0.4s
```

```bash
zhad0@protocol:~$ node -e "
  const { Zhad0Client } = require('@zhad0/sdk');
  const client = new Zhad0Client();

  client.submitIntent({
    action:   'SWAP',
    tokenIn:  '0x833589fCD6eDb6E08f4c7C32D4f71b54bdA02913',
    tokenOut: '0x4200000000000000000000000000000000000006',
    amountIn: '1000000000',
  }).then(r => console.log('intent:', r.intentHash));
"
```

```
intent: 0x7f3a9c2b1e84d06f5a8c3b7e1d4f9a2c6b8e3d7a1f4c9e2b5d8a3f6c1e7b4d9
```

```bash
zhad0@protocol:~$ cat stack.json
```

```json
{
  "language":   "TypeScript",
  "runtime":    "Node.js + Web Crypto API",
  "crypto":     ["AES-256-GCM", "RISC Zero (WASM)"],
  "chain":      "Base L2 (chain 8453)",
  "frontend":   ["React 18", "Vite", "Wagmi", "shadcn/ui"],
  "backend":    ["Express 5", "Drizzle ORM", "PostgreSQL", "Pino"],
  "frameworks": ["ElizaOS", "Virtuals Protocol", "Coinbase AgentKit"]
}
```

```bash
zhad0@protocol:~$ curl https://zhad0.io
```

```
→  https://zhad0.io
```

```bash
zhad0@protocol:~$ █
```

---

<div align="center">

[![zhad0-sdk](https://img.shields.io/badge/zhad0--sdk-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://github.com/zhad0/zhad0-sdk)
[![zhad0-app](https://img.shields.io/badge/zhad0--app-React-61DAFB?style=flat-square&logo=react&logoColor=black)](https://github.com/zhad0/zhad0-app)
[![zhad0-api](https://img.shields.io/badge/zhad0--api-Express-000000?style=flat-square&logo=express&logoColor=white)](https://github.com/zhad0/zhad0-api)
[![zhad0-eliza](https://img.shields.io/badge/zhad0--eliza-ElizaOS-8B5CF6?style=flat-square)](https://github.com/zhad0/zhad0-eliza)
[![zhad0-virtuals](https://img.shields.io/badge/zhad0--virtuals-Virtuals-10B981?style=flat-square)](https://github.com/zhad0/zhad0-virtuals)
[![zhad0-docs](https://img.shields.io/badge/zhad0--docs-Docs-F59E0B?style=flat-square)](https://github.com/zhad0/zhad0-docs)

[![Base](https://img.shields.io/badge/Base_L2-0052FF?style=flat-square&logo=coinbase&logoColor=white)](https://base.org)
[![License](https://img.shields.io/badge/license-MIT-00d26a?style=flat-square)](https://github.com/zhad0/zhad0-sdk/blob/main/LICENSE)

</div>
