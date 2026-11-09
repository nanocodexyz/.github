<p align="center">
  <img src="./logo.png" alt="nanocode" width="100%" />
</p>

Welcome to the Nanocode organization.

Nanocode is an SDK for frontier embedded agents, written in Rust. One core runs the same agent,
with the same prompts, durability and Hands, in a terminal, a Cloudflare Worker, a browser tab, a
Vercel Function, a Mac app or an iPhone.

You can install Nanocode on macOS and Linux in seconds via:

```
curl -L https://nanocodex.paradigm.xyz | bash
```

Then, in a new terminal run: `nc`.

That's it! If everything goes well, you will now have a coding agent in your terminal, and the same
agent is ready to embed in your own app:

- [nanocode](https://github.com/nanocodexyz/nanocode): the Rust SDK and the `nc` CLI
- [nanocode-ts](https://github.com/nanocodexyz/nanocode-ts): the SDK as one WebAssembly module, for Workers, Vercel, Node and browsers
- [nanocode-swift](https://github.com/nanocodexyz/nanocode-swift): the SDK for macOS and iOS, with AppKit and UIKit views

Try the live demos:

- [nanocode.xyz/cloudflare](https://nanocode.xyz/cloudflare): durable agents in Cloudflare Durable Objects ([source](https://github.com/nanocodexyz/durable-cloudflare))
- [nanocode.xyz/vercel](https://nanocode.xyz/vercel): durable agents on Vercel Workflows, with [ChatGPT-style](https://nanocode.xyz/vercel/chatgpt) and [Claude-style](https://nanocode.xyz/vercel/claude) clones ([source](https://github.com/nanocodexyz/durable-vercel))
- [nanocode.xyz/machines](https://nanocode.xyz/machines): an agent in your browser that pays for every token from your Tempo Wallet ([source](https://github.com/gakonst/nanocode-machines-web))

## Principles

Every repository here follows the same principles, from [nanocode's AGENTS.md](https://github.com/nanocodexyz/nanocode/blob/master/AGENTS.md):

- Keep code simple and changes small, matching the code around them.
- No code comments, doc comments, tests or test-only dependencies.
- No magic constants or arbitrary caps: a limit comes from a protocol, a measurement or caller policy. Invalid states surface; nothing hides them with silent truncation, clamping or fallbacks.
- Invalid states are unrepresentable: a lifecycle is one enum whose variants carry only what that phase has.
- Lock-free: no Mutex, RwLock or Condvar, and blocking I/O never runs on async workers.
- One workspace of reusable crates that build for native and WASM with parity.
- The real Claude and Codex prompts and tool shapes, version-pinned from upstream, with SDK additions kept apart.
- Inference, subagents and durability live in the brain; Code Mode runs on the user's machine. Dispatched work is never silently replayed: an uncertain outcome is reported as unknown.
- Every performance change comes with reproducible before/after measurements.
- Everything lands on master and is built, released and deployed by hand: no pull requests, no CI.

See the [Nanocode Docs](https://nanocode.xyz) for more.

Nanocode development is spearheaded by [Paradigm](https://github.com/paradigmxyz) and the open-source community.
