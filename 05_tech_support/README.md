# 05 Tech Support

This directory contains investigations, diagnostics, and root-cause analyses of production support issues, customer tickets, crash reports, or incident troubleshooting.

- [ ] `<ticket-id>/investigation.md`: A structured writeup of the findings for a particular support issue.

## Naming Conventions
- **Flexible Identifiers**: The `<ticket-id>` folder name should match the external identifier associated with the support issue (e.g., `SUPPORT-123`, `GH-456`, or raw numbers like `1092`). No specific format or prefix/suffix is strictly enforced.

## Structure & Asset Inclusion
- Each investigation should reside in its own folder: `05_tech_support/<ticket-id>/`.
- **`investigation.md`**: Every ticket folder must contain an `investigation.md` file based on the template at `templates/investigation_template.md`.
- **Supporting Assets**: You are encouraged to place arbitrary supporting assets directly in the ticket folder alongside `investigation.md` (e.g., `.log`, `.json`, `.png` files, stack traces, or payloads) to keep diagnostic evidence organized and easily accessible to both humans and AI agents.

*Agent Instruction*: Before investigating an active support ticket or incident, check if a folder already exists under this directory for the relevant ticket identifier. Use `templates/investigation_template.md` to document your findings, diagnostic steps, root cause, and resolution.
