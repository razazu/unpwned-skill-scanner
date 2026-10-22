# Primary references

[Home](../README.md) · [Checklist](checklist.md)

These sources explain the underlying format, runtime behavior, and instruction-trust problem. The exercises in this repository are original synthetic examples, not copied incidents from these sources.

Reviewed for this edition on October 22, 2026. Follow the current documentation for your actual client and version.

| Source | Useful for |
| --- | --- |
| [Agent Skills specification](https://agentskills.io/specification) | Skill structure, supporting files, and the experimental nature of `allowed-tools`. |
| [Claude Code: Extend Claude with skills](https://code.claude.com/docs/en/skills) | Client-specific invocation, supporting files, dynamic context, and tool-permission behavior. |
| [Anthropic: Agent Skills security considerations](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview#security-considerations) | Reviewing the skill package, external sources, and dependencies before use. |
| [OWASP: LLM Prompt Injection Prevention Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/LLM_Prompt_Injection_Prevention_Cheat_Sheet.html) | Why untrusted content can influence an agent and why controls need more than instruction wording. |
| [OWASP: MCP Security Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/MCP_Security_Cheat_Sheet.html) | Trust boundaries around tool-returned content and downstream actions. |
| [GitHub: Saving repositories with stars](https://docs.github.com/en/get-started/exploring-projects-on-github/saving-repositories-with-stars) | Stars as a discovery and appreciation feature, not a security attestation. |

These organizations do not endorse UNPWNED by being referenced here. A general recommendation must still be checked against the behavior of the tools you actually use.
