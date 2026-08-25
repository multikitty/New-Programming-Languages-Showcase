# SEMAPRAX (programming language)

### Description

[SEMAPRAX](https://wavect.io/semaprax/) is an experimental agent-native systems programming language and compiler from Wavect GmbH. Its premise is that human-readable `.spx` source remains the canonical Git representation while a deterministic, versioned semantic graph provides a structured interface for coding agents.

The Rust implementation gives public declarations persistent identities and makes contracts, effects, capabilities, ownership, and call relationships explicit. Its bounded agent workflows include semantic context, impact analysis, review, and replayable evidence-gated patches. The compiler currently has Native C11/Clang and WebAssembly Core output paths.

SEMAPRAX v0.2 is pre-alpha research software. Its language, graph schemas, diagnostics, and ABIs can change, and the maintainers explicitly advise against production or security-critical use.

### Developed by

SEMAPRAX is developed by [Wavect GmbH](https://wavect.io/). Coding agents are used extensively as development assistants; Wavect retains human responsibility and uses executable quality gates as evidence for implemented slices.

### Brief history

The public repository was launched in August 2026. The project explores a compiler and language architecture in which semantic identity survives source-level changes such as renaming, and agent-proposed changes can be checked against deterministic semantic evidence before they receive commit authority.

### Research goals

- **Stable semantic identity**: Public declarations can carry persistent `@id` identities rather than being identified only by mutable names and source locations.
- **Agent-readable program meaning**: The compiler emits deterministic semantic graphs and bounded context, impact, and review reports.
- **Replayable changes**: Evidence-gated semantic patches can be independently replayed before an authorized application route publishes them.
- **Explicit authority**: Capabilities, effects, ownership, and resource lifecycles are represented explicitly instead of silently granting ambient authority.
- **Backend consistency**: Implemented language behavior is intended to remain equivalent across the native C11/Clang and WebAssembly Core backends.

These are research directions, not claims that the project already provides a complete general-purpose language, autonomous software engineer, or production toolchain.

### Current use cases

At its present maturity, SEMAPRAX is most appropriate for:

- studying stable identities and semantic graphs in compiler design;
- experimenting with deterministic, bounded context for coding agents;
- evaluating evidence-carrying semantic change workflows;
- exploring explicit ownership, capabilities, effects, contracts, and cleanup semantics; and
- comparing native and WebAssembly projections of a checked source language.

Its bounded injected-host Agent Runtime can emit canonical Trace and Evidence data and replay it independently. It does not include a built-in model, network transport, durable memory, signing keys, or production authority.

### Project status and outlook

The project's completion matrix deliberately marks implemented areas as partial until their stated evidence gates pass and records missing scope separately. Current work covers a useful core language and bounded agent-facing workflows, while broader language completeness, packaging, interoperability, application SDKs, and production readiness remain open.

### How to learn and evaluate it

- **Project overview**: Read the [SEMAPRAX homepage](https://wavect.io/semaprax/) for the motivation, architecture summary, and current status.
- **Source and documentation**: Review the [Apache-2.0 repository](https://github.com/wavect/semaprax), especially its RFC, architecture document, completion matrix, and quality gates.
- **Examples**: The repository includes canonical `.spx` programs exercised by the project's automated gates.
- **Try the projections**: The CLI can format and check source, emit the semantic graph, and generate bounded context and impact reports for supported programs.

Because the project is pre-alpha, readers should verify every capability against the repository's current completion matrix rather than assuming roadmap items are already implemented.
