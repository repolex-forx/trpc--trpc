# Repolex Knowledge Graph of trpc/trpc

RDF knowledge graph data for [trpc/trpc](https://github.com/trpc/trpc), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download trpc/trpc
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
└── aggregate
    ├── ast
    │   ├── 08f3ac714bd19f7f7cac7935b3f2dbe5386b4a90.nq.gz
    │   ├── 09177f0767bcd5878b0fe039bc7e53ab6e0fdaea.nq.gz
    │   ├── 0a2f99d211ae73ef34a039694fbcfb3f3a75ff74.nq.gz
    │   ├── 1b9e65aed95202531b9f2afbc3ec8e05ae353513.nq.gz
    │   ├── 1bf67dcc3d2d44a98405cf3c1900571cfe2d762e.nq.gz
    │   ├── 2581b3d1c674c2c775d2e12d9f3b653efe40d5dd.nq.gz
    │   ├── 3102802183e37cb08e1d48f636eb5bfef9a813e7.nq.gz
    │   ├── 38d756d8b588e8ddd614633e5dcb509a23064c6e.nq.gz
    │   ├── 3c2825801545605b636921bb14c1234efb7c9a2c.nq.gz
    │   ├── 3fb0a5a1090330bbe0f08650c4d62568d1be8528.nq.gz
    │   ├── 44e50cb6530999af5695d3c9301d84de593e1d00.nq.gz
    │   ├── 471a69c2d6997b8d5dfa1887fd62b24ada31a4d3.nq.gz
    │   ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
    │   ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
    │   ├── 4fa8f77bcfbbe7707042cc584aeecf4e54421600.nq.gz
    │   ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
    │   ├── 6c1e5ad3c4eee7c4be6d7a220b50d64cf58eaeb8.nq.gz
    │   ├── 6eb1642a4a0aba9eb5fe4c1aa2648f5bdf65fcde.nq.gz
    │   ├── 711f122307c9441c16606add544c0810308d3f79.nq.gz
    │   ├── 72c14127f7b799510c8dda78a9e72c6aa933457e.nq.gz
    │   ├── 79f545134b8a30b7b3f866dc2dd219303d9e8c05.nq.gz
    │   ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
    │   ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
    │   ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
    │   ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
    │   ├── 94113223dddb08649a5b91f85d942d74173578aa.nq.gz
    │   ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
    │   ├── ae296e6fb92935e0065bf969c498f7a1d3ad3684.nq.gz
    │   ├── aefe56bb3edd7b17b68e5a76eabed8528168313e.nq.gz
    │   ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
    │   ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
    │   ├── ba1b84048ae31942a9e4d411cf2a9bc3603915bf.nq.gz
    │   ├── bfcabb55010f3e6612308595a79f6be3637d38d8.nq.gz
    │   ├── bff29e906b73a8f52ef8f9ef7c10b49067413641.nq.gz
    │   ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
    │   ├── c31f87835c2f8cec5cdb67f269fdf4d030e275eb.nq.gz
    │   ├── c4138897578949d910dd0bce9e1471a6ae73137e.nq.gz
    │   ├── c6f4be284b3a7b35455339b2b5566e2c75e9168e.nq.gz
    │   ├── c90221a3058aa5c10e48a78399174b26f56046bb.nq.gz
    │   ├── d2a529de7ef004af7c5e3da815ca91548a0be7a8.nq.gz
    │   ├── d4d5e7a347c39d2169a87fdb207de669db60758b.nq.gz
    │   ├── d7747e5dcef086b59b6427aab467ae483f5b4a8e.nq.gz
    │   ├── d7b9442ba2979046417e49986ddcd58d54642347.nq.gz
    │   ├── e0153995c36c0f0b2ffb4ce0fdd02690607d50c0.nq.gz
    │   ├── e4812361ceb1735e0b04281e908d538a32d21ad7.nq.gz
    │   ├── e4bb8cdd4aaba3bdd128ca25dfa72752c44db261.nq.gz
    │   ├── e547e7e80e09148887cce9e03efd1bec4fe854f6.nq.gz
    │   ├── e8468a50b289b0231cf1ee92d0f5195fe20c0d44.nq.gz
    │   ├── e9f4f7750c0ff7b66c1ff291e45a42eb86d05f8a.nq.gz
    │   ├── ee9dfa1b3028c8919b37b9fdc0419cfbd70d1573.nq.gz
    │   ├── f7663b07e41b6411fa9517acbba83a5c5cfb167f.nq.gz
    │   ├── f7cb49f8c741e80b4af96b3fb4947eb87e73c913.nq.gz
    │   ├── f944ac0c3bcb90e7bc4d8a08ecd3da988c5b12af.nq.gz
    │   ├── fbc382148832adc2ea95220e81220bd614cd169f.nq.gz
    │   ├── fdc5e071cb566335071e70b8f58299e846fa6d83.nq.gz
    │   └── ff3026c8cf47ea68878f57ec8fd41acd34b1879c.nq.gz
    ├── dataflow
    │   ├── 1b9e65aed95202531b9f2afbc3ec8e05ae353513.nq.gz
    │   ├── 2581b3d1c674c2c775d2e12d9f3b653efe40d5dd.nq.gz
    │   ├── 3102802183e37cb08e1d48f636eb5bfef9a813e7.nq.gz
    │   ├── 38d756d8b588e8ddd614633e5dcb509a23064c6e.nq.gz
    │   ├── 3c2825801545605b636921bb14c1234efb7c9a2c.nq.gz
    │   ├── 3fb0a5a1090330bbe0f08650c4d62568d1be8528.nq.gz
    │   ├── 471a69c2d6997b8d5dfa1887fd62b24ada31a4d3.nq.gz
    │   ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
    │   ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
    │   ├── 4fa8f77bcfbbe7707042cc584aeecf4e54421600.nq.gz
    │   ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
    │   ├── 6c1e5ad3c4eee7c4be6d7a220b50d64cf58eaeb8.nq.gz
    │   ├── 79f545134b8a30b7b3f866dc2dd219303d9e8c05.nq.gz
    │   ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
    │   ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
    │   ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
    │   ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
    │   ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
    │   ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
    │   ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
    │   ├── bfcabb55010f3e6612308595a79f6be3637d38d8.nq.gz
    │   ├── bff29e906b73a8f52ef8f9ef7c10b49067413641.nq.gz
    │   ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
    │   ├── c31f87835c2f8cec5cdb67f269fdf4d030e275eb.nq.gz
    │   ├── c4138897578949d910dd0bce9e1471a6ae73137e.nq.gz
    │   ├── c6f4be284b3a7b35455339b2b5566e2c75e9168e.nq.gz
    │   ├── d4d5e7a347c39d2169a87fdb207de669db60758b.nq.gz
    │   ├── e0153995c36c0f0b2ffb4ce0fdd02690607d50c0.nq.gz
    │   ├── e4812361ceb1735e0b04281e908d538a32d21ad7.nq.gz
    │   ├── e4bb8cdd4aaba3bdd128ca25dfa72752c44db261.nq.gz
    │   ├── e9f4f7750c0ff7b66c1ff291e45a42eb86d05f8a.nq.gz
    │   ├── ee9dfa1b3028c8919b37b9fdc0419cfbd70d1573.nq.gz
    │   ├── f7663b07e41b6411fa9517acbba83a5c5cfb167f.nq.gz
    │   ├── f944ac0c3bcb90e7bc4d8a08ecd3da988c5b12af.nq.gz
    │   ├── fbc382148832adc2ea95220e81220bd614cd169f.nq.gz
    │   └── ff3026c8cf47ea68878f57ec8fd41acd34b1879c.nq.gz
    ├── lsp
    │   ├── 08f3ac714bd19f7f7cac7935b3f2dbe5386b4a90.nq.gz
    │   ├── 09177f0767bcd5878b0fe039bc7e53ab6e0fdaea.nq.gz
    │   ├── 0a2f99d211ae73ef34a039694fbcfb3f3a75ff74.nq.gz
    │   ├── 1b9e65aed95202531b9f2afbc3ec8e05ae353513.nq.gz
    │   ├── 1bf67dcc3d2d44a98405cf3c1900571cfe2d762e.nq.gz
    │   ├── 2581b3d1c674c2c775d2e12d9f3b653efe40d5dd.nq.gz
    │   ├── 3102802183e37cb08e1d48f636eb5bfef9a813e7.nq.gz
    │   ├── 38d756d8b588e8ddd614633e5dcb509a23064c6e.nq.gz
    │   ├── 3c2825801545605b636921bb14c1234efb7c9a2c.nq.gz
    │   ├── 3fb0a5a1090330bbe0f08650c4d62568d1be8528.nq.gz
    │   ├── 44e50cb6530999af5695d3c9301d84de593e1d00.nq.gz
    │   ├── 471a69c2d6997b8d5dfa1887fd62b24ada31a4d3.nq.gz
    │   ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
    │   ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
    │   ├── 4fa8f77bcfbbe7707042cc584aeecf4e54421600.nq.gz
    │   ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
    │   ├── 6c1e5ad3c4eee7c4be6d7a220b50d64cf58eaeb8.nq.gz
    │   ├── 6eb1642a4a0aba9eb5fe4c1aa2648f5bdf65fcde.nq.gz
    │   ├── 711f122307c9441c16606add544c0810308d3f79.nq.gz
    │   ├── 72c14127f7b799510c8dda78a9e72c6aa933457e.nq.gz
    │   ├── 79f545134b8a30b7b3f866dc2dd219303d9e8c05.nq.gz
    │   ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
    │   ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
    │   ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
    │   ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
    │   ├── 94113223dddb08649a5b91f85d942d74173578aa.nq.gz
    │   ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
    │   ├── ae296e6fb92935e0065bf969c498f7a1d3ad3684.nq.gz
    │   ├── aefe56bb3edd7b17b68e5a76eabed8528168313e.nq.gz
    │   ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
    │   ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
    │   ├── ba1b84048ae31942a9e4d411cf2a9bc3603915bf.nq.gz
    │   ├── bfcabb55010f3e6612308595a79f6be3637d38d8.nq.gz
    │   ├── bff29e906b73a8f52ef8f9ef7c10b49067413641.nq.gz
    │   ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
    │   ├── c31f87835c2f8cec5cdb67f269fdf4d030e275eb.nq.gz
    │   ├── c4138897578949d910dd0bce9e1471a6ae73137e.nq.gz
    │   ├── c6f4be284b3a7b35455339b2b5566e2c75e9168e.nq.gz
    │   ├── c90221a3058aa5c10e48a78399174b26f56046bb.nq.gz
    │   ├── d2a529de7ef004af7c5e3da815ca91548a0be7a8.nq.gz
    │   ├── d4d5e7a347c39d2169a87fdb207de669db60758b.nq.gz
    │   ├── d7747e5dcef086b59b6427aab467ae483f5b4a8e.nq.gz
    │   ├── d7b9442ba2979046417e49986ddcd58d54642347.nq.gz
    │   ├── e0153995c36c0f0b2ffb4ce0fdd02690607d50c0.nq.gz
    │   ├── e4812361ceb1735e0b04281e908d538a32d21ad7.nq.gz
    │   ├── e4bb8cdd4aaba3bdd128ca25dfa72752c44db261.nq.gz
    │   ├── e547e7e80e09148887cce9e03efd1bec4fe854f6.nq.gz
    │   ├── e8468a50b289b0231cf1ee92d0f5195fe20c0d44.nq.gz
    │   ├── e9f4f7750c0ff7b66c1ff291e45a42eb86d05f8a.nq.gz
    │   ├── ee9dfa1b3028c8919b37b9fdc0419cfbd70d1573.nq.gz
    │   ├── f7663b07e41b6411fa9517acbba83a5c5cfb167f.nq.gz
    │   ├── f7cb49f8c741e80b4af96b3fb4947eb87e73c913.nq.gz
    │   ├── f944ac0c3bcb90e7bc4d8a08ecd3da988c5b12af.nq.gz
    │   ├── fbc382148832adc2ea95220e81220bd614cd169f.nq.gz
    │   ├── fdc5e071cb566335071e70b8f58299e846fa6d83.nq.gz
    │   └── ff3026c8cf47ea68878f57ec8fd41acd34b1879c.nq.gz
    └── repolex
        ├── 08f3ac714bd19f7f7cac7935b3f2dbe5386b4a90.nq.gz
        ├── 09177f0767bcd5878b0fe039bc7e53ab6e0fdaea.nq.gz
        ├── 0a2f99d211ae73ef34a039694fbcfb3f3a75ff74.nq.gz
        ├── 1b9e65aed95202531b9f2afbc3ec8e05ae353513.nq.gz
        ├── 1bf67dcc3d2d44a98405cf3c1900571cfe2d762e.nq.gz
        ├── 2581b3d1c674c2c775d2e12d9f3b653efe40d5dd.nq.gz
        ├── 3102802183e37cb08e1d48f636eb5bfef9a813e7.nq.gz
        ├── 38d756d8b588e8ddd614633e5dcb509a23064c6e.nq.gz
        ├── 3c2825801545605b636921bb14c1234efb7c9a2c.nq.gz
        ├── 3fb0a5a1090330bbe0f08650c4d62568d1be8528.nq.gz
        ├── 44e50cb6530999af5695d3c9301d84de593e1d00.nq.gz
        ├── 471a69c2d6997b8d5dfa1887fd62b24ada31a4d3.nq.gz
        ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
        ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
        ├── 4fa8f77bcfbbe7707042cc584aeecf4e54421600.nq.gz
        ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
        ├── 6c1e5ad3c4eee7c4be6d7a220b50d64cf58eaeb8.nq.gz
        ├── 6eb1642a4a0aba9eb5fe4c1aa2648f5bdf65fcde.nq.gz
        ├── 711f122307c9441c16606add544c0810308d3f79.nq.gz
        ├── 72c14127f7b799510c8dda78a9e72c6aa933457e.nq.gz
        ├── 79f545134b8a30b7b3f866dc2dd219303d9e8c05.nq.gz
        ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
        ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
        ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
        ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
        ├── 94113223dddb08649a5b91f85d942d74173578aa.nq.gz
        ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
        ├── ae296e6fb92935e0065bf969c498f7a1d3ad3684.nq.gz
        ├── aefe56bb3edd7b17b68e5a76eabed8528168313e.nq.gz
        ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
        ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
        ├── ba1b84048ae31942a9e4d411cf2a9bc3603915bf.nq.gz
        ├── bfcabb55010f3e6612308595a79f6be3637d38d8.nq.gz
        ├── bff29e906b73a8f52ef8f9ef7c10b49067413641.nq.gz
        ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
        ├── c31f87835c2f8cec5cdb67f269fdf4d030e275eb.nq.gz
        ├── c4138897578949d910dd0bce9e1471a6ae73137e.nq.gz
        ├── c6f4be284b3a7b35455339b2b5566e2c75e9168e.nq.gz
        ├── c90221a3058aa5c10e48a78399174b26f56046bb.nq.gz
        ├── d2a529de7ef004af7c5e3da815ca91548a0be7a8.nq.gz
        ├── d4d5e7a347c39d2169a87fdb207de669db60758b.nq.gz
        ├── d7747e5dcef086b59b6427aab467ae483f5b4a8e.nq.gz
        ├── d7b9442ba2979046417e49986ddcd58d54642347.nq.gz
        ├── e0153995c36c0f0b2ffb4ce0fdd02690607d50c0.nq.gz
        ├── e4812361ceb1735e0b04281e908d538a32d21ad7.nq.gz
        ├── e4bb8cdd4aaba3bdd128ca25dfa72752c44db261.nq.gz
        ├── e547e7e80e09148887cce9e03efd1bec4fe854f6.nq.gz
        ├── e8468a50b289b0231cf1ee92d0f5195fe20c0d44.nq.gz
        ├── e9f4f7750c0ff7b66c1ff291e45a42eb86d05f8a.nq.gz
        ├── ee9dfa1b3028c8919b37b9fdc0419cfbd70d1573.nq.gz
        ├── f7663b07e41b6411fa9517acbba83a5c5cfb167f.nq.gz
        └── f7cb49f8c741e80b4af96b3fb4947eb87e73c913.nq.gz

6 directories, 200 files
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

## Source repository

[trpc/trpc](https://github.com/trpc/trpc)

---
*Parsed on 2026-03-31 by [repolex](https://repolex.ai)*
