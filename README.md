# La Tanda — Web3 Ecosystem of Honduras

> **Not an app. An ecosystem.**
> Red social + tandas digitales + marketplace + minería + blockchain propia.

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)
[![Chain](https://img.shields.io/badge/chain-latanda--testnet--1-00d4ff)](https://latanda.online/chain/)
[![Supply](https://img.shields.io/badge/supply-200M%20LTD%20fijo-ffd700)](https://latanda.online/whitepaper.html)
[![Inflation](https://img.shields.io/badge/inflation-0%25-22c55e)](https://latanda.online/whitepaper.html)
[![Mainnet](https://img.shields.io/badge/mainnet-Q1%202027-8b5cf6)](https://latanda.online/chain/)

This repository is the **public mirror** of the La Tanda frontend — the first sovereign Web3 ecosystem built in Honduras for Latin America.

> **Developer note:** This is a pure HTML/CSS/JS frontend (no build step). See **Development Setup** below to run locally.

---

## 🌐 What is La Tanda

La Tanda is a **Web3 ecosystem with 7 integrated layers**, not a simple savings app. The tandas (rotating savings ROSCA groups) are ONE of the 7 layers. Think of it as Amazon to e-commerce: much more than a cardboard box.

La Tanda es un **ecosistema Web3 con 7 capas integradas**, no una simple app de tandas. Las tandas (grupos de ahorro rotativo ROSCA) son UNA de las 7 capas. Piénsalo como Amazon al e-commerce: mucho más que una caja de cartón.

### Las 7 capas del ecosistema

| # | Capa | Qué hace |
|---|---|---|
| 1 | 💬 **Red Social** | Feed, stories, comentarios, reacciones. Tu tiempo genera reputación on-chain. |
| 2 | 🔄 **Tandas Digitales** | Grupos de ahorro rotativo 0% comisión, score on-chain, préstamos integrados |
| 3 | 🛍️ **Marketplace Web3** | Productos, servicios, bookings. Seller Score on-chain. Pagos en lempiras o LTD |
| 4 | ⛏️ **Minería de LTD** | 5 tiers (1-12 LTD/día), cap 500 LTD/día global, gana por actividad real |
| 5 | ⭐ **Reputación On-Chain** | Score financiero unificado 300-850, portable entre capas, anclado en blockchain |
| 6 | 🔗 **La Tanda Chain** | Blockchain soberana Cosmos SDK + CometBFT, 200M LTD fijo, 0% inflación |
| 7 | 🤖 **MIA AI** | Asistente financiero con 16 capacidades (Groq Llama 3.3 70B) |

---

## 📊 Estado actual (live en testnet)

| Métrica | Valor actual |
|---|---|
| **Usuarios activos mensuales** | 15,000+ |
| **Tandas activas** | 300+ |
| **Validadores de chain** | 13+ |
| **API endpoints en producción** | 160+ |
| **Algoritmos productivos** | 14 (fraud, ranking, credit, salud, etc.) |
| **Propuestas de gobernanza pasadas** | 2 (GOV-001, GOV-002) |
| **Uptime testnet desde Q1 2026** | 100% (sin incidentes de consenso) |

Toda métrica es verificable contra datos on-chain o el dev portal público.

---

## 💎 Tokenomics (200M LTD fijo)

**Modelo**: Supply fijo + Treasury pre-acuñado (similar a THORChain), **cero inflación real**.

### Distribución (10 pools)

| Pool | % | Amount | Uso |
|---|---|---|---|
| Comunidad y Minería | 30% | 60M LTD | Recompensas usuarios, Incentivized Testnet |
| Staking y Validadores | 20% | 40M LTD | Rewards pre-acuñados (APY 15-25%, ~8 años) |
| Fondo de Desarrollo | 12% | 24M LTD | 6 meses cliff + 3 años linear |
| Equipo y Fundadores | 12% | 24M LTD | 1 año cliff + 2 años linear |
| Marketing y Alianzas | 6% | 12M LTD | Trimestral por hitos |
| Seed Round | 5% | 10M LTD | $0.02/LTD, 6mo cliff + 18mo linear |
| Strategic / Private | 5% | 10M LTD | $0.03/LTD, 3mo cliff + 12mo linear |
| Liquidez Inicial TGE | 5% | 10M LTD | DEX pools + listings |
| Bug Bounties y Grants | 3% | 6M LTD | Via governance |
| Fondo de Seguro | 2% | 4M LTD | Emergency governance vote |
| **TOTAL** | **100%** | **200M LTD** | |

**Post-Staking-Pool sustainability** (post año 8): 6 fuentes redundantes incluyendo **marketplace commission routing (0.5% GMV → validadores)** — un revenue stream único vs cadenas pure store-of-value.

Tokenomics completa: [Whitepaper v2.0](https://latanda.online/whitepaper.html) · [Página interactiva](https://latanda.online/ltd-token-economics.html)

---

## 🔗 La Tanda Chain

Blockchain soberana construida con **Cosmos SDK + CometBFT**, específicamente diseñada para fintech comunitaria en Latinoamérica.

- **Chain ID (testnet)**: `latanda-testnet-1`
- **Token**: LTD (denom `ultd`, 1 LTD = 1,000,000 ultd)
- **Address prefix**: `ltd`
- **Block time**: ~5 segundos
- **Consensus**: CometBFT (BFT, Delegated Proof of Stake)
- **Validators activos**: 13+ (genesis, PRO Delegators, drops, UTSA/lesnik, OwlStake, StakerHouse, ANODE.TEAM, AlxVoy, VALIDARIOS, narkosha, oleg1, +community)
- **Governance**: activa, 2 props pasadas
- **Mainnet**: Q1 2027 planificado
- **Explorer (community)**: https://exp.utsa.tech/latanda/staking

### Incentivized Testnet Program

Reservados ~100K LTD para validadores que se suman antes del mainnet:

| Tier | Slots | Reward al genesis |
|---|---|---|
| Infra Partner | 5 (4 ocupados) | 5,000 LTD |
| Validator | 10 | 2,000 LTD |
| Full Node | 20 | 500 LTD |
| Bug Reporter | abierto | 100-1,000 LTD |

**Cómo sumarte**: [Node Operator Guide](./la-tanda-chain-node-guide.md) (si está en este repo) o [latanda.online/chain](https://latanda.online/chain/)


---

## 🛠️ Development Setup

### Prerequisites

- **Node.js 18+** (or any static file server)
- A modern browser (Chrome, Firefox, Edge)
- Git

### Local Development

Since this is a pure HTML/CSS/JS frontend (no build step), serving it locally is straightforward:

```bash
# Clone the repository
git clone https://github.com/INDIGOAZUL/la-tanda-web.git
cd la-tanda-web

# Option A: Using npx (recommended, no global install)
npx serve .

# Option B: Using Python (if you don't have Node.js)
python3 -m http.server 8000

# Option C: Using VS Code Live Server extension
# Right-click index.html → "Open with Live Server"
```

Then open `http://localhost:3000` (or `http://localhost:8000` for Python) in your browser.

### Development Notes

- **No build step needed** — edit `.html`, `.css`, or `.js` files directly and refresh
- **Auth tokens** use `localStorage.getItem('auth_token')` (snake_case)
- **All user data** in HTML must use `escapeHtml()` for XSS safety
- **UI text** should be in Spanish, **code** in English
- **API endpoints** can be tested via the [Swagger UI](https://latanda.online/docs)
- Before committing, verify no `console.log()` remains in production code
- Never commit `.env` files or credentials (see `.env.example`)

### Verifying Your Setup

1. Open `http://localhost:3000` — you should see the La Tanda landing page
2. Navigate to `http://localhost:3000/dev-dashboard.html` — Dev Portal should load
3. Check API connectivity at `http://localhost:3000/docs` — Swagger UI should render


---

## 🚀 Quick Start

### Para usuarios (no technical)
1. Ve a [latanda.online](https://latanda.online)
2. Crea tu cuenta (email o Google Sign-In)
3. Únete a una tanda, publica en el feed, mina LTD, explora el marketplace

### Para desarrolladores (integrar con La Tanda API)
1. Documentación API: https://latanda.online/docs
2. Dev portal: https://latanda.online/dev-dashboard.html
3. Autenticación: JWT via `/api/auth/login`
4. 160+ endpoints productivos

### Para validadores (correr un nodo)
1. Lee la guía: [la-tanda-chain-node-guide.md](https://latanda.online/la-tanda-chain-node-guide.md)
2. Instalación one-line: `wget -q https://latanda.online/chain/node-setup.sh -O node-setup.sh && chmod +x node-setup.sh && ./node-setup.sh`
3. Chain page con seeds: https://latanda.online/chain/
4. Únete al Incentivized Testnet Program enviando 10 LTD testnet + create-validator tx

---

## 📂 Repository Structure

```
la-tanda-web/
├── *.html                    # Ecosystem pages (60+ HTML files — pages, admin panels, tools)
├── css/                      # Stylesheets (design tokens, components, modules)
├── js/                       # JavaScript modules (components-loader, hub, utilities)
├── assets/                   # Images, logos, favicons
├── chain/                    # La Tanda Chain resources (node-setup.sh, genesis.json)
├── docs/                     # OpenAPI specification + Swagger UI
├── .github/                  # Bounty templates, PR gatekeeper workflows, ban list
└── api-*.js                  # API adapters and proxies (api-proxy-enhanced.js is the main one)
```

**Páginas principales alineadas al framework**:
- `index.html` — Landing con hero cósmico 3D + tokenomics donut + personas cards
- `whitepaper.html` — Whitepaper v2.0 con 10 pools + 6 fuentes sustainability
- `ltd-token-economics.html` — Tokenomics interactiva con datos live del chain
- `governance.html` — Hub de gobernanza on-chain con Keplr wallet
- `mia.html` — MIA AI (7ma capa del ecosistema)
- `chain/index.html` — Chain landing con stats live

---

## 🤝 Cómo contribuir

La Tanda tiene un **sistema de bounties de 3 tiers** en GitHub Issues:

| Tier | Quién puede | Reward |
|---|---|---|
| **Tier 0** | Cualquiera | 10-50 LTD |
| **Tier 1** | 1+ merge previo | 50-150 LTD |
| **Tier 2** | 2+ merges previos | 150-500 LTD |

- Cada bounty requiere responder una pregunta de verificación del código (requiere leer la fuente real)
- PR Gatekeeper automático rechaza: PRs sin asignación, cuentas <30 días, usuarios en ban list
- Labels: `tier-0`, `tier-1`, `tier-2`

**Antes de abrir PR**:
1. Lee `CONTRIBUTING.md` (si existe) + `.github/ban-list.txt`
2. Responde la pregunta de verificación del bounty
3. Firma commits con tu email verificado en GitHub
4. Un PR = un bounty

---

## 📚 Recursos

### Documentación pública
- 🌐 Website: [latanda.online](https://latanda.online)
- 📜 Whitepaper v2.0: [latanda.online/whitepaper.html](https://latanda.online/whitepaper.html)
- 💰 Tokenomics: [latanda.online/ltd-token-economics.html](https://latanda.online/ltd-token-economics.html)
- 🏛️ Governance: [latanda.online/governance.html](https://latanda.online/governance.html)
- 💻 Dev Portal: [latanda.online/dev-dashboard.html](https://latanda.online/dev-dashboard.html)
- 📖 API Docs: [latanda.online/docs](https://latanda.online/docs)
- 🔗 Chain: [latanda.online/chain](https://latanda.online/chain/)

### Comunidad
- 💬 Discord: [discord.gg/Ve9M2ZSYC2](https://discord.gg/Ve9M2ZSYC2)
- 📢 Telegram: [t.me/latandahn](https://t.me/latandahn)
- 🐦 Twitter: [@TandaWeb3](https://twitter.com/TandaWeb3)
- 📰 Cosmos Forum: [Thread #16709](https://forum.cosmos.network/t/la-tanda-chain-incentivized-testnet-live-validators-node-operators-welcome-cosmos-sdk-v0-53-6/16709)
- 🟣 Reddit (own sub): [r/LaTandaChain](https://reddit.com/r/LaTandaChain)

---

## 📜 Licencia

MIT License — see [LICENSE](./LICENSE)

Código abierto, uso libre con atribución. Las marcas "La Tanda" y "La Tanda Chain" son propiedad de Ray-Banks LLC.

---

## ⚖️ Legal

La Tanda es operada por **Ray-Banks LLC**. Más información en [raybanks.org](https://raybanks.org).

Este repositorio es un mirror público del frontend. El código está liberado para transparencia y contribuciones comunitarias. No constituye oferta de valores ni asesoramiento financiero.

---

## 🚫 Reglas importantes

- **NUNCA** commitees `.env` o credenciales (ver `.env.example`)
- **NUNCA** uses `rsync --delete` con este repo
- **NUNCA** modifiques `api-proxy-enhanced.js` sin coordinar con el equipo
- Ban list pública: `.github/ban-list.txt` (no aceptamos PRs de cuentas listadas)

---

<p align="center">
<strong>Construyendo el Web3 de Latinoamérica, un tanda a la vez.</strong><br>
🇭🇳 Honduras → 🌎 LatAm → 🌍 Global
</p>
