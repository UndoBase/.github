<p align="center">
  <img src="logo.png" alt="UndoBase"/>
</p>

<h3 align="center">UndoBase</h3>

<p align="center">The safety layer your agent infrastructure is missing.</p>

<p align="center">
  AI agents take real-world actions. Most frameworks have no way to reverse them.<br/>
  UndoBase builds the infrastructure that makes every agent action accountable.
</p>

<!-- ── PRODUCTS ── -->

## Products

### UndoLog
The AI agent safe execution runtime. Every tool call is classified as `safe`, `compensable`, or `irreversible`. Compensable actions register a compensation function before executing. Irreversible actions require explicit human approval. On failure, the undo stack walks back in LIFO order with exactly-once guarantees.

Built on a Rust core (`undolog-engine`, `undolog-store`, `undolog-types`, `undolog-saga`), a Go MCP proxy (`undolog-proxy`), and a Python SDK (`undolog-sdk`).

**Grounded in ACRFence (2026)** -- the first open-source implementation of its replay-or-fork semantics.

### Coming next
`UndoScan` -- RAG pipeline quality and retrieval evaluation.  
`UndoRoute` -- Intelligent multi-model orchestration and cost routing.  
`UndoWatch` -- LLM observability and policy enforcement.

<!-- ── PRINCIPLES ── -->

## Principles

- **Determinism over hope.** Safety guarantees are enforced by the system, not by prompting the model correctly.
- **Built in the open.** Every decision is documented. Every trade-off is an ADR. Apache 2.0, free forever.
- **Infrastructure, not tooling.** UndoBase products sit at the protocol layer and work with any agent framework.

<!-- ── GET STARTED ── -->

## Get started

- [UndoLog documentation](https://github.com/UndoBase/UndoLog)
- [Python SDK on PyPI](https://pypi.org/project/undolog-sdk)
- [Architecture decisions](https://github.com/UndoBase/UndoLog/tree/main/docs/adr)
- [Contributing guide](https://github.com/UndoBase/UndoLog/blob/main/docs/contributing/CONTRIBUTING.md)

<!-- ── FOOTER ── -->

---

Apache 2.0 &nbsp;|&nbsp; [github.com/UndoBase](https://github.com/UndoBase)
