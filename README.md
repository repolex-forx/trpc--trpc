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
    ├── 0051adc5111874bf1b24040f599975bedc1fde3d.nq.gz
    ├── 0066745d0cc34b7045017ff99b58baf4172fcc6c.nq.gz
    ├── 0067db8987709161de54fe16c2f63398d0cd9c58.nq.gz
    ├── 007692e6321e9608afb5a22ad8a012a75a9cffab.nq.gz
    ├── 0097f7dec47cae26aa3330e53cda8e264edf1bb5.nq.gz
    ├── 009dc6e95d49238abc072ea5dea413895b4810e7.nq.gz
    ├── 00a130ea959c1605e1203934354daa0c19e45c54.nq.gz
    ├── 00ac3d8cc4a916cb042cdd479ea3f6b39fbf8f18.nq.gz
    ├── 00b8704851b541625b24233400e866c046d2ae5c.nq.gz
    ├── 00d9f219e9f752feab2427ed9268a14ff9ef2e10.nq.gz
    ├── 010e4683d40ca6fb430c0bf5298a5e459d358f72.nq.gz
    ├── 0112e00f0b4bccb3a01e9eac28a1cd3a04b29723.nq.gz
    ├── 0143177a04eabc626297a100f0c6061c13e07142.nq.gz
    ├── 015781a02fb29169091e748ac23d270e03836fb2.nq.gz
    ├── 0174c9352764f58caab6035b67c242c687124720.nq.gz
    ├── 01811bdea5de23e3122a0ef80ed8730782c0c792.nq.gz
    ├── 01c91597dafb7ec9038ba138b614cab889c543d1.nq.gz
    ├── 01cc0b086bca7281ff07027f22566e4ea0873fbc.nq.gz
    ├── 01cd6cc99a5c8501decee24b60ee6a3d2d35b5d3.nq.gz
    ├── 01cf6ac3723871cbc029b76cbec5d8256536b3be.nq.gz
    ├── 01daf3c3ad45720be4b1f25ea831728975b00669.nq.gz
    ├── 01dc39397a65f6a52c205400cb62eb6b9db31435.nq.gz
    ├── 01f1981dec6808d6459965c9bbec82c579b98e58.nq.gz
    ├── 01f44e0ccbefb867e665340f8efcdbd7a30cd927.nq.gz
    ├── 02084e4031f5fc001e41366908321059d7239bc3.nq.gz
    ├── 02163fb472387e9f091a191694be311e30b53f9c.nq.gz
    ├── 0229e61f97cd030c54045f54f3bef57924643e47.nq.gz
    ├── 022ec8eb20d14081953c6ae669758ec863fcab36.nq.gz
    ├── 0237df2ec35d7646adcda333c28dfa6868182ba1.nq.gz
    ├── 02654857a0399602555657ceddbcbd9939249b5a.nq.gz
    ├── 026cb0aa97e23fab7f4cc3b7efd95493b37ef645.nq.gz
    ├── 0273a5a2e5c8ba0d3200037f3bc781244f45c931.nq.gz
    ├── 02756b45e2c489a61adbffa63741ed2f06d450c8.nq.gz
    ├── 027ef9c6fc1f130570d6dd993feb58c9594f7b56.nq.gz
    ├── 02aeb971e4fbb9f7fcae7b02497a4585092a796f.nq.gz
    ├── 02b498fc108a5bda2bb27fd458e352903792f54b.nq.gz
    ├── 02bde5a0d40620854b74c5c23a8594575bdf0eb7.nq.gz
    ├── 02c57fce05530fd42ec5b9a96d1deaaaa43b13c2.nq.gz
    ├── 02d1adb70d6314040895b7d62a458b36bca5549f.nq.gz
    ├── 02e645cf5ad901c103591955411c90c79b8efa39.nq.gz
    ├── 02fd14b8e065909c742dd9e579ccacfc44ff9295.nq.gz
    ├── 02fd29ea86cd776fbb23860135a0c678fc15a80d.nq.gz
    ├── 02ffd953521b83656f0a420587a3edea89dd5b3d.nq.gz
    ├── 0321e8a0e4a36d5b4980b5ec56fc333e32adee50.nq.gz
    ├── 0332c6b56bb31aab9baad7b9d2c30edaac7d2e60.nq.gz
    ├── 0350309134cadaa6a81f96a31a8236b45863125c.nq.gz
    ├── 035ae2ed00eda3f920b29fcd6769cb721448a54f.nq.gz
    ├── 03c0ba51ef858bb6fbfb90677dc2d257102202e2.nq.gz
    ├── 03c74a970112d80f8c8532a6d193654f02477e89.nq.gz
    ├── 03ca464a665705c06cd15ca764f29da5ebef1d96.nq.gz
    └── 03d17889c3b4c8f0e4dbcb044a750d054f0e4e23.nq.gz

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
*Parsed on 2026-03-21 by [repolex](https://repolex.ai)*
