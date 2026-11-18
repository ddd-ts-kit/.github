<div align="center">

<img src="https://raw.githubusercontent.com/ddd-ts-kit/ddd-ts-kit/main/docs/assets/logo.svg" alt="" width="96" height="96">

# ddd-ts-kit

Domain-Driven Design, Clean Architecture and Clean Code for TypeScript and Node.js backends,
held by tools rather than by good intentions.

**[Documentation](https://ddd-ts-kit.github.io/ddd-ts-kit/)** ·
[Repository](https://github.com/ddd-ts-kit/ddd-ts-kit) ·
[npm](https://www.npmjs.com/package/ddd-ts-kit) ·
[Discussions](https://github.com/ddd-ts-kit/ddd-ts-kit/discussions) ·
[Changelog](https://github.com/ddd-ts-kit/ddd-ts-kit/blob/main/CHANGELOG.md)

</div>

## What it is

An architecture written as rules with ids, checked at every file write, before every merge and on
every push, and the tools that make following them the short path:

- **A CLI** that bootstraps a project, generates its building blocks with their specs and checks
  the architecture: `npx ddd-ts-kit init`.
- **Runtime packages** under `@ddd-ts-kit/*`: a kernel without dependencies, integration events
  with a transactional outbox, access control, audit trail, HTTP, validation, and adapters for
  four ORMs, four brokers and the common HTTP frameworks.
- **An ESLint plugin** that carries the code rules into the editor.
- **A plugin for Claude Code, Codex and GitHub Copilot**: skills that conduct a project from a
  statement of needs to working bounded contexts, and a hook that checks each file the agent
  writes.

Everything lives in one repository, released under one version:
[ddd-ts-kit/ddd-ts-kit](https://github.com/ddd-ts-kit/ddd-ts-kit).

## How it is built

- Every pull request passes the whole pipeline again in a merge queue before it reaches `main`.
- Every release is published from CI by npm trusted publishing, with provenance, a signed
  attestation and a bill of materials for each package
  ([verifying a release](https://github.com/ddd-ts-kit/ddd-ts-kit/blob/main/SECURITY.md)).
- The documentation is written in English and in French.

## Taking part

Questions and ideas go to [Discussions](https://github.com/ddd-ts-kit/ddd-ts-kit/discussions),
bugs and proposals to [issues](https://github.com/ddd-ts-kit/ddd-ts-kit/issues/new/choose), and a
vulnerability to a private report, never a public issue
([security policy](https://github.com/ddd-ts-kit/ddd-ts-kit/blob/main/SECURITY.md)).
[CONTRIBUTING.md](https://github.com/ddd-ts-kit/ddd-ts-kit/blob/main/CONTRIBUTING.md) says how a
change reaches `main`. MIT licensed.
