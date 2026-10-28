# Nanocode

<img src="./logo.svg" alt="Nanocode logo" align="right" width="120" />

Welcome to the Nanocode organization.

Nanocode is an SDK for frontier embedded agents, written in Rust. One core runs the same agent,
with the same prompts, durability and Hands, in a terminal, a Cloudflare Worker, a browser tab, a
Vercel Function, a Mac app or an iPhone.

You can install Nanocode on macOS and Linux in seconds via:

```
curl -fsSL https://nanocode.xyz/install | sh
```

Then, in a new terminal run: `nc`.

That's it! If everything goes well, you will now have a coding agent in your terminal, and the same
agent is ready to embed in your own app:

- [nanocode](https://github.com/gakonst/nanocode): the Rust SDK and the `nc` CLI
- [nanocode-ts](https://github.com/gakonst/nanocode-ts): the SDK as one WebAssembly module, for Workers, Vercel, Node and browsers
- [nanocode-swift](https://github.com/gakonst/nanocode-swift): the SDK for macOS and iOS, with AppKit and UIKit views

See the [Nanocode Docs](https://nanocode.xyz) for more.

Nanocode development is spearheaded by [Georgios Konstantopoulos](https://github.com/gakonst) and the open-source community.
