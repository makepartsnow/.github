<p align="center">
  <a href="https://makepartsnow.com"><img src="https://makepartsnow.com/brand-logo.png" alt="Make Parts Now: online 3D printing and CNC machining service" width="420"></a>
</p>

<h1 align="center">Instant 3D printing and CNC machining quotes</h1>

<p align="center">
  <b>Make Parts Now</b> (<a href="https://makepartsnow.com">MakePartsNow.com</a>) is a US online manufacturing service for custom parts and prototypes.<br>
  Upload a CAD file and get an instant quote with real ship dates: SLS and FDM 3D printing, and CNC-machined aluminum and brass, made in our Las Vegas, Nevada shop.<br>
  Order on the website, from AI assistants like Claude, ChatGPT, Cursor and Gemini CLI, or through our API.
</p>

<p align="center">
  <a href="https://makepartsnow.com"><b>Get an instant quote</b></a> ·
  <a href="https://makepartsnow.com/materials">Materials</a> ·
  <a href="https://makepartsnow.com/developers">Developers &amp; AI agents</a> ·
  <a href="https://makepartsnow.com/contact">Contact</a>
</p>

## What we make

| Process | Materials | Finishes and services |
|---|---|---|
| **SLS 3D printing** | PA12 nylon, TPU 90A | Bead blasted, black dye, vibratory smoothing; heat-set threaded inserts |
| **FDM 3D printing** | PLA, PETG, ABS, ASA, TPU 95A, carbon-fiber nylon (PA-CF), PETG-CF | As printed; heat-set threaded inserts |
| **CNC machining** | 6061-T6511 aluminum, C360 brass | As machined, bead blast, deburr, powder coat; tapped holes |

- **CAD files:** STEP, STL, 3MF and OBJ, up to 95 MB. CNC machining needs a STEP file.
- **Lead times:** five production speeds, from Economy to Fastest. Every quote shows the date we'll ship and when the parts should arrive, from our live production schedule.
- **Shipping:** within the United States, free ground shipping on orders of $50 or more.

## How to order custom parts online

1. **Upload your CAD file** at [makepartsnow.com](https://makepartsnow.com). We check its size, volume and wall thickness, and that it fits our machines.
2. **Configure it:** process, material, color, finish, and services like heat-set inserts or tapped holes. The 3D preview shows the finish on your part.
3. **See your price and ship date** for every production speed.
4. **Order:** pay by card through Stripe, or download a PDF quote for your purchasing team. No account needed.
5. **We make it:** your parts are printed or machined, finished, inspected and shipped, with an email at each step and tracking when they ship.

## Get quotes from AI assistants

Ask for a quote in the chat, then review the order and pay on makepartsnow.com. Nothing is charged in the chat, and quotes don't need an account. Try "Quote 25 of this bracket in black nylon."

| AI assistant | How to connect |
|---|---|
| **Claude** | Add a custom connector with `https://makepartsnow.com/mcp/assistant`. Claude shows a Make Parts Now upload box and quote card in the chat. Claude Code: `/plugin install make-parts-now --marketplace makepartsnow/makepartsnow-claude` ([plugin](https://github.com/makepartsnow/makepartsnow-claude), in review for the Claude directory) |
| **ChatGPT** | Add a custom connector with `https://makepartsnow.com/mcp/assistant` |
| **Cursor** | Install the [Make Parts Now plugin](https://cursor.directory/plugins/make-parts-now-3d-printing-cnc-machining-quotes) from Cursor Directory ([plugin](https://github.com/makepartsnow/makepartsnow-cursor)). Cursor's agent quotes the CAD files in your project and uploads them itself |
| **Gemini CLI** | `gemini extensions install https://github.com/makepartsnow/makepartsnow-gemini` ([extension](https://github.com/makepartsnow/makepartsnow-gemini)), then `/make-parts-now:quote ./bracket.step 25` |
| **OpenClaw** | Install the [Make Parts Now plugin](https://clawhub.ai/makepartsnow/plugins/make-parts-now) from ClawHub: `openclaw plugins install clawhub:@makepartsnow/make-parts-now` ([plugin](https://github.com/makepartsnow/makepartsnow-openclaw)) |
| **Hermes Agent** | Install the [Make Parts Now plugin](https://hermes-agent.nousresearch.com/docs/plugins/make-parts-now) from the Hermes plugin catalog: `hermes plugins install make-parts-now`, then `hermes plugins enable make-parts-now` ([plugin](https://github.com/makepartsnow/makepartsnow-hermes)) |

## Manufacturing API and MCP server for developers

- **MCP server** for coding agents and MCP clients (Claude Code, Cursor, VS Code): `https://makepartsnow.com/mcp`. Sign in with your website account or use an agent account key. Listed in the [official MCP Registry](https://registry.modelcontextprotocol.io/v0/servers/com.makepartsnow%2Fmanufacturing/versions/latest) as `com.makepartsnow/manufacturing` and on [Smithery](https://smithery.ai/servers/nathan-egs1/MakePartsNow).
- **REST API** at `https://makepartsnow.com/api/agent/v1`: upload CAD files, get quotes and place orders from your own code, with webhooks for order updates. Pay with a Stripe Checkout link, or let an agent pay in USDC on Base with [x402](https://x402.org).
- **Agent skill** for coding agents (Claude Code, Codex, Cursor, Gemini CLI and more): `npx skills add makepartsnow/skills` teaches the agent to export CAD, quote it, compare quantities and open checkout through the REST API ([skills](https://github.com/makepartsnow/skills)).
- **CAD add-ins:** quote the parts you select and open checkout on makepartsnow.com, with no account. Autodesk Fusion: the [Fusion add-in](https://makepartsnow.com/fusion) ([download](https://github.com/makepartsnow/makepartsnow-fusion/releases/latest)). FreeCAD 1.0+ (beta): the [FreeCAD workbench](https://github.com/makepartsnow/makepartsnow-freecad), installed from Addon Manager as a custom repository or with git ([install](https://github.com/makepartsnow/makepartsnow-freecad#install)). Make Parts Now is not affiliated with the FreeCAD project.
- **Command line:** `pip install makepartsnow`, then `mpn quote bracket.step:10 --zip 89101` prices STEP and STL files from a terminal, a script or CI, with `--json` output and a link to order on makepartsnow.com. No account or key; Python 3.11+ ([makepartsnow-cli](https://github.com/makepartsnow/makepartsnow-cli), [PyPI](https://pypi.org/project/makepartsnow/)).
- **Docs:** [developer guide](https://makepartsnow.com/developers), [interactive API docs](https://makepartsnow.com/api/agent/v1/docs), [OpenAPI spec](https://makepartsnow.com/api/agent/v1/openapi.json), [llms.txt](https://makepartsnow.com/llms.txt).

## Open-source plugins

| Repository | What it is |
|---|---|
| [skills](https://github.com/makepartsnow/skills) | Agent skill for any coding agent: `npx skills add makepartsnow/skills` |
| [makepartsnow-claude](https://github.com/makepartsnow/makepartsnow-claude) | Claude plugin: 3D printing and CNC machining quotes in Claude chat, Cowork and Claude Code |
| [makepartsnow-cli](https://github.com/makepartsnow/makepartsnow-cli) | Command-line tool `mpn`: instant 3D printing quotes for STEP and STL files, `pip install makepartsnow` |
| [makepartsnow-cursor](https://github.com/makepartsnow/makepartsnow-cursor) | Cursor plugin, on [Cursor Directory](https://cursor.directory/plugins/make-parts-now-3d-printing-cnc-machining-quotes) |
| [makepartsnow-freecad](https://github.com/makepartsnow/makepartsnow-freecad) | FreeCAD workbench (beta): instant 3D printing quotes for the selected bodies |
| [makepartsnow-fusion](https://github.com/makepartsnow/makepartsnow-fusion) | Autodesk Fusion (Fusion 360) add-in: instant 3D printing quotes for the parts you click; downloads and docs |
| [makepartsnow-gemini](https://github.com/makepartsnow/makepartsnow-gemini) | Gemini CLI extension |
| [makepartsnow-grok](https://github.com/makepartsnow/makepartsnow-grok) | Grok Build plugin, in review for the xAI marketplace |
| [makepartsnow-hermes](https://github.com/makepartsnow/makepartsnow-hermes) | Hermes Agent plugin, in the [Hermes plugin catalog](https://hermes-agent.nousresearch.com/docs/plugins/make-parts-now) |
| [makepartsnow-openclaw](https://github.com/makepartsnow/makepartsnow-openclaw) | OpenClaw plugin, on [ClawHub](https://clawhub.ai/makepartsnow/plugins/make-parts-now) |

## FAQ

**How fast can I get 3D printed or CNC machined parts?** Every quote lists each production speed with the date we'll ship and the expected arrival, before you order.

**Do I need an account to get a quote?** No. Upload a CAD file and see prices right away, on the website or in an AI assistant.

**Where do you ship?** Within the United States, with free ground shipping on orders of $50 or more.

**Is my CAD file kept private?** Files are stored encrypted and used only to quote and make your parts. Files you never order are deleted; see the [privacy policy](https://makepartsnow.com/legal/privacy). Don't upload files subject to ITAR, EAR or CUI rules.

**What won't you make?** Firearms or their parts, other weapons, and other restricted products.

## Contact

Questions about an order or a part: [makepartsnow.com/contact](https://makepartsnow.com/contact) or orders@makepartsnow.com.
