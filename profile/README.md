<p align="center">
  <img src="./logo.png" alt="nanocode" width="100%" />
</p>

Nanocode is the SDK for embedded frontier agents.

- One SDK, every language. Codex and Claude in Rust, and the same code in TypeScript, Swift, Python, and C.
- Durable. Every model call and tool call is journaled to SQL, so a turn finishes after its process dies.
- Code Mode. The model writes one program that calls every tool, and only its result enters the context.
- Hands. No sandbox per session. A turn reaches a laptop, a server, or a browser tab only for the calls that need one.
- Any payer. A ChatGPT or Claude subscription, an API key, or Machine Payments from a Tempo Wallet.
- Embedded. The agent on this page runs in this tab, with these docs as its files.

You can install Nanocode on macOS and Linux in seconds via:

```
curl -L https://nanocodex.paradigm.xyz | bash
```

Try the live demos:

- [nanocode.xyz/cloudflare](https://nanocode.xyz/cloudflare): durable agents in Cloudflare Durable Objects ([source](https://github.com/nanocodexyz/durable-cloudflare))
- [nanocode.xyz/vercel](https://nanocode.xyz/vercel): durable agents on Vercel Workflows, with [ChatGPT-style](https://nanocode.xyz/vercel/chatgpt) and [Claude-style](https://nanocode.xyz/vercel/claude) clones ([source](https://github.com/nanocodexyz/durable-vercel))

Check the [Nanocode Experiments](https://nanocode.xyz/experiments).

See the [Nanocode Docs](https://nanocode.xyz) for more.

Nanocode development is spearheaded by [Paradigm](https://github.com/paradigmxyz) and the open-source community.
