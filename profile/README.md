<p align="center">
  <a href="https://makepartsnow.com"><img src="https://makepartsnow.com/brand-logo.png" alt="Make Parts Now" width="420"></a>
</p>

<p align="center">
  Custom parts made in our Las Vegas shop: SLS nylon and FDM 3D printing, and CNC-machined aluminum and brass.<br>
  Instant quotes with real ship dates, on the website or from your AI agent or code.
</p>

<p align="center">
  <a href="https://makepartsnow.com"><b>Get an instant quote</b></a> ·
  <a href="https://makepartsnow.com/developers">Developers & AI agents</a> ·
  <a href="https://makepartsnow.com/materials">Materials</a> ·
  <a href="https://makepartsnow.com/contact">Contact</a>
</p>

## Order on the website

1. **Upload your CAD file** (STEP, STL, 3MF or OBJ, up to 95 MB) at [makepartsnow.com](https://makepartsnow.com). We check its size, volume and walls and that it fits our machines.
2. **Configure it.** Choose the process, material, color, finishes and services like heat-set inserts or tapped holes. The 3D preview shows the finish on your part.
3. **See your price and dates.** Every production speed shows the date we'll ship and when it should arrive, from our live schedule.
4. **Order.** Pay by card through Stripe, or download a PDF quote for your purchasing team. You don't need an account.
5. **We make it.** Your parts are printed or machined, finished, inspected and shipped, with an email at each step and tracking when they ship.

We ship within the United States. CNC parts need a STEP file.

## Use it from an AI assistant

Quote in the chat, then review the order and pay on makepartsnow.com. Nothing is charged in the chat, and quotes don't need an account.

| App | How to connect |
|---|---|
| Claude, ChatGPT | Add a custom connector with `https://makepartsnow.com/mcp/assistant` |
| OpenClaw | `openclaw plugins install clawhub:@makepartsnow/make-parts-now` ([plugin source](https://github.com/makepartsnow/makepartsnow-openclaw)) |
| Hermes Agent | Add `https://makepartsnow.com/mcp/assistant?client=hermes` as an MCP server ([setup](https://makepartsnow.com/developers#ai-assistants)) |

Then ask something like "Quote 25 of this bracket in black nylon."

## Build with it

- **MCP server** for coding agents and MCP clients (Claude Code, Cursor, VS Code): `https://makepartsnow.com/mcp`. You sign in with your website account or use an agent account key. It's listed in the [official MCP Registry](https://registry.modelcontextprotocol.io/v0/servers/com.makepartsnow%2Fmanufacturing/versions/latest) as `com.makepartsnow/manufacturing` and on [Smithery](https://smithery.ai/servers/nathan-egs1/MakePartsNow).
- **REST API** at `https://makepartsnow.com/api/agent/v1`: upload, quote and order from your own code, with webhooks for order updates. Pay with a Stripe Checkout link, or let the agent pay in USDC on Base with [x402](https://x402.org).
- **Docs:** [developer guide](https://makepartsnow.com/developers), [interactive API docs](https://makepartsnow.com/api/agent/v1/docs), [OpenAPI spec](https://makepartsnow.com/api/agent/v1/openapi.json), [llms.txt](https://makepartsnow.com/llms.txt).

## Contact

Questions about an order or a part: [makepartsnow.com/contact](https://makepartsnow.com/contact) or orders@makepartsnow.com.
