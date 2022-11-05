---
theme: purplin
colorSchema: 'light'
---

# Ethereum development with chaintool libraries.

Grassroots Economics (docs.grassecon.org)

By Louis Holbrook (manbytesgnu.com) & Mohamed Sohail (sohailazim.com)

<BarBottom  title="Ethereum development with chaintool libraries.">
  <Item text="chainlib-py">
    <carbon:logo-github />
  </Item>
</BarBottom>

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---

# What is chaintool?

An attempt at an agnostic approach to interface blockchain RPCs, while also providing tools for controlling transaction delivery and syncing of results.
  
- **Ethereum ready** - chaintool has been implemented for the EVM
- **Libraries** - both high level convenience functions and low level abstractions
- **CLI executable tools** - for common blockchain actions e.g. erc20 transfers, enc/dec bytecode e.t.c.
- **Blockchain event processing** - pluggable infrastructure for arbitary code execution on blockchain events

Other supporting libraries for general python development:

- **shep** - a bitfield-oriented state transition backend used in transaction submission queues
- **confini** - merges and validates configurations from multiple ini file sources
- **aiee** - an bitfield-oriented argument and environment settings helper for CLI tools
- ...and more


<BarBottom  title="Ethereum development with chaintool libraries.">
  <Item text="chainlib-py">
    <carbon:logo-github />
  </Item>
</BarBottom>

---

# Background

Why were chaintool libs written?
  
- Concurrency issues with celery / python web3
- GE stores and manipulates raw transaction data

**Current state:**

- Used in production at GE, over 100k custodial transactions to date


<BarBottom  title="Ethereum development with chaintool libraries.">
  <Item text="chainlib-py">
    <carbon:logo-github />
  </Item>
</BarBottom>

---

# chaind-eth demo

Ethereum queue syncer daemon

Use cases:

- Bulk gas gifting
- Token air dropping

Features:

- Pluggable input source, CSV implemented
- Full transaction lifecycle state management (create -> sign -> dispatch -> status)
- Pluggable storage provider

<BarBottom  title="Ethereum development with chaintool libraries.">
  <Item text="chainlib-py">
    <carbon:logo-github />
  </Item>
</BarBottom>

---

# CLI tools demo
CLI tools for commom Ethereum actions

Some of the CLI tools:

- eth-balance
- eth-gas
- eth-encode and eth-decode
- erc20-balance
- ...and more

<BarBottom  title="Ethereum development with chaintool libraries.">
  <Item text="chainlib-py">
    <carbon:logo-github />
  </Item>
</BarBottom>

---

# Roadmap

https://github.com/chaintool-py

- Improve concurrency support
- Other blockchain implementations
- Documentation

**We welcome contributors!**