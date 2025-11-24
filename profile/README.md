<div align="center">

<pre>
██╗     ██╗   ██╗███╗   ███╗ ██████╗ ███████╗
██║     ██║   ██║████╗ ████║██╔═══██╗██╔════╝
██║     ██║   ██║██╔████╔██║██║   ██║███████╗
██║     ██║   ██║██║╚██╔╝██║██║   ██║╚════██║
███████╗╚██████╔╝██║ ╚═╝ ██║╚██████╔╝███████║
╚══════╝ ╚═════╝ ╚═╝     ╚═╝ ╚═════╝ ╚══════╝
</pre>

### Write Once. Deploy Everywhere.

[![Website](https://img.shields.io/badge/🌐_lumos--lang.org-9945FF?style=for-the-badge)](https://lumos-lang.org)
[![Crates.io](https://img.shields.io/crates/v/lumos-core?style=for-the-badge&logo=rust&label=crates.io)](https://crates.io/crates/lumos-core)
[![npm](https://img.shields.io/npm/v/@getlumos/cli?style=for-the-badge&logo=npm&label=npm)](https://www.npmjs.com/package/@getlumos/cli)
[![GitHub Action](https://img.shields.io/badge/Marketplace-LUMOS%20Generate-purple.svg?style=for-the-badge&logo=github)](https://github.com/marketplace/actions/lumos-generate)

*Type-safe schema language for Solana development • TypeScript ↔ Rust synchronization • Zero type drift*

</div>

---

## 🎯 What is LUMOS?

**LUMOS** is a powerful schema language that eliminates the pain of maintaining duplicate type definitions across TypeScript and Rust in Solana applications.

Write your data structures **once** in `.lumos` syntax → Generate production-ready TypeScript + Rust code with guaranteed Borsh serialization compatibility.

```rust
// schema.lumos
#[solana]
#[account]
struct PlayerAccount {
    wallet: PublicKey,
    level: u16,
    experience: u64,
}
```

**Generates:**
- ✅ Rust structs with Anchor integration
- ✅ TypeScript interfaces with Borsh schemas
- ✅ Perfect serialization compatibility
- ✅ Zero manual synchronization needed

---

## 🌟 Ecosystem

The LUMOS ecosystem provides everything you need for type-safe Solana development.

<table>
<tr>
<td width="50%">

### 🦀 [lumos](https://github.com/getlumos/lumos)
**Core Compiler & CLI**

The heart of LUMOS - Rust-based compiler and command-line tool for schema generation and validation.

- ✅ **Published:** crates.io
- 🛠️ **Stack:** Rust, syn, Borsh
- 📦 **Packages:** lumos-core, lumos-cli, lumos-lsp
- ✨ **Features:** Context-aware generation, LSP server

[📖 Documentation](https://lumos-lang.org) • [🚀 Get Started](https://crates.io/crates/lumos-cli)

</td>
<td width="50%">

### 📦 [npm Package](https://github.com/getlumos/lumos/tree/main/packages/npm)
**WASM CLI for JavaScript/TypeScript**

Use LUMOS in JavaScript/TypeScript projects without installing Rust - WASM-powered CLI for seamless integration.

- ✅ **Published:** npm (@getlumos/cli)
- 🛠️ **Stack:** Rust + WASM, Node.js
- 🎯 **Use Case:** JS/TS devs, no Rust required
- ⚡ **Speed:** Native performance via WASM

[📦 View on npm](https://www.npmjs.com/package/@getlumos/cli)

</td>
</tr>
<tr>
<td width="50%">

### 💻 [vscode-lumos](https://github.com/getlumos/vscode-lumos)
**Visual Studio Code Extension**

Full IDE support for `.lumos` files with syntax highlighting, IntelliSense, diagnostics, and quick fixes.

- ✅ **Published:** VS Marketplace (v0.5.0)
- ⭐ **Features:** LSP integration, snippets, format-on-save
- 🛠️ **Stack:** TypeScript, VSCode API
- 🎨 **Grammar:** 26 syntax rules

[🔌 Install Extension](https://marketplace.visualstudio.com/items?itemName=getlumos.vscode-lumos)

</td>
<td width="50%">

### 🧠 [intellij-lumos](https://github.com/getlumos/intellij-lumos)
**IntelliJ IDEA / Rust Rover Plugin**

Native LUMOS support for JetBrains IDEs with LSP integration and smart features.

- 🚧 **Status:** v0.1.0 development
- 🛠️ **Stack:** Kotlin, IntelliJ Platform SDK
- 🎯 **Target:** IntelliJ IDEA, Rust Rover, CLion
- ⚡ **Features:** LSP client, syntax highlighting

[📦 View Repository](https://github.com/getlumos/intellij-lumos)

</td>
</tr>
<tr>
<td width="50%">

### 🌙 [nvim-lumos](https://github.com/getlumos/nvim-lumos)
**Neovim Plugin**

First-class Neovim support with Tree-sitter syntax highlighting and LSP integration.

- ✅ **Status:** v0.1.0 ready
- 🛠️ **Stack:** Lua, Tree-sitter, nvim-lspconfig
- 🎯 **Features:** Auto-detection, keybindings, LSP
- ⚡ **Grammar:** tree-sitter-lumos

[📦 View Repository](https://github.com/getlumos/nvim-lumos)

</td>
<td width="50%">

### 🦄 [lumos-mode](https://github.com/getlumos/lumos-mode)
**Emacs Major Mode**

Complete Emacs integration with syntax highlighting, indentation, and LSP support.

- ✅ **Status:** v0.1.0 ready
- 🛠️ **Stack:** Emacs Lisp, lsp-mode
- ✨ **Features:** Smart indent, LSP integration
- ✅ **Tests:** 14 tests passing

[📦 View Repository](https://github.com/getlumos/lumos-mode)

</td>
</tr>
<tr>
<td width="50%">

### 🎨 [sublime-lumos](https://github.com/getlumos/sublime-lumos)
**Sublime Text Package**

Professional LUMOS support for Sublime Text with syntax definition and LSP client.

- ✅ **Status:** v0.1.0 (Package Control PR pending)
- 🛠️ **Stack:** YAML syntax, LSP integration
- ✨ **Features:** 6 snippets, auto-indent, LSP
- 📦 **PR:** Package Control #9251

[📦 View Repository](https://github.com/getlumos/sublime-lumos)

</td>
<td width="50%">

### 🌳 [tree-sitter-lumos](https://github.com/getlumos/tree-sitter-lumos)
**Tree-sitter Grammar**

Official Tree-sitter grammar for LUMOS syntax - powers syntax highlighting across multiple editors.

- ✅ **Status:** v0.1.0 ready
- 🛠️ **Stack:** JavaScript, Tree-sitter
- ✅ **Tests:** 6/6 passing
- 🎯 **Coverage:** Structs, enums, all types

[📦 View Repository](https://github.com/getlumos/tree-sitter-lumos)

</td>
</tr>
<tr>
<td width="50%">

### 🎓 [awesome-lumos](https://github.com/getlumos/awesome-lumos)
**Production-Ready Examples**

5 complete Solana applications showcasing LUMOS in real-world scenarios.

- 📦 **Examples:** NFT Marketplace, DeFi Staking, DAO Governance, Gaming, Token Vesting
- 🛠️ **Stack:** Anchor, TypeScript, Solana web3.js
- 📊 **Scale:** 53 types, 42 instructions, 4000+ LOC
- ✅ **Status:** All examples complete

[📖 Explore Examples](https://github.com/getlumos/awesome-lumos)

</td>
<td width="50%">

### 📚 [docs-lumos](https://github.com/getlumos/docs-lumos)
**Official Documentation**

Comprehensive guides, references, and examples - deployed to lumos-lang.org.

- 🌐 **Live:** lumos-lang.org
- 🛠️ **Stack:** VitePress, Markdown, Vue
- 🚀 **Deploy:** Cloudflare Pages (auto)
- 📖 **Content:** Guide, Reference, Examples, API

[🌐 Visit Docs](https://lumos-lang.org)

</td>
</tr>
<tr>
<td width="50%">

### ⚙️ [lumos-action](https://github.com/getlumos/lumos-action)
**GitHub Action**

Automated schema validation and code generation for CI/CD pipelines.

- ✅ **Published:** GitHub Marketplace (v1.0.0)
- 🛠️ **Type:** Composite Action (Bash)
- ✨ **Features:** Auto-install, validate, generate, drift detection
- 🎯 **Use Case:** CI/CD automation

[🔌 View on Marketplace](https://github.com/marketplace/actions/lumos-generate)

</td>
<td width="50%">

</td>
</tr>
</table>

---

## 🚀 Quick Start

### Installation

**Option 1: Rust CLI (Recommended)**
```bash
cargo install lumos-cli
lumos --version
```

**Option 2: npm Package (JavaScript/TypeScript projects)**
```bash
npm install --save-dev @getlumos/cli
npx lumos --version
```

**Option 3: GitHub Action (CI/CD)**
```yaml
- uses: getlumos/lumos-action@v1
  with:
    schema: 'schemas/**/*.lumos'
```

### Your First Schema

**1. Create a schema file** (`schema.lumos`):
```rust
#[solana]
#[account]
struct Counter {
    authority: PublicKey,
    count: u64,
}
```

**2. Generate code:**
```bash
lumos generate schema.lumos
```

**3. Use generated code:**
```typescript
// TypeScript (generated.ts)
import { Counter } from './generated';

const counter = new Counter({
  authority: publicKey,
  count: 0n,
});
```

```rust
// Rust (generated.rs)
use crate::generated::Counter;

#[derive(Accounts)]
pub struct Initialize<'info> {
    #[account(init, payer = authority, space = 8 + Counter::LEN)]
    pub counter: Account<'info, Counter>,
    // ...
}
```

**Perfect synchronization guaranteed!** ✨

---

## 🛠️ Editor Support

LUMOS works in **your favorite editor**:

| Editor | Package | Status | LSP | Syntax | Snippets |
|--------|---------|--------|-----|--------|----------|
| **VS Code** | vscode-lumos | ✅ v0.5.0 | ✅ | ✅ | ✅ 13 snippets |
| **IntelliJ IDEA** | intellij-lumos | 🚧 v0.1.0 | ✅ | ✅ | - |
| **Neovim** | nvim-lumos | ✅ v0.1.0 | ✅ | ✅ Tree-sitter | - |
| **Emacs** | lumos-mode | ✅ v0.1.0 | ✅ | ✅ | - |
| **Sublime Text** | sublime-lumos | ✅ v0.1.0 | ✅ | ✅ | ✅ 6 snippets |

**All editors connect to the same LSP server** (`lumos-lsp`) for consistent features!

---

## 📊 Stats

<div align="center">

| Metric | Count | Details |
|--------|-------|---------|
| 🎯 **Repositories** | 10 | Core, 5 editor plugins, examples, docs, npm, action |
| 📦 **Published Packages** | 6 | crates.io (3), npm (1), VS Marketplace (1), GitHub Marketplace (1) |
| ✅ **Tests Passing** | 142 | Comprehensive test coverage across all packages |
| 📖 **Example Projects** | 5 | NFT, DeFi, DAO, Gaming, Vesting |
| 🌐 **Editor Integrations** | 5 | VSCode, IntelliJ, Neovim, Emacs, Sublime |
| 🚀 **Lines of Code** | 10,000+ | Including examples and generated code |

</div>

---

## 💡 Why LUMOS?

### The Problem

Building Solana dApps requires maintaining **duplicate type definitions**:
- ❌ Rust structs for on-chain programs (Anchor)
- ❌ TypeScript interfaces for client-side code
- ❌ Manual Borsh serialization schemas
- ❌ Constant synchronization overhead
- ❌ Type drift bugs in production

### The Solution

**Write once in LUMOS** → Generate everything automatically:
- ✅ **Single source of truth** - `.lumos` schema files
- ✅ **Guaranteed compatibility** - Borsh serialization verified
- ✅ **Context-aware generation** - Anchor vs pure Borsh detection
- ✅ **Zero manual work** - Automated with CLI or GitHub Actions
- ✅ **Type safety** - Catch errors at compile time, not runtime

### Real-World Impact

```
Before LUMOS:
├── 📝 Write Rust struct (5 min)
├── 📝 Write TypeScript interface (3 min)
├── 📝 Write Borsh schema (5 min)
├── 🐛 Debug type mismatch (30 min)
└── ⏱️ Total: 43 minutes per type

After LUMOS:
├── 📝 Write .lumos schema (2 min)
├── ⚡ lumos generate (5 sec)
└── ⏱️ Total: 2 minutes per type

💰 95% time savings • 🐛 Zero type drift bugs
```

---

## 🌍 Community

### Learn & Contribute

- 📖 **[Documentation](https://lumos-lang.org)** - Comprehensive guides and references
- 🎓 **[Examples](https://github.com/getlumos/awesome-lumos)** - Production-ready templates
- 🐙 **[GitHub Discussions](https://github.com/getlumos/lumos/discussions)** - Ask questions, share ideas
- 🐛 **[Issue Tracker](https://github.com/getlumos/lumos/issues)** - Report bugs, request features

### How to Contribute

1. ⭐ **Star** repositories you find useful
2. 🐛 **Report issues** to help us improve
3. 💡 **Suggest features** in GitHub Discussions
4. 🔧 **Submit PRs** with improvements
5. 📖 **Share examples** of your LUMOS projects
6. 📣 **Spread the word** in Solana communities

---

## 🗺️ Roadmap

### ✅ Completed

- **Phase 1-3:** Core compiler, CLI, basic types
- **Phase 4:** Advanced types (Vec, Option, arrays)
- **Phase 5.1:** Schema evolution (versioning, migrations, deprecation)
- **Phase 5.2:** IDE integration (VSCode, IntelliJ, Neovim, Emacs, Sublime)
- **Phase 6.1:** Documentation website
- **Phase 6.2:** npm package, GitHub Action

### 🚧 In Progress

- **Cargo subcommand:** `cargo lumos` integration
- **Pre-commit hooks:** Automated validation

### 🔮 Future

- **Phase 7:** Advanced features (generics, traits, macros)
- **Phase 8:** Cross-chain support (beyond Solana)
- **Phase 9:** Visual schema designer (GUI)

[📋 Full Roadmap](https://github.com/getlumos/lumos/blob/main/docs/ROADMAP.md)

---

## 📬 Get Involved

### For Developers

- 🚀 **Try LUMOS** in your next Solana project
- 🎓 **Learn from examples** at awesome-lumos
- 🔧 **Integrate with CI/CD** using lumos-action
- 💬 **Share feedback** in GitHub Discussions

### For Contributors

- 📖 **Improve documentation** with real-world use cases
- 🎨 **Build editor plugins** for your favorite IDE
- 🐛 **Fix bugs** and improve error messages
- ✨ **Add features** from the roadmap

### For Organizations

- 💼 **Adopt LUMOS** for type-safe Solana development
- 🤝 **Sponsor development** via GitHub Sponsors
- 🏆 **Showcase projects** using LUMOS
- 📣 **Spread awareness** in blockchain communities

---

<div align="center">

### Production-Ready Type Safety for Solana

*Write once. Deploy everywhere. Zero type drift.*

---

**LUMOS** | Illuminate Your Solana Development | 2025

[![GitHub](https://img.shields.io/badge/GitHub-getlumos-181717?style=for-the-badge&logo=github)](https://github.com/getlumos)
[![Website](https://img.shields.io/badge/Website-lumos--lang.org-9945FF?style=for-the-badge&logo=google-chrome&logoColor=white)](https://lumos-lang.org)
[![Discord](https://img.shields.io/badge/Community-Join_Us-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://github.com/getlumos/lumos/discussions)

*Made with ❤️ for the Solana ecosystem*

</div>
