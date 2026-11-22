# Documentation project instructions

## About this project

- Documentation site for Emet Labs' products:
  - [Sentinel](https://github.com/emet-labs/sentinel), a trace-verification platform.
  - [trace-grab](https://github.com/emet-labs/trace-grab), a local CLI for sanitizing trace exports.
- Built on [Mintlify](https://mintlify.com).
- Navigation is organized as one tab per product (`docs.json`); pages live under `sentinel/` and `trace-grab/`.
- Pages are MDX files with YAML frontmatter.
- Configuration lives in `docs.json`.
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP.
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP.

## Terminology

- Sentinel pages use the terms of `CONTEXT.md` in the Sentinel repository (the glossary): Specification, Verdict, Event, Trace, Pattern, Evidence Coverage, Watermark, Source Tier, Data Class. Do not use "rule", "policy", or "result" for these concepts.
- trace-grab pages keep the names that the tool uses: `policy`, `report.md`, `corpus`, `record`, `span`, `disposition`. These are technical names. Do not rename them.
- Use one word for one meaning: "tokenize" (not "mask" or "redact"), "bundle" (the output directory), "grab" (the command), "pass unchanged" (a field that trace-grab does not change).
- Writing standards: ASD-STE100 Simplified Technical English (procedure sentences of at most 20 words, other sentences of at most 25 words, active voice, no semicolons, no contractions) and the Diataxis framework (each page is one of tutorial, how-to guide, reference, or explanation).

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- Prose (overviews, guides, anything narrative) follows the `anti-ai-slop-writing` skill:
  no banned vocabulary, no rule-of-three padding, varied sentence length, no fabricated
  numbers or quotes. Reference material (tables, CLI flags, schema fields) follows ordinary
  technical-writing convention — see that skill's note on applying it to reference docs.
- For substantial writing or editing passes, use the `technical-writer` subagent
  (`.claude/agents/technical-writer.md`).

## Content boundaries

- Sentinel is pre-launch: don't document internals, architecture, component names, or ADR
  content. Sentinel pages are placeholders (product-facing section names, "Coming soon" body)
  until the product ships.
- trace-grab is not framed as a commercial product. Its docs should read as an invitation to
  donate trace data to Emet Labs' research, sanitized and auditable before you send anything —
  not as a sales pitch or a general-purpose tool.
