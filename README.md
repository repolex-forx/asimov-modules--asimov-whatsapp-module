# Repolex Knowledge Graph of asimov-modules/asimov-whatsapp-module

RDF knowledge graph data for [asimov-modules/asimov-whatsapp-module](https://github.com/asimov-modules/asimov-whatsapp-module), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download asimov-modules/asimov-whatsapp-module
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 775675ed8b9ac96f51844d2a32178014c255db47
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 775675ed8b9ac96f51844d2a32178014c255db47.nq.gz
│   └── repolex
│       └── 775675ed8b9ac96f51844d2a32178014c255db47
│           └── chunk-001.nq.gz
├── blob
│   ├── 10b359dd05935c73efb064470f9ecda90f6d28aa.nq.gz
│   ├── 2b0c788e2596d934456a7ce78cc4e7f3fe40e217.nq.gz
│   ├── 3f7a460159a40edf9302bd9d3f2c8a6cdbd7c121.nq.gz
│   ├── 5ce44ba9d63ada47d0c562c8f2f33dc87c55a737.nq.gz
│   ├── 5d7dce87a40bfd4d48e4d958c9c1d641dfaa22eb.nq.gz
│   ├── 6995075d2aa0fcf85b0c4434341ab53c9d343ae0.nq.gz
│   ├── 75e3b65f99b29f48ab230e3eab3de8d0b7a9229f.nq.gz
│   ├── 779b1556bdfd351df91a1ac2b5965423e0aeb0a3.nq.gz
│   ├── 8acdd82b765e8e0b8cd8787f7f18c7fe2ec52493.nq.gz
│   ├── 91825a15bd47be191d72a58f40809bb4f36c2bb1.nq.gz
│   ├── 9fe50de16e59d550235aa6d7d15ee12ddf054414.nq.gz
│   ├── a0b02ef97f672cc65e2362cc26102e6cd4ea1fdb.nq.gz
│   ├── a3fead7f33c09a3a92cc9e40a1fdae99655dd610.nq.gz
│   ├── b79496c555f0aad6c3430d107cbd210d5a213071.nq.gz
│   ├── bd258c057ff14a4e87c0d7df4f5d5c91a1bdc5cf.nq.gz
│   ├── be61068482c9eef58d992fffba11d067e4e916f8.nq.gz
│   ├── cf42f6893594e2f8be2b722de51123d65e4d61c4.nq.gz
│   ├── d47d445d7010eabcd057b4b10440e6e47304237e.nq.gz
│   ├── d896fada89f907fdd862871be886c73003b340dc.nq.gz
│   ├── e3e57a8ce4ccbf74759a6df8fa4a3980ff1c9209.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── efb98088164f5786b17e83ed384971fc3c74f93c.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 775675ed8b9ac96f51844d2a32178014c255db47.nq.gz
├── filetree
│   └── 775675ed8b9ac96f51844d2a32178014c255db47.nq.gz
├── issue
│   └── issue.nq.gz
└── tag
    └── tag.nq.gz

14 directories, 31 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[asimov-modules/asimov-whatsapp-module](https://github.com/asimov-modules/asimov-whatsapp-module)

---
*Parsed on 2026-09-28 by [repolex](https://repolex.ai)*
