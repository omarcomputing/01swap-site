# 01swap — built bundle

This repository holds **only the built dapp bundle**, published through GitHub
Pages so the seller and buyer flows can be exercised in a real browser. The
source lives in a separate private repository.

Nothing here is written by hand. Every file except this README is build output.

## What this build is pinned to

| | |
|---|---|
| Network | Oasis Sapphire **testnet** (chain 23295) |
| Vault | [`0x42eDC6dBD8919D00C17f68b64D69A866c9B306ba`](https://explorer.oasis.io/testnet/sapphire/address/0x42eDC6dBD8919D00C17f68b64D69A866c9B306ba) |
| Canonical host | `omarcomputing.github.io` |

The canonical host is baked in at build time and checked before anything
mounts. Opening this bundle on any other hostname shows a notice and refuses
to run — a seller's storage account is a passkey credential scoped to the
hostname that created it, so running elsewhere would silently produce a
different, empty account and strand the funded one.

## This is a testnet deployment

It spends testnet tokens only and is **disposable**. The tokens have no value
and come from faucets. Do not treat anything published through it as durable.
