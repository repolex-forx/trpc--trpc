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
├── aggregate
│   ├── ast
│   │   ├── 1b9e65aed95202531b9f2afbc3ec8e05ae353513.nq.gz
│   │   ├── 2581b3d1c674c2c775d2e12d9f3b653efe40d5dd.nq.gz
│   │   ├── 3102802183e37cb08e1d48f636eb5bfef9a813e7.nq.gz
│   │   ├── 38d756d8b588e8ddd614633e5dcb509a23064c6e.nq.gz
│   │   ├── 3c2825801545605b636921bb14c1234efb7c9a2c.nq.gz
│   │   ├── 3fb0a5a1090330bbe0f08650c4d62568d1be8528.nq.gz
│   │   ├── 471a69c2d6997b8d5dfa1887fd62b24ada31a4d3.nq.gz
│   │   ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
│   │   ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
│   │   ├── 4fa8f77bcfbbe7707042cc584aeecf4e54421600.nq.gz
│   │   ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
│   │   ├── 6c1e5ad3c4eee7c4be6d7a220b50d64cf58eaeb8.nq.gz
│   │   ├── 79f545134b8a30b7b3f866dc2dd219303d9e8c05.nq.gz
│   │   ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
│   │   ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
│   │   ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
│   │   ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
│   │   ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
│   │   ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
│   │   ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
│   │   ├── bfcabb55010f3e6612308595a79f6be3637d38d8.nq.gz
│   │   ├── bff29e906b73a8f52ef8f9ef7c10b49067413641.nq.gz
│   │   ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
│   │   ├── c31f87835c2f8cec5cdb67f269fdf4d030e275eb.nq.gz
│   │   ├── c4138897578949d910dd0bce9e1471a6ae73137e.nq.gz
│   │   ├── c6f4be284b3a7b35455339b2b5566e2c75e9168e.nq.gz
│   │   ├── d4d5e7a347c39d2169a87fdb207de669db60758b.nq.gz
│   │   ├── e0153995c36c0f0b2ffb4ce0fdd02690607d50c0.nq.gz
│   │   ├── e4812361ceb1735e0b04281e908d538a32d21ad7.nq.gz
│   │   ├── e4bb8cdd4aaba3bdd128ca25dfa72752c44db261.nq.gz
│   │   ├── e9f4f7750c0ff7b66c1ff291e45a42eb86d05f8a.nq.gz
│   │   ├── ee9dfa1b3028c8919b37b9fdc0419cfbd70d1573.nq.gz
│   │   ├── f7663b07e41b6411fa9517acbba83a5c5cfb167f.nq.gz
│   │   ├── f944ac0c3bcb90e7bc4d8a08ecd3da988c5b12af.nq.gz
│   │   ├── fbc382148832adc2ea95220e81220bd614cd169f.nq.gz
│   │   └── ff3026c8cf47ea68878f57ec8fd41acd34b1879c.nq.gz
│   ├── dataflow
│   │   ├── 1b9e65aed95202531b9f2afbc3ec8e05ae353513.nq.gz
│   │   ├── 2581b3d1c674c2c775d2e12d9f3b653efe40d5dd.nq.gz
│   │   ├── 3102802183e37cb08e1d48f636eb5bfef9a813e7.nq.gz
│   │   ├── 38d756d8b588e8ddd614633e5dcb509a23064c6e.nq.gz
│   │   ├── 3c2825801545605b636921bb14c1234efb7c9a2c.nq.gz
│   │   ├── 3fb0a5a1090330bbe0f08650c4d62568d1be8528.nq.gz
│   │   ├── 471a69c2d6997b8d5dfa1887fd62b24ada31a4d3.nq.gz
│   │   ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
│   │   ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
│   │   ├── 4fa8f77bcfbbe7707042cc584aeecf4e54421600.nq.gz
│   │   ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
│   │   ├── 6c1e5ad3c4eee7c4be6d7a220b50d64cf58eaeb8.nq.gz
│   │   ├── 79f545134b8a30b7b3f866dc2dd219303d9e8c05.nq.gz
│   │   ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
│   │   ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
│   │   ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
│   │   ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
│   │   ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
│   │   ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
│   │   ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
│   │   ├── bfcabb55010f3e6612308595a79f6be3637d38d8.nq.gz
│   │   ├── bff29e906b73a8f52ef8f9ef7c10b49067413641.nq.gz
│   │   ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
│   │   ├── c31f87835c2f8cec5cdb67f269fdf4d030e275eb.nq.gz
│   │   ├── c4138897578949d910dd0bce9e1471a6ae73137e.nq.gz
│   │   ├── c6f4be284b3a7b35455339b2b5566e2c75e9168e.nq.gz
│   │   ├── d4d5e7a347c39d2169a87fdb207de669db60758b.nq.gz
│   │   ├── e0153995c36c0f0b2ffb4ce0fdd02690607d50c0.nq.gz
│   │   ├── e4812361ceb1735e0b04281e908d538a32d21ad7.nq.gz
│   │   ├── e4bb8cdd4aaba3bdd128ca25dfa72752c44db261.nq.gz
│   │   ├── e9f4f7750c0ff7b66c1ff291e45a42eb86d05f8a.nq.gz
│   │   ├── ee9dfa1b3028c8919b37b9fdc0419cfbd70d1573.nq.gz
│   │   ├── f7663b07e41b6411fa9517acbba83a5c5cfb167f.nq.gz
│   │   ├── f944ac0c3bcb90e7bc4d8a08ecd3da988c5b12af.nq.gz
│   │   ├── fbc382148832adc2ea95220e81220bd614cd169f.nq.gz
│   │   └── ff3026c8cf47ea68878f57ec8fd41acd34b1879c.nq.gz
│   ├── lsp
│   │   ├── 1b9e65aed95202531b9f2afbc3ec8e05ae353513.nq.gz
│   │   ├── 2581b3d1c674c2c775d2e12d9f3b653efe40d5dd.nq.gz
│   │   ├── 3102802183e37cb08e1d48f636eb5bfef9a813e7.nq.gz
│   │   ├── 38d756d8b588e8ddd614633e5dcb509a23064c6e.nq.gz
│   │   ├── 3c2825801545605b636921bb14c1234efb7c9a2c.nq.gz
│   │   ├── 3fb0a5a1090330bbe0f08650c4d62568d1be8528.nq.gz
│   │   ├── 471a69c2d6997b8d5dfa1887fd62b24ada31a4d3.nq.gz
│   │   ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
│   │   ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
│   │   ├── 4fa8f77bcfbbe7707042cc584aeecf4e54421600.nq.gz
│   │   ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
│   │   ├── 6c1e5ad3c4eee7c4be6d7a220b50d64cf58eaeb8.nq.gz
│   │   ├── 79f545134b8a30b7b3f866dc2dd219303d9e8c05.nq.gz
│   │   ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
│   │   ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
│   │   ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
│   │   ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
│   │   ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
│   │   ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
│   │   ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
│   │   ├── bfcabb55010f3e6612308595a79f6be3637d38d8.nq.gz
│   │   ├── bff29e906b73a8f52ef8f9ef7c10b49067413641.nq.gz
│   │   ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
│   │   ├── c31f87835c2f8cec5cdb67f269fdf4d030e275eb.nq.gz
│   │   ├── c4138897578949d910dd0bce9e1471a6ae73137e.nq.gz
│   │   ├── c6f4be284b3a7b35455339b2b5566e2c75e9168e.nq.gz
│   │   ├── d4d5e7a347c39d2169a87fdb207de669db60758b.nq.gz
│   │   ├── e0153995c36c0f0b2ffb4ce0fdd02690607d50c0.nq.gz
│   │   ├── e4812361ceb1735e0b04281e908d538a32d21ad7.nq.gz
│   │   ├── e4bb8cdd4aaba3bdd128ca25dfa72752c44db261.nq.gz
│   │   ├── e9f4f7750c0ff7b66c1ff291e45a42eb86d05f8a.nq.gz
│   │   ├── ee9dfa1b3028c8919b37b9fdc0419cfbd70d1573.nq.gz
│   │   ├── f7663b07e41b6411fa9517acbba83a5c5cfb167f.nq.gz
│   │   ├── f944ac0c3bcb90e7bc4d8a08ecd3da988c5b12af.nq.gz
│   │   ├── fbc382148832adc2ea95220e81220bd614cd169f.nq.gz
│   │   └── ff3026c8cf47ea68878f57ec8fd41acd34b1879c.nq.gz
│   └── repolex
│       ├── 1b9e65aed95202531b9f2afbc3ec8e05ae353513.nq.gz
│       ├── 2581b3d1c674c2c775d2e12d9f3b653efe40d5dd.nq.gz
│       ├── 3102802183e37cb08e1d48f636eb5bfef9a813e7.nq.gz
│       ├── 38d756d8b588e8ddd614633e5dcb509a23064c6e.nq.gz
│       ├── 3c2825801545605b636921bb14c1234efb7c9a2c.nq.gz
│       ├── 3fb0a5a1090330bbe0f08650c4d62568d1be8528.nq.gz
│       ├── 471a69c2d6997b8d5dfa1887fd62b24ada31a4d3.nq.gz
│       ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
│       ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
│       ├── 4fa8f77bcfbbe7707042cc584aeecf4e54421600.nq.gz
│       ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
│       ├── 6c1e5ad3c4eee7c4be6d7a220b50d64cf58eaeb8.nq.gz
│       ├── 79f545134b8a30b7b3f866dc2dd219303d9e8c05.nq.gz
│       ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
│       ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
│       ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
│       ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
│       ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
│       ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
│       ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
│       ├── bfcabb55010f3e6612308595a79f6be3637d38d8.nq.gz
│       ├── bff29e906b73a8f52ef8f9ef7c10b49067413641.nq.gz
│       ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
│       ├── c31f87835c2f8cec5cdb67f269fdf4d030e275eb.nq.gz
│       ├── c4138897578949d910dd0bce9e1471a6ae73137e.nq.gz
│       ├── c6f4be284b3a7b35455339b2b5566e2c75e9168e.nq.gz
│       ├── d4d5e7a347c39d2169a87fdb207de669db60758b.nq.gz
│       ├── e0153995c36c0f0b2ffb4ce0fdd02690607d50c0.nq.gz
│       ├── e4812361ceb1735e0b04281e908d538a32d21ad7.nq.gz
│       ├── e4bb8cdd4aaba3bdd128ca25dfa72752c44db261.nq.gz
│       ├── e9f4f7750c0ff7b66c1ff291e45a42eb86d05f8a.nq.gz
│       ├── ee9dfa1b3028c8919b37b9fdc0419cfbd70d1573.nq.gz
│       ├── f7663b07e41b6411fa9517acbba83a5c5cfb167f.nq.gz
│       ├── f944ac0c3bcb90e7bc4d8a08ecd3da988c5b12af.nq.gz
│       ├── fbc382148832adc2ea95220e81220bd614cd169f.nq.gz
│       └── ff3026c8cf47ea68878f57ec8fd41acd34b1879c.nq.gz
└── blob
    ├── 001af3b68f008ca4e720b7401bbe9f8a9b6c728b.nq.gz
    ├── 002b80c8b8e03f93ba60b5e31aea37b9e5858fe5.nq.gz
    ├── 002e27a410d6d00041f05468693a989b03e5a280.nq.gz
    ├── 003d94a1382a227593904aa0c04a1bee1366e47f.nq.gz
    ├── 004404de981a8ae6ba75992cb4f66606ccc6b433.nq.gz
    ├── 004de394616c417b6216569f2effeb2070622ffb.nq.gz
    ├── 00509147375d91e0a1fc9ff6a8e67fd43c3c9e00.nq.gz
    ├── 0051adc5111874bf1b24040f599975bedc1fde3d.nq.gz
    ├── 0053c259f99e11d3da1b30e1625b7c26b34f5248.nq.gz
    ├── 0055e54a94050675295f3c020e0b3e3130065da7.nq.gz
    ├── 0066745d0cc34b7045017ff99b58baf4172fcc6c.nq.gz
    ├── 0067db8987709161de54fe16c2f63398d0cd9c58.nq.gz
    ├── 006e8952540d23f3d53be56dd70f3ae83c46e9ab.nq.gz
    ├── 0072e19c13a2ef42212378cc3b8ea3d58a2ef58a.nq.gz
    ├── 007692e6321e9608afb5a22ad8a012a75a9cffab.nq.gz
    ├── 00816b9168b792df54eece81f4c4978c54b60b9a.nq.gz
    ├── 008a45d7ab0869784bdbd95f5c7d0ec890d277cf.nq.gz
    ├── 0097f7dec47cae26aa3330e53cda8e264edf1bb5.nq.gz
    ├── 009dc6e95d49238abc072ea5dea413895b4810e7.nq.gz
    ├── 009dd2f418b3264d1782c79c3ca7e802f08392c3.nq.gz
    ├── 00a130ea959c1605e1203934354daa0c19e45c54.nq.gz
    ├── 00a60ff63e67181cb42e76b38f4b4abe571cb8f9.nq.gz
    ├── 00ac3d8cc4a916cb042cdd479ea3f6b39fbf8f18.nq.gz
    ├── 00b8704851b541625b24233400e866c046d2ae5c.nq.gz
    ├── 00d9f219e9f752feab2427ed9268a14ff9ef2e10.nq.gz
    ├── 00eb9c004856c853ca3b43a5b8507fedcacd186a.nq.gz
    ├── 0106803d171d04bf0d7c5728874bcc419c696e8f.nq.gz
    ├── 010b933fd2708bd5d492b6da0a8d63404e460fc1.nq.gz
    ├── 010e4683d40ca6fb430c0bf5298a5e459d358f72.nq.gz
    ├── 0112e00f0b4bccb3a01e9eac28a1cd3a04b29723.nq.gz
    ├── 011594c60a28e097000aa97f7b31186a086d4085.nq.gz
    ├── 011d3ca8bed2377081b19aa69492ec0092c68f1f.nq.gz
    ├── 01208ef39cb145303906ae3f7546c6a14f45452b.nq.gz
    ├── 01225344b2e0da4b0a1a471d661cd25862963c26.nq.gz
    ├── 0143177a04eabc626297a100f0c6061c13e07142.nq.gz
    ├── 014c271033e7d7235d078314afa22bc3a559551d.nq.gz
    ├── 0151982db5cfb6d392a5ddd847559f3891aa24d2.nq.gz
    ├── 015781a02fb29169091e748ac23d270e03836fb2.nq.gz
    ├── 015e2a1ec199492d11c5a63a882daa436a73a99d.nq.gz
    ├── 0174c9352764f58caab6035b67c242c687124720.nq.gz
    ├── 01811bdea5de23e3122a0ef80ed8730782c0c792.nq.gz
    ├── 018258c9e2594cdb81cecbc3b4a3f133b0abeee0.nq.gz
    ├── 0182823744a544f9ebe572a69a7711cbabadf4ce.nq.gz
    ├── 019f1862eec7e38c197278c6e33997effc4d3c0e.nq.gz
    ├── 01a47061de6d23c8f9e4509dc0f6565d393842aa.nq.gz
    ├── 01abe4ea6c17c8b7e47875dd717b8847d4a75da5.nq.gz
    ├── 01afc597b476aa5253619afbf0f056cb74917bc0.nq.gz
    ├── 01b225e7f6bc423360270678b6eb3296191a98b5.nq.gz
    ├── 01b6c0bcb92516b1b8ffbd49ab65c613257ba078.nq.gz
    ├── 01bef03abb2e6015db3cd1a0f43ac82510a7ea3a.nq.gz
    ├── 01bf7432f67fa9a4fd3ebe3ca0fb9b18d3b791cb.nq.gz
    ├── 01bfebce8348cc5fe2466aaa8ea70e9b37cf309e.nq.gz
    ├── 01c91597dafb7ec9038ba138b614cab889c543d1.nq.gz
    ├── 01cc0b086bca7281ff07027f22566e4ea0873fbc.nq.gz
    ├── 01cd6cc99a5c8501decee24b60ee6a3d2d35b5d3.nq.gz
    └── 01cf6ac3723871cbc029b76cbec5d8256536b3be.nq.gz

7 directories, 200 files
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
*Parsed on 2026-03-22 by [repolex](https://repolex.ai)*
