# Parameters

- {{AUTHOR_ROLE}}: PRODUCT OWNER
- {{COMPANY_DOMAIN}}: AVIATION
- {{COMPANY_DESCRIPTION}}: an aviation company that writes software for pilots
- {{DOCUMENT_TYPE}}: short requirements document
- {{FEATURE_NAME}}: todo list
- {{OUTPUT_FILE}}: output.md

- {{TARGET_IMPLEMENTER_ROLE}}: SENIOR BACKEND C++ ENGINEER
- {{TARGET_AUDIENCE}}: senior backend C++ engineer
- {{SECURITY_EMPHASIS_LEVEL}}: HIGH
- {{PRIORITY_FOCUS_AREAS}}: security

- {{OUTPUT_FORMAT}}: Markdown
- {{SECTION_ORDER}}:
  - Assumptions
  - Overview
  - Functional Requirements
  - Non-Functional Requirements
  - Open Questions

- {{REQUIREMENT_ID_PREFIX}}: TODO
- {{REQUIREMENT_ID_START}}: 1

- {{WRITING_STYLE_RULES}}:
  - Requirements must be testable and measurable; avoid vague terms (e.g., “easy”, “fast”) without thresholds.
  - Do not include implementation code or specific libraries; focus on what must be true.

- {{HIDDEN_REASONING_INSTRUCTIONS}}:
  - Before producing the final output, reason step-by-step about security, safety, and misuse scenarios. Do not include that reasoning in the output.
  - For each requirement, consider multiple wording options, rank each on a scale of 1-5 for expressiveness, and choose the best. Do not include this analysis in the output.

---

You are a {{AUTHOR_ROLE}} at {{COMPANY_DESCRIPTION}} ({{COMPANY_DOMAIN}}). Generate a {{DOCUMENT_TYPE}} for a {{FEATURE_NAME}} in `{{OUTPUT_FILE}}` that will be implemented by a {{TARGET_IMPLEMENTER_ROLE}}. Emphasize {{PRIORITY_FOCUS_AREAS}} ({{SECURITY_EMPHASIS_LEVEL}}).

---

The document must be output in {{OUTPUT_FORMAT}} and use the following structure (in this order):

{{SECTION_ORDER}}

Each requirement must be given an ID in the format `{{REQUIREMENT_ID_PREFIX}}-N` starting at `{{REQUIREMENT_ID_PREFIX}}-{{REQUIREMENT_ID_START}}` (e.g., `{{REQUIREMENT_ID_PREFIX}}-1`, `{{REQUIREMENT_ID_PREFIX}}-2`, ...).

Additional rules (must be followed):
{{WRITING_STYLE_RULES}}

Internal process (must be done, but not shown in the output):
{{HIDDEN_REASONING_INSTRUCTIONS}}
