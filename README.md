# Repolex Knowledge Graph of spatialaudio/jackclient-python

RDF knowledge graph data for [spatialaudio/jackclient-python](https://github.com/spatialaudio/jackclient-python), parsed by [repolex](https://repolex.ai).

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
rlex download spatialaudio/jackclient-python
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 1dc4598dbb02fcba7cfeb3eb41853edf70cd1109
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 1dc4598dbb02fcba7cfeb3eb41853edf70cd1109
│           └── chunk-001.nq.gz
├── blob
│   ├── 0de24862a8cfb14c6e99b5c0d003068706b1f712.nq.gz
│   ├── 11c36b7005178e86930018763e301674872a620d.nq.gz
│   ├── 1365c129ff5efa9577356218f3672206f3e9e283.nq.gz
│   ├── 247496e2a212ae79218dbdca2b2192197baff586.nq.gz
│   ├── 2501d725abb6f39329d6f08e77b57c8478842a6c.nq.gz
│   ├── 25e8033f039d46254c83d70f620524aba3440de9.nq.gz
│   ├── 38506255070bd8825299595f2a776394e8f323dd.nq.gz
│   ├── 445f4ee2f9f9510689bc8dee12db0824e4d80b4b.nq.gz
│   ├── 4c3dde898872a07668566642bfdd274349ab05ef.nq.gz
│   ├── 50080492c3bf765b03c2a5ae5ae38128c31d8ec4.nq.gz
│   ├── 54549b245864bcc92b9805ce113f27f8bf498d89.nq.gz
│   ├── 56aaee4e6e7209bbaf84b969cb01864fd5cb9f4c.nq.gz
│   ├── 657d7ae052deac94a3108c3b390222e082aadec9.nq.gz
│   ├── 68a3c2232c46bc3ef09047e7c0dcf0b5a422bd05.nq.gz
│   ├── 7c89417a91b91647648ca02a0000eaad53b8d4bb.nq.gz
│   ├── 7fd319de89bd2fd4095cf094c0dbd9f8edd86757.nq.gz
│   ├── 816dba02c933521a68447d808dfaf4b6e126d5e9.nq.gz
│   ├── 8182c2a56ab52e4120a0f52e26e8c4cb090826b7.nq.gz
│   ├── 8352196a4084e03f64fda6ea909d6ed446d90557.nq.gz
│   ├── 87fc91ab3a555822d237515d282141e707fd3508.nq.gz
│   ├── 973ebb4e51070bc9bea073dc0ece9156df7d6a3e.nq.gz
│   ├── 974ea9c52155ff39315bf72de795a48956c44b6e.nq.gz
│   ├── a465bad16c73cd677188c548fc7d9dd6d3f1ea67.nq.gz
│   ├── a5d528340e08969d48068c4e8f4ea8a13988afd3.nq.gz
│   ├── aa09feac8b41a2a2e331d8c3bf542a249e804ac3.nq.gz
│   ├── b4f6a79c580ce012482b593ba38fff9e9bebcec9.nq.gz
│   ├── b9825d81696a0dbe39c3cd279670ba77e11c4220.nq.gz
│   ├── bc3a5c94e80b971f4d8d817fdfdd28d49847a6fa.nq.gz
│   ├── bf595edeef6047aa3e65b1eb33abed0ebaf9cb3b.nq.gz
│   ├── c421856dd2fe638882cc71b74ed81e873ba5a219.nq.gz
│   ├── c766b7ed1695a1298116e375432cb7776ca599b6.nq.gz
│   ├── cbea989df6f15d8ced8a5a8bf1a70c57323c6d28.nq.gz
│   ├── d8bb83faec20dd62c8030c11cd76fedfa024a606.nq.gz
│   ├── dfae0ddd0b182f9ce4d62cd9fb908c4fdb7a036e.nq.gz
│   ├── dfea982b90606eb97a09075a3b515f19060f9e30.nq.gz
│   ├── e582053ea018c369be05aae96cf730744f1dc616.nq.gz
│   ├── e71703a7648919e7cd346406f616ee78aca847b7.nq.gz
│   ├── e90b07a84cf1463ba322de767e0a1f907f34d7af.nq.gz
│   ├── ebcc63cf681a889e84bf9cc7e88caeb454c5a2b5.nq.gz
│   └── f7c7adb51c43b6f92a9c047226ecb521723ac4d1.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 1dc4598dbb02fcba7cfeb3eb41853edf70cd1109.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 48 files
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

[spatialaudio/jackclient-python](https://github.com/spatialaudio/jackclient-python)

---
*Parsed on 2026-10-28 by [repolex](https://repolex.ai)*
