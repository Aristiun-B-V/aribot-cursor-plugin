---
name: aribot-security-posture
description: Answer questions about the user's security and compliance posture using the Aribot MCP tools (threat models, cloud compliance, code and shadow-AI findings), and use Aribot's governed actions only with the user's confirmation.
---

# Aribot security posture

Use the `aribot` MCP server for questions about the user's own Aribot workspace.

- Compliance by framework: `compliance_status`, `get_framework_coverage`; cloud posture and failing controls: `get_cloud_compliance`.
- Threat models: `list_diagrams`, then `get_diagram_summary` or `get_insights` for one diagram.
- Code and supply chain: `get_code_findings`, `code_review_scan`, `verify_threats_in_code`; shadow AI: `get_shadow_ai`.
- Tools that change the workspace (`apply_remediation`, `file_threat_tickets`, `assign_threat`, `comment_threat_on_change`, scans, `generate_architecture`) act on real data — describe what will happen and get the user's confirmation first.
- Report figures exactly as returned. If a tool returns nothing, say so; never estimate.
