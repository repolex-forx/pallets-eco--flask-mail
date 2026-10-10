# Repolex Knowledge Graph of pallets-eco/flask-mail

RDF knowledge graph data for [pallets-eco/flask-mail](https://github.com/pallets-eco/flask-mail), parsed by [repolex](https://repolex.ai).

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
rlex download pallets-eco/flask-mail
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 98203358d836788ab96e6125489895d71e9d99a3
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 98203358d836788ab96e6125489895d71e9d99a3
│           └── chunk-001.nq.gz
├── blob
│   ├── 014d8538651c5f739e525dc9570bea9994f056bd.nq.gz
│   ├── 10e0933f0690adbf434ef75d652e1ba808e46fd0.nq.gz
│   ├── 1202c49e07a39a07d004ec1574747ea457d6aba7.nq.gz
│   ├── 2ff985a67af35fdfd1076354b771c425867cdab4.nq.gz
│   ├── 35e705c5abf566a1ae72137eeb3fab13e89629b3.nq.gz
│   ├── 40ceb3e7476ea1b564291141df9b1b22e1fe8332.nq.gz
│   ├── 501a5b720b0641fe81da393f53575c0c98746486.nq.gz
│   ├── 59495a954c25db9cf03cf56a8b5d41924bcb1b2c.nq.gz
│   ├── 5f522c22204b689033f69e581c007bc1e1d73774.nq.gz
│   ├── 61ab092a18e6ede80fe9861eee93066e90db4cd8.nq.gz
│   ├── 62c1b887d73cc6325731f0c9c97927df23a42d1d.nq.gz
│   ├── 62d10c3d74e57d41cae2a5899d8ae957c6e80d80.nq.gz
│   ├── 65134d540bd92f57b88e7194ce347f24eae89af5.nq.gz
│   ├── 6b79eaa1d6e754caa0986f1f206799c325b95b4c.nq.gz
│   ├── 73cbb2d8514a061fbca75cb689818290eb081f8c.nq.gz
│   ├── 78e76e8f6616ba373d8d3cc06d5856c5c45856de.nq.gz
│   ├── 8460d367ccfbb9911768e78fa52f5bdfecbab880.nq.gz
│   ├── 87172e9d061f8f052dbdf30d14f0f4cd4c9bb4eb.nq.gz
│   ├── 9c2d0ef398039ab06a9a33cbe66f4801b25cff55.nq.gz
│   ├── a5f1b46a997610f8f09e4e720001662bb1c37315.nq.gz
│   ├── b3c637829e29229619b0e943270571197d61cb88.nq.gz
│   ├── b8bf57179fbfc302c3bb24248eb84b558e53c663.nq.gz
│   ├── bb1a7559e1785e2d3a7aa574e4daa7445c0ec922.nq.gz
│   ├── bee8495cc77b171f0f27a4ac318642b8a6d9f3dd.nq.gz
│   ├── c3bb2c75205cb3d0fd24f4cea9ae66e7dbc79667.nq.gz
│   ├── c81164e47793ec0fd5a4ec7daf71128324d8b455.nq.gz
│   ├── c8b512175f393313874024d59331c789663f1729.nq.gz
│   ├── cd3be72046ee75db7914fc8653dc3969f94da3d7.nq.gz
│   ├── d41960fc228ca413b1ccb4a3e2a601cd9e89e930.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── ecdb7d59ea41168ee6d1b0d3520050eb42b8125e.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 98203358d836788ab96e6125489895d71e9d99a3.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 39 files
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

[pallets-eco/flask-mail](https://github.com/pallets-eco/flask-mail)

---
*Parsed on 2026-10-10 by [repolex](https://repolex.ai)*
