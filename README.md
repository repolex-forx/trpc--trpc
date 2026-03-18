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
│   │   ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
│   │   ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
│   │   ├── 4fa8f77bcfbbe7707042cc584aeecf4e54421600.nq.gz
│   │   ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
│   │   ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
│   │   ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
│   │   ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
│   │   ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
│   │   ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
│   │   ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
│   │   ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
│   │   ├── bff29e906b73a8f52ef8f9ef7c10b49067413641.nq.gz
│   │   ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
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
│   │   ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
│   │   ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
│   │   ├── 4fa8f77bcfbbe7707042cc584aeecf4e54421600.nq.gz
│   │   ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
│   │   ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
│   │   ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
│   │   ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
│   │   ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
│   │   ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
│   │   ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
│   │   ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
│   │   ├── bff29e906b73a8f52ef8f9ef7c10b49067413641.nq.gz
│   │   ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
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
│   │   ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
│   │   ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
│   │   ├── 4fa8f77bcfbbe7707042cc584aeecf4e54421600.nq.gz
│   │   ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
│   │   ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
│   │   ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
│   │   ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
│   │   ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
│   │   ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
│   │   ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
│   │   ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
│   │   ├── bff29e906b73a8f52ef8f9ef7c10b49067413641.nq.gz
│   │   ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
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
│       ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
│       ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
│       ├── 4fa8f77bcfbbe7707042cc584aeecf4e54421600.nq.gz
│       ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
│       ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
│       ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
│       ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
│       ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
│       ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
│       ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
│       ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
│       ├── bff29e906b73a8f52ef8f9ef7c10b49067413641.nq.gz
│       ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
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
    ├── 002e27a410d6d00041f05468693a989b03e5a280.nq.gz
    ├── 004404de981a8ae6ba75992cb4f66606ccc6b433.nq.gz
    ├── 0066745d0cc34b7045017ff99b58baf4172fcc6c.nq.gz
    ├── 007692e6321e9608afb5a22ad8a012a75a9cffab.nq.gz
    ├── 00b8704851b541625b24233400e866c046d2ae5c.nq.gz
    ├── 0112e00f0b4bccb3a01e9eac28a1cd3a04b29723.nq.gz
    ├── 0143177a04eabc626297a100f0c6061c13e07142.nq.gz
    ├── 0174c9352764f58caab6035b67c242c687124720.nq.gz
    ├── 01811bdea5de23e3122a0ef80ed8730782c0c792.nq.gz
    ├── 01daf3c3ad45720be4b1f25ea831728975b00669.nq.gz
    ├── 01dc39397a65f6a52c205400cb62eb6b9db31435.nq.gz
    ├── 01f1981dec6808d6459965c9bbec82c579b98e58.nq.gz
    ├── 0229e61f97cd030c54045f54f3bef57924643e47.nq.gz
    ├── 022ec8eb20d14081953c6ae669758ec863fcab36.nq.gz
    ├── 0237df2ec35d7646adcda333c28dfa6868182ba1.nq.gz
    ├── 02756b45e2c489a61adbffa63741ed2f06d450c8.nq.gz
    ├── 02aeb971e4fbb9f7fcae7b02497a4585092a796f.nq.gz
    ├── 02bde5a0d40620854b74c5c23a8594575bdf0eb7.nq.gz
    ├── 02c57fce05530fd42ec5b9a96d1deaaaa43b13c2.nq.gz
    ├── 02e645cf5ad901c103591955411c90c79b8efa39.nq.gz
    ├── 03c74a970112d80f8c8532a6d193654f02477e89.nq.gz
    ├── 03d504e67bf4128ca92c36c1423e7e8cfe685af6.nq.gz
    ├── 03e9f1cf68d1cc8de726767a81dbb14790c07490.nq.gz
    ├── 040264a07eadba18c740fd1182f62ef70c2619f5.nq.gz
    ├── 040a7b92096b8b2b39ac75d7a85d9c3e9a2177f3.nq.gz
    ├── 04290f398e3657ce650b9e0d7b48e203e6704739.nq.gz
    ├── 046425b3beb8efaa10f0f26299756efb8da0179f.nq.gz
    ├── 04f724c67aa22846f3a4307464b2cdb1d2278373.nq.gz
    ├── 0525ac7149cbe29c28186ad277e3d2b574ba77be.nq.gz
    ├── 05b5b3e76ed67d35b59d1e9fcec7a124e4604846.nq.gz
    ├── 05dd7f67efea0d0feee9cd81eb7e71dbce8b9cdb.nq.gz
    ├── 05e4493a206ab156d3b77d25369345d2e0a49c77.nq.gz
    ├── 063dc8e9ee52cf6e5425d1f238836dc0e8b5b27e.nq.gz
    ├── 065b5a6f67b4cdec5c13411f5715469350aa6518.nq.gz
    ├── 0688c4e69f698a9348d55136713f69b4d035c8b1.nq.gz
    ├── 0714eeb2065108f120a09a2fba41071e01e8f405.nq.gz
    ├── 07190e9507ff4043fb8fa1feedd0abf9615c5b00.nq.gz
    ├── 073a227dee3d848021bb15eba7f7e31ad9f572b8.nq.gz
    ├── 07448d96391661f7eed2e406bb7a1819b8041325.nq.gz
    ├── 075d343b4bb1874b0e42dc470c134c0359b5c509.nq.gz
    ├── 0775c99398d7ab87faeee99c775dddc92def2030.nq.gz
    ├── 0793ce54875ebf88db3d4f95f43ee300231db4cc.nq.gz
    ├── 07b1204a2066ff25970356a26f2344d4ca55e641.nq.gz
    ├── 07bb0371d69f22870e94dedb7e003a35403d670f.nq.gz
    ├── 07d5b90b87e1d070ac5b438f023fa2e316c36be2.nq.gz
    ├── 083d3f834119d9f8f49cafeb0d6a7af48705e813.nq.gz
    ├── 088cf9d209b2cee4b0a37050c13453532acf0e52.nq.gz
    ├── 08c31d0b81dad6fb00bd9e813661f1e9327bd7a7.nq.gz
    ├── 09664c31e0deb9856ba736a78d5dba057264e9a8.nq.gz
    ├── 099de9f2427cb831a7eb1afbed612ba1c4ee3c8e.nq.gz
    ├── 09a58adeec0a2e10ab61898e12ac2fb01e1ad57d.nq.gz
    ├── 09b9a5f89b07c2cccea20c64c0d2ef358f3291a7.nq.gz
    ├── 09ce686267f67a955f1d3360ade4126ab3ddae24.nq.gz
    ├── 09d16ddf178adbd9ca1053822cc7a84096f7a595.nq.gz
    ├── 0a2fcff8fbc870c5414dd72cae2241b4fdec3a6f.nq.gz
    ├── 0ab62329eb9f8236e03c81c51c6e4015e988ca8b.nq.gz
    ├── 0aecc68074a53a9793daacdb2cccf2412f8ec80e.nq.gz
    ├── 0b14b222b726aa90edd4b89bfd6240437aab1480.nq.gz
    ├── 0b6bd21e4850e4a6473f37e35f623082e8902a02.nq.gz
    ├── 0b91bd9b3491a459b6322d6b1e8ddd1366e8a07c.nq.gz
    ├── 0bff437be833e9552fd963086dee65f92ffdfb09.nq.gz
    ├── 0c0c9b271cc0c1abd7a80ff30f6e6f76d7a9de63.nq.gz
    ├── 0c3108bbdde73ca722663946cf322a8b8d5b63e0.nq.gz
    ├── 0c4ff9a268b0725a6f22d254389fd044caa78d6b.nq.gz
    ├── 0c81dfb103c2fbfea0309d1b1d42608e14e4ec9d.nq.gz
    ├── 0ccbfa761ec76a6357d7a9e4e7c6aa007084c526.nq.gz
    ├── 0ccfcab5be23259276dae2486a03986c7c8c5d5f.nq.gz
    ├── 0cd6f4b8573e65077827a17f51b8b368732bc1b8.nq.gz
    ├── 0d30a721304f3f6765a44dc69cab9527763030df.nq.gz
    ├── 0d39be9ad5e34db3d0899342c84be1da83a6e962.nq.gz
    ├── 0daab02c2482402432775c0f843044ce9b1f6083.nq.gz
    ├── 0dbc82bf4ff3e1dadaddb06b6451d2a3bb1361da.nq.gz
    ├── 0e086b9c62f429bd94f3e002d888955fc1cd8ef7.nq.gz
    ├── 0e4b960dcec1d9a4ca6d0d0afe9599260cfb7619.nq.gz
    ├── 0e99f1818150cf16aa66951311cddb15f0b92ad5.nq.gz
    ├── 0ed5a69aa7131104df0e9b690309cc82143a73d4.nq.gz
    ├── 0f2192fde06002f5b12059dd97eab8599b7fa40a.nq.gz
    ├── 0f49bd65460cd5abfbcf3183b6cdc46c64305034.nq.gz
    ├── 0f74bf1d5113ccbe700a8fb1e817e94c1470baed.nq.gz
    └── 0f908be14c48d4224d9bfde2313e43b64974e80d.nq.gz

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
*Parsed on 2026-03-18 by [repolex](https://repolex.ai)*
