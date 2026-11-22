# GMRI Agent Reach: ChatGPT-native plugin

**Upload this ZIP as one plugin in ChatGPT. No local installation is needed.**

This is the **ChatGPT-native adaptation** of Agent Reach's read-first, channel-based research workflow. It is deliberately **not** the original CLI, a local MCP executable, or a server deployment kit. It works by directing ChatGPT to use its own web research and any research apps already connected to the account. It does not create new MCP tools or unlock external services that ChatGPT could not otherwise access.

## What happens after upload

ChatGPT can invoke the included research skill when you ask it to search the open web, read pages, compare evidence, trace historical archives, research GitHub, find video transcripts, or inspect public social-media material. It chooses an available tool, obtains source evidence, checks an independent source, and reports what it actually verified. Tool availability depends on the ChatGPT plan, surface, permissions, and connected apps.

No MCP server, SSH, tunnel, desktop CLI, Proxmox host, API key, or installation script is needed. The plugin relies on built-in ChatGPT capabilities and already-accessible apps rather than deploying an executable service.

## How to upload

If you have workspace plugin ZIP upload rights, use **ChatGPT web > Admin console > select workspace > Plugins > Add > Upload plugin**. Upload the entire ZIP; do not upload the files one by one. The ZIP contains exactly one root plugin folder and one skill. Installation controls may vary by workspace.

Once installed, mention **@GMRI Agent Reach** (if your ChatGPT client presents that option), or simply ask:

- "Use Agent Reach to research the 1988-1991 Dallas organized-crime record trail and separate primary evidence from hypotheses."
- "Use Agent Reach to find this video's transcript, original sources, dates, and any substantive contradictions."
- "Use Agent Reach to inspect this GitHub repository's actual issues, commits, release history, and code, citing direct links."
- "Agent Reach: trace this named person's aliases through contemporaneous reporting and court indexes. Verify identity before merging any matches."

## Precisely what this is (and is not)

**Included:** 14-channel research route map; tool discovery; fallbacks and alternate-search tactics; full-text retrieval; video and repository routes; handling of blocked sites; provenance/identity/chronology checks; evidence report templates.

**Not included:** the original Python CLI or browser session manager; a new custom MCP tool or remote endpoint; automatic browser logins or session copying; unauthorized CAPTCHA bypass; guarantees that a restricted or paywalled platform can be accessed.

ChatGPT cannot turn locally bundled Python scripts into a cloud-hosted MCP endpoint merely by uploading a ZIP. To expose the original CLI's private platform APIs as independent ChatGPT tools would still require an authorized hosted MCP service. This plugin deliberately avoids that dependency and provides the useful research workflow immediately through available tools.

## Source and licensing

Adapted from the user-provided Agent Reach v1.6.1 and v1.4.0 archives and the Agent Reach instruction archive. The 14 channel names and fallback-first conceptual design come from Panniantong's Agent Reach, MIT licensed: https://github.com/Panniantong/Agent-Reach. This adaptation does not claim to be released or maintained by the upstream project. See `skills/agent-reach-native/references/PROVENANCE.md`.
