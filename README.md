# Eviory

**Open-source workspaces for the modern web.**

Eviory is a collection of browser-based, local-first workspaces designed to help people think, create, organize, and execute without being locked into a traditional SaaS workflow.

The ecosystem is built around a simple idea:

> **Your workspace should belong to you.**

Eviory prioritizes local-first data, open standards, portable content, and a polished desktop-like experience that runs directly in the browser.

---

## The Eviory Ecosystem

Eviory is not a single application. It is an ecosystem of focused workspaces that can work independently or evolve together.

### Eviory Docs

A visual document workspace inspired by the flexibility of modern block editors and collaborative documents.

Designed for:

* Documents
* Notes
* Knowledge bases
* Structured content
* AI-generated document architectures
* Rich blocks and layouts

Eviory Docs is designed around structured, portable data rather than locking your content inside a proprietary database.

---

### Eviory Board

A visual workspace for thinking and organizing ideas spatially.

Designed for:

* Brainstorming
* Mind maps
* Project planning
* Visual research
* Strategy
* Diagrams
* Canvas-based workflows

The goal is to provide a capable visual workspace without requiring users to connect dozens of external services just to get work done.

---

### Eviory OS

The broader Eviory workspace ecosystem.

Eviory OS brings together tools for planning, content, business operations, and execution into a unified browser-based environment.

Instead of building another collection of disconnected SaaS tools, Eviory aims to provide a workspace where different capabilities can operate together while remaining useful on their own.

---

## Core Principles

### Local-first

Your data should work even when the network does not.

Eviory is designed around local storage and browser-native technologies wherever practical, with cloud synchronization treated as an additional capability rather than the foundation of the application.

### Open source

The core software should remain inspectable, understandable, and extensible.

Eviory is built in the open so developers can study the architecture, contribute improvements, build integrations, and create their own versions.

### Portable data

Your work should not be trapped inside a proprietary application.

Eviory aims to use structured data formats and architectures that make it possible to move, export, synchronize, and process your data independently of the interface.

### AI-native

AI should be able to work with your workspace directly.

Rather than treating AI as a separate chatbot, Eviory is designed so AI can eventually create and manipulate structured workspace data.

For example:

```text
User
  ↓
AI / MCP
  ↓
Structured JSON
  ↓
Eviory Workspace
  ↓
Document / Board / Workflow
```

This makes it possible for an AI agent to generate an entire document structure, workspace, or visual system that the user can immediately open and edit.

### Browser-native

Eviory is designed to run directly in the browser.

No traditional desktop installation is required, while modern browser capabilities can provide an experience much closer to a native application.

---

## Why Eviory?

Modern productivity software often creates the same problem it tries to solve:

* One application for documents
* Another for whiteboards
* Another for project management
* Another for AI
* Another for automation
* Another for file storage
* Another for publishing

Eviory explores a different approach.

Build focused tools that feel independent, but share a common philosophy and technical foundation.

```text
                    ┌───────────────┐
                    │    EVIORY     │
                    └───────┬───────┘
                            │
             ┌──────────────┼──────────────┐
             │              │              │
        ┌────▼────┐    ┌────▼────┐    ┌────▼────┐
        │   Docs  │    │  Board  │    │   OS    │
        └────┬────┘    └────┬────┘    └────┬────┘
             │              │              │
             └──────────────┼──────────────┘
                            │
                     Local-first Core
                            │
                   ┌────────┴────────┐
                   │                 │
                  AI                Sync
                 /MCP              Layer
```

---

## AI + MCP

One of the long-term goals of Eviory is making workspaces understandable and controllable by AI agents.

Instead of asking an AI to merely describe a document, an agent could generate the underlying structure itself.

For example:

```json
{
  "type": "document",
  "title": "Product Launch Plan",
  "blocks": [
    {
      "type": "heading",
      "content": "Launch Strategy"
    },
    {
      "type": "paragraph",
      "content": "Define the core positioning..."
    },
    {
      "type": "database",
      "name": "Launch Tasks"
    }
  ]
}
```

The workspace can then interpret that structure and render it as an editable document.

This approach opens the door to:

* AI-generated workspaces
* AI-generated documents
* AI-generated boards
* Agent-driven workflows
* MCP integrations
* Structured workspace automation
* User-approved AI actions

The objective is simple:

**AI creates the structure. You remain in control of the result.**

---

## Architecture

Eviory is being built around a local-first architecture.

A simplified model looks like this:

```text
                    Browser
                       │
              ┌────────┴────────┐
              │                  │
          Application         IndexedDB
              │                  │
              └────────┬─────────┘
                       │
                 Local Source
                    of Truth
                       │
                 Optional Sync
                       │
                ┌──────┴──────┐
                │             │
              Cloud          Export
              Storage        / Import
```

The architecture is intentionally designed to minimize unnecessary infrastructure.

Cloud services can provide:

* Synchronization
* Authentication
* Backups
* Shared workspaces
* Remote assets
* Collaboration

But the core workspace should remain useful without depending on a permanent cloud connection.

---

## Technology

Eviory is built with modern web technologies, with a strong focus on browser-native capabilities.

The stack may evolve as the projects develop, but the architecture currently revolves around technologies such as:

* **Astro**
* **React**
* **TypeScript**
* **IndexedDB**
* **Web APIs**
* **JSON-based data structures**
* **MCP / AI integrations**
* **Serverless infrastructure**

The project intentionally avoids unnecessary infrastructure when a browser-native or serverless solution can accomplish the same thing.

---

## Projects

The Eviory ecosystem is evolving.

| Project          | Purpose                                              |
| ---------------- | ---------------------------------------------------- |
| **Eviory Docs**  | Structured documents and knowledge work              |
| **Eviory Board** | Visual thinking and spatial work                     |
| **Eviory OS**    | Broader workspace and business operating environment |
| **EvioryKit**    | Commercial digital-product ecosystem                 |

Some projects may live in separate repositories as they mature.

---

## Development

Clone the repository:

```bash
git clone https://github.com/aldhydheriz/eviory.git
cd eviory
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Build for production:

```bash
npm run build
```

Check the project:

```bash
npm run check
```

> Commands may change as the project evolves. Check the repository configuration for the current development workflow.

---

## Contributing

Contributions are welcome.

You can contribute through:

* Bug fixes
* Performance improvements
* UI improvements
* Accessibility improvements
* Documentation
* New workspace capabilities
* AI / MCP integrations
* Browser-native experiments
* Architecture discussions

Before making a large change, open an issue or discussion so the direction can be aligned with the project's architecture.

---

## Philosophy

Eviory is built around a few simple questions:

**What if your workspace actually belonged to you?**

**What if local-first software could feel as polished as SaaS?**

**What if AI could understand the structure of your work instead of only generating text around it?**

**What if powerful workspaces could remain open, portable, and inexpensive to operate?**

Eviory is an exploration of those ideas.

---

## Status

Eviory is actively evolving.

Expect architectural changes, experiments, unfinished features, and breaking changes while the ecosystem takes shape.

The goal is not to recreate every existing productivity application.

The goal is to explore what an **open, local-first, AI-**
