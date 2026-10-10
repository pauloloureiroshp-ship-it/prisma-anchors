# Prisma · public anchors

This repository publishes **hash anchors** of Prisma's pre-registered measurement protocols, plans and rules.

Each file under `anchors/` holds the Merkle root (`sha256-merkle/1`) of every pre-registration that existed on that date. The root reveals nothing about clients, brands, files, costs or prompts. Its job is to let a third party check later that a protocol we show them existed, unchanged, on the date we claim: we hand over the item and its Merkle path, and anyone can recompute the root and compare it with the file here (git history dates each version).

Format:

```
prisma-anchor/1
date: YYYY-MM-DD
algorithm: sha256-merkle/1
items: <number of pre-registrations>
root: <64 hex characters>
```

Published by Prisma (prismalens.ai). Files are append-only: an anchor is never edited or deleted.

---

# Prisma · âncoras públicas

Este repositório publica as **âncoras de hash** dos protocolos, planos e regras pré-registrados do Prisma. Cada arquivo em `anchors/` traz a raiz Merkle de todos os pré-registros que existiam naquela data, sem nenhum dado de cliente, marca, custo ou prompt. Serve para que um terceiro confira depois que um protocolo existia, sem mudança, na data que afirmamos. Os arquivos só são acrescentados, nunca editados ou apagados.
