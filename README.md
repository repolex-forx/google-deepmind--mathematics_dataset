# Repolex Knowledge Graph of google-deepmind/mathematics_dataset

RDF knowledge graph data for [google-deepmind/mathematics_dataset](https://github.com/google-deepmind/mathematics_dataset), parsed by [repolex](https://repolex.ai).

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
rlex download google-deepmind/mathematics_dataset
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 427f45075f84b8b9774950196ad63867ca20ffb3
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 427f45075f84b8b9774950196ad63867ca20ffb3
│           └── chunk-001.nq.gz
├── blob
│   ├── 05f4a6d59820f19260eb046d99d8e465c5abdebc.nq.gz
│   ├── 0b024d9feaabaccab8116f16401a9c177116af48.nq.gz
│   ├── 137178d3d932f925f0c6df722576ad3bffb0ec5e.nq.gz
│   ├── 150dd3f3599ea68a56767f1c669585a765e5d914.nq.gz
│   ├── 1620bcb13bdc26034c9ab829b7842afe60f17683.nq.gz
│   ├── 1a4687b70da72cc10cde66a5d116d998a45541cb.nq.gz
│   ├── 26347a4369d7787244ca9bcf7a5960ea805fa39b.nq.gz
│   ├── 29e0c69bf58dc8c15ac5e70b71afe031a7311b2f.nq.gz
│   ├── 2b7c6a9b5965c2e0a0beb03cc7a2130058fa887e.nq.gz
│   ├── 2e86478d5812f384f3559098bfde9b16b69e83a0.nq.gz
│   ├── 2ef73fc0c59c9da8a023d954646243f11768ed29.nq.gz
│   ├── 3016d0523306bebdd9671a104be8c6da51a61170.nq.gz
│   ├── 3381619974657f5d6e480c2daba3da3e46865d08.nq.gz
│   ├── 403f5c7c8edb7fb6d13df315a9ad1d8ec4c53f49.nq.gz
│   ├── 409a7a9fa992ec7f47dcdd54282d89da4394429e.nq.gz
│   ├── 41bdf658a0e09775c83d6fdefc9dd73a5639f99b.nq.gz
│   ├── 44344698f2f1fa9c8e32893b8e00f5aee44542ef.nq.gz
│   ├── 4bc6ef994a9fc789fb9b0f7d5b663229f444f0d8.nq.gz
│   ├── 4ccc0d93b4203c95e9fc5f51208ac5ca1c4178ea.nq.gz
│   ├── 6d010c3c7a5f8232a426537e3218b03c1fbbce28.nq.gz
│   ├── 71d9eaa9c3357017d7ca2468d36a06b806380faf.nq.gz
│   ├── 7bab2c79da289f723b0a6d03e4269c5290789c97.nq.gz
│   ├── 7dbf779b8612356afa91bc7fbfafe3d964079082.nq.gz
│   ├── 828e5b83b00b5d35a93e817aa35f462ec619268d.nq.gz
│   ├── 92eb8288622c3fd9b6f9516619674e1b7db1c082.nq.gz
│   ├── b69a0c3d1420f27db6d755b63b470e97e599aa29.nq.gz
│   ├── c1cb681a1a2c47ef33ab3df4244a1ace83269e39.nq.gz
│   ├── c4732902404c7f9aa988ee280cebaef5301fcbc3.nq.gz
│   ├── d12161e88da78b17985457f1ff92da02c52a822e.nq.gz
│   ├── d645695673349e3947e8e5ae42332d0ac3164cd7.nq.gz
│   ├── d780829a1f5101333577a1ca9adcb960529213f1.nq.gz
│   ├── db177d4ac70f76c2172ce65ca33c830d6cbd3ac5.nq.gz
│   ├── e1c363713b30b8052cdaa86fb3ce473fe3d2e111.nq.gz
│   ├── e66063982424b7f2a6aeb73beae8d5125686fc9a.nq.gz
│   ├── e85d3d991a480d0e8ef6cddd31bd0ed49aff9d3a.nq.gz
│   ├── eb46a96bad9159fc8089ddd5d39b49eed990802f.nq.gz
│   ├── efacf6298c09a7f707bad0284b86462d22536994.nq.gz
│   ├── f412b5948870fc35486b715b4209a6f661b077e7.nq.gz
│   ├── f60e960282e291138dadfb89bcb749e98328b5d1.nq.gz
│   ├── f8fd5ffcf79ca28695f45aba155c97c17236bb45.nq.gz
│   └── ff42349c797a44065b17ddf21fea8fc7a341745e.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 427f45075f84b8b9774950196ad63867ca20ffb3.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 49 files
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

[google-deepmind/mathematics_dataset](https://github.com/google-deepmind/mathematics_dataset)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
