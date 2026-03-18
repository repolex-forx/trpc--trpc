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
│   │   ├── 3102802183e37cb08e1d48f636eb5bfef9a813e7.nq.gz
│   │   ├── 38d756d8b588e8ddd614633e5dcb509a23064c6e.nq.gz
│   │   ├── 3c2825801545605b636921bb14c1234efb7c9a2c.nq.gz
│   │   ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
│   │   ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
│   │   ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
│   │   ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
│   │   ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
│   │   ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
│   │   ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
│   │   ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
│   │   ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
│   │   ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
│   │   ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
│   │   ├── c6f4be284b3a7b35455339b2b5566e2c75e9168e.nq.gz
│   │   ├── d4d5e7a347c39d2169a87fdb207de669db60758b.nq.gz
│   │   ├── e0153995c36c0f0b2ffb4ce0fdd02690607d50c0.nq.gz
│   │   ├── e4812361ceb1735e0b04281e908d538a32d21ad7.nq.gz
│   │   ├── e9f4f7750c0ff7b66c1ff291e45a42eb86d05f8a.nq.gz
│   │   ├── ee9dfa1b3028c8919b37b9fdc0419cfbd70d1573.nq.gz
│   │   ├── f944ac0c3bcb90e7bc4d8a08ecd3da988c5b12af.nq.gz
│   │   └── ff3026c8cf47ea68878f57ec8fd41acd34b1879c.nq.gz
│   ├── dataflow
│   │   ├── 1b9e65aed95202531b9f2afbc3ec8e05ae353513.nq.gz
│   │   ├── 3102802183e37cb08e1d48f636eb5bfef9a813e7.nq.gz
│   │   ├── 38d756d8b588e8ddd614633e5dcb509a23064c6e.nq.gz
│   │   ├── 3c2825801545605b636921bb14c1234efb7c9a2c.nq.gz
│   │   ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
│   │   ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
│   │   ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
│   │   ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
│   │   ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
│   │   ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
│   │   ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
│   │   ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
│   │   ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
│   │   ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
│   │   ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
│   │   ├── c6f4be284b3a7b35455339b2b5566e2c75e9168e.nq.gz
│   │   ├── d4d5e7a347c39d2169a87fdb207de669db60758b.nq.gz
│   │   ├── e0153995c36c0f0b2ffb4ce0fdd02690607d50c0.nq.gz
│   │   ├── e4812361ceb1735e0b04281e908d538a32d21ad7.nq.gz
│   │   ├── e9f4f7750c0ff7b66c1ff291e45a42eb86d05f8a.nq.gz
│   │   ├── ee9dfa1b3028c8919b37b9fdc0419cfbd70d1573.nq.gz
│   │   ├── f944ac0c3bcb90e7bc4d8a08ecd3da988c5b12af.nq.gz
│   │   └── ff3026c8cf47ea68878f57ec8fd41acd34b1879c.nq.gz
│   ├── lsp
│   │   ├── 1b9e65aed95202531b9f2afbc3ec8e05ae353513.nq.gz
│   │   ├── 3102802183e37cb08e1d48f636eb5bfef9a813e7.nq.gz
│   │   ├── 38d756d8b588e8ddd614633e5dcb509a23064c6e.nq.gz
│   │   ├── 3c2825801545605b636921bb14c1234efb7c9a2c.nq.gz
│   │   ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
│   │   ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
│   │   ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
│   │   ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
│   │   ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
│   │   ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
│   │   ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
│   │   ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
│   │   ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
│   │   ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
│   │   ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
│   │   ├── c6f4be284b3a7b35455339b2b5566e2c75e9168e.nq.gz
│   │   ├── d4d5e7a347c39d2169a87fdb207de669db60758b.nq.gz
│   │   ├── e0153995c36c0f0b2ffb4ce0fdd02690607d50c0.nq.gz
│   │   ├── e4812361ceb1735e0b04281e908d538a32d21ad7.nq.gz
│   │   ├── e9f4f7750c0ff7b66c1ff291e45a42eb86d05f8a.nq.gz
│   │   ├── ee9dfa1b3028c8919b37b9fdc0419cfbd70d1573.nq.gz
│   │   ├── f944ac0c3bcb90e7bc4d8a08ecd3da988c5b12af.nq.gz
│   │   └── ff3026c8cf47ea68878f57ec8fd41acd34b1879c.nq.gz
│   └── repolex
│       ├── 1b9e65aed95202531b9f2afbc3ec8e05ae353513.nq.gz
│       ├── 3102802183e37cb08e1d48f636eb5bfef9a813e7.nq.gz
│       ├── 38d756d8b588e8ddd614633e5dcb509a23064c6e.nq.gz
│       ├── 3c2825801545605b636921bb14c1234efb7c9a2c.nq.gz
│       ├── 4b7273324d09c609fbb3b22d0b393de7b942c984.nq.gz
│       ├── 4e2b3fde9f3581e69034b37bd1764e531a873409.nq.gz
│       ├── 50c16d03b3d61e5f49e24731c3b4b79d1c20a8ad.nq.gz
│       ├── 7d3802466387437709589b16325d0417fc85eeef.nq.gz
│       ├── 7da1847b07167d880e3e4a0c7ec2bebfc75af8c5.nq.gz
│       ├── 8b352b18cd900c5707afe6201c749c84625041d0.nq.gz
│       ├── 93325f01a5713de75171940b90738b2713b3bb07.nq.gz
│       ├── a781ed088e72b49702359d4f9368cf2ddabe6130.nq.gz
│       ├── afefcf0556784d364778a7fef573716d174134cd.nq.gz
│       ├── b3d4b9ff0cf63e9f8d09554907dcb9690d40084c.nq.gz
│       ├── c2cb43d42c55fefbda324dfaa2c58e88c5116d36.nq.gz
│       ├── c6f4be284b3a7b35455339b2b5566e2c75e9168e.nq.gz
│       ├── d4d5e7a347c39d2169a87fdb207de669db60758b.nq.gz
│       ├── e0153995c36c0f0b2ffb4ce0fdd02690607d50c0.nq.gz
│       ├── e4812361ceb1735e0b04281e908d538a32d21ad7.nq.gz
│       ├── e9f4f7750c0ff7b66c1ff291e45a42eb86d05f8a.nq.gz
│       ├── ee9dfa1b3028c8919b37b9fdc0419cfbd70d1573.nq.gz
│       ├── f944ac0c3bcb90e7bc4d8a08ecd3da988c5b12af.nq.gz
│       └── ff3026c8cf47ea68878f57ec8fd41acd34b1879c.nq.gz
└── blob
    ├── 002e27a410d6d00041f05468693a989b03e5a280.nq.gz
    ├── 004404de981a8ae6ba75992cb4f66606ccc6b433.nq.gz
    ├── 0066745d0cc34b7045017ff99b58baf4172fcc6c.nq.gz
    ├── 007692e6321e9608afb5a22ad8a012a75a9cffab.nq.gz
    ├── 0174c9352764f58caab6035b67c242c687124720.nq.gz
    ├── 01f1981dec6808d6459965c9bbec82c579b98e58.nq.gz
    ├── 022ec8eb20d14081953c6ae669758ec863fcab36.nq.gz
    ├── 0237df2ec35d7646adcda333c28dfa6868182ba1.nq.gz
    ├── 02bde5a0d40620854b74c5c23a8594575bdf0eb7.nq.gz
    ├── 02e645cf5ad901c103591955411c90c79b8efa39.nq.gz
    ├── 03c74a970112d80f8c8532a6d193654f02477e89.nq.gz
    ├── 03d504e67bf4128ca92c36c1423e7e8cfe685af6.nq.gz
    ├── 03e9f1cf68d1cc8de726767a81dbb14790c07490.nq.gz
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
    ├── 07190e9507ff4043fb8fa1feedd0abf9615c5b00.nq.gz
    ├── 073a227dee3d848021bb15eba7f7e31ad9f572b8.nq.gz
    ├── 07bb0371d69f22870e94dedb7e003a35403d670f.nq.gz
    ├── 088cf9d209b2cee4b0a37050c13453532acf0e52.nq.gz
    ├── 099de9f2427cb831a7eb1afbed612ba1c4ee3c8e.nq.gz
    ├── 09a58adeec0a2e10ab61898e12ac2fb01e1ad57d.nq.gz
    ├── 09b9a5f89b07c2cccea20c64c0d2ef358f3291a7.nq.gz
    ├── 0ab62329eb9f8236e03c81c51c6e4015e988ca8b.nq.gz
    ├── 0aecc68074a53a9793daacdb2cccf2412f8ec80e.nq.gz
    ├── 0b6bd21e4850e4a6473f37e35f623082e8902a02.nq.gz
    ├── 0b91bd9b3491a459b6322d6b1e8ddd1366e8a07c.nq.gz
    ├── 0c0c9b271cc0c1abd7a80ff30f6e6f76d7a9de63.nq.gz
    ├── 0c3108bbdde73ca722663946cf322a8b8d5b63e0.nq.gz
    ├── 0c4ff9a268b0725a6f22d254389fd044caa78d6b.nq.gz
    ├── 0cd6f4b8573e65077827a17f51b8b368732bc1b8.nq.gz
    ├── 0d39be9ad5e34db3d0899342c84be1da83a6e962.nq.gz
    ├── 0dbc82bf4ff3e1dadaddb06b6451d2a3bb1361da.nq.gz
    ├── 0e086b9c62f429bd94f3e002d888955fc1cd8ef7.nq.gz
    ├── 0e4b960dcec1d9a4ca6d0d0afe9599260cfb7619.nq.gz
    ├── 0e99f1818150cf16aa66951311cddb15f0b92ad5.nq.gz
    ├── 0ed5a69aa7131104df0e9b690309cc82143a73d4.nq.gz
    ├── 0fd9beebe04cc98bbcadb50de3b031e06fcfd94a.nq.gz
    ├── 0ff4c3568ecef0f16b37b07c3e9a57421e294265.nq.gz
    ├── 100d2bab4ead0ee7c5bd53af837b3ac7cfb2f191.nq.gz
    ├── 114c61e6ea0d8d9209c1ccaacbbb4b9ec8f147e1.nq.gz
    ├── 11aac89448d9e1bc73f35b0ed8f96a86955cb91f.nq.gz
    ├── 11c267493e61b5fc47ed06cfa56b4c60fc832b76.nq.gz
    ├── 11cbc178ad12c5d024efe0bfbb1f4e59a9eab117.nq.gz
    ├── 11eef69c572056c4ddf9088452000d67b8a9261a.nq.gz
    ├── 123f397b1458b871991b90e56276cf948366bc6a.nq.gz
    ├── 12e476cf7be66414d8d17940e312edb7dae1041e.nq.gz
    ├── 1328234d2a0db656d9e5963d1fc609e2a456dbfd.nq.gz
    ├── 13732b6a84d6b520835943479015ce550e6690b6.nq.gz
    ├── 13c81a1ce8066b2bda7865c303a967e1772f0bad.nq.gz
    ├── 142312eee20ce374e3d7817ddf4503747070beab.nq.gz
    ├── 142dce13ebba1f28dde9d538cefd02b679de8806.nq.gz
    ├── 1437c53f70bc211ec65739ec4a8c2a4db5874c73.nq.gz
    ├── 14ac40680707742d8b48ce009dc738d936624b28.nq.gz
    ├── 14edd56dc2ea2a7b6d39a2d721b73a77dc036597.nq.gz
    ├── 15a918bdf1c1f5d8a9d3f9e7ae105ffeec2c6f88.nq.gz
    ├── 15f1c5a84620e4482335369bab435616e820862c.nq.gz
    ├── 161a058f4227aefac57df1fe6d171f0dd7ba47c6.nq.gz
    ├── 167836f78e0ad0e91ddfe946c49ecfd771715167.nq.gz
    ├── 16786daa7eb8f276a12f1c33da995e9c2801c901.nq.gz
    ├── 16bbd61d3a8eb91fae7adc3f51ac65a2d9150ded.nq.gz
    ├── 17faa72756bfb088aacf6d090adb0523263639e3.nq.gz
    ├── 18fc5fc03b552be9becea39bd9e300601dbdef93.nq.gz
    ├── 191e58de23508dd71dbdf42b039dfcdda24f3a13.nq.gz
    ├── 1a05a9308f928c508978db21003b1444d9183990.nq.gz
    ├── 1a0a95c1542b8e466343de8b6af71066a0ceac2e.nq.gz
    ├── 1a1e8a2f5bc1b7051b331778f4639c49524f6100.nq.gz
    ├── 1a413d8226de6b6476e1c6e6dd314e7f19cebdcb.nq.gz
    ├── 1ab3618568ce6bdc47e8ec40063e102e1e6f0315.nq.gz
    ├── 1aeb13af4e627f83509a597da713f45ba5b99afa.nq.gz
    ├── 1b0928fd9a283167c0e2c2dc7f3d6e346770b212.nq.gz
    ├── 1b3fd5a904f84b927a01d2226c073741ca904ce0.nq.gz
    ├── 1c331c47822a9bccb4c475953c43f415de175cbe.nq.gz
    ├── 1c6dda5dbecd525187ccbfc99d066154c3cb0fa2.nq.gz
    ├── 1c9fdf082d90dc8b7fb84f39ed9b5ceb29d822c4.nq.gz
    ├── 1d5098ac76e3573eb6fa0b8579af4bb53057e093.nq.gz
    ├── 1e955717b12e108ecfc5ffa5442e4e59b2e907c3.nq.gz
    ├── 1fc3625e380755eb6be4c5474d0cc369fca7867b.nq.gz
    ├── 203fe2c39413efa3e29487aba2b82b59964bc326.nq.gz
    ├── 2071b6d16df06517c9b8c86e8b43927f9422fabd.nq.gz
    ├── 207f8a183205f35842271f97a1d7545d9d0eafe0.nq.gz
    ├── 20c362089dcee5e9d94ca09c8d9a70b0e916b0d7.nq.gz
    ├── 20c8b2d7199f833e985315c57825c06d87e911a8.nq.gz
    ├── 20d30bedb9969a292a62638471426a6a6f3c5f9c.nq.gz
    ├── 20d404d36528faae5e19c474a7564a2079243b6c.nq.gz
    ├── 2102274e7dd356685594c32a23a72e049dd2e345.nq.gz
    ├── 211706b66ca1b8fa5be33deb7c58fe4845b47b9b.nq.gz
    ├── 21698ffcd22c722f57e1fc1c1058f91cf34040e5.nq.gz
    ├── 21813a71b3e59a3441fda4e5ca8e66f70a4f40f3.nq.gz
    ├── 218c8434e93e10167303a57d977ab5c1c9e46bc6.nq.gz
    ├── 21bb1acf7b5136114a6833b2b1a7736849092c0e.nq.gz
    ├── 21be381a506acadfd35b75c8d58ba60d17b67e90.nq.gz
    ├── 21f9f59829f556d40f519b66ca9c12ecaca88ad3.nq.gz
    ├── 222cd551eb167fad9a87f13dd8c0728c541a7579.nq.gz
    ├── 2255e3f51817daec798bc67156e0459f22f88b85.nq.gz
    ├── 23f0a7d18dd4848a4b36a519a066c80c5d28b3dd.nq.gz
    ├── 24d4d2dfff98abb690fb34a04f3b0103aa0aecbd.nq.gz
    ├── 2577205edd2a1fbb4d860017893eaf53fec96251.nq.gz
    ├── 25dcd7a51aac367fb9053ca4ff950d19358774ad.nq.gz
    ├── 25f694842d1832fe14028420cf5f90e18f8f3f1f.nq.gz
    └── 264fd55bccfe463be1c5bb235101d90dc0dce790.nq.gz

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
