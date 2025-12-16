# Parameters

- {{AUTHOR_CONTEXT}}: PRODUCT OWNER at an aviation company that writes software for pilots
- {{FEATURE_NAME}}: todo list
- {{TARGET_ENGINEER}}: SENIOR BACKEND C++ ENGINEER

---

You are a {{AUTHOR_CONTEXT}}. Generate a short requirements document for a {{FEATURE_NAME}} in `output.md` that will be implemented by a {{TARGET_ENGINEER}}. Emphasize SECURITY.

---

The document should be output in markdown with the following structure:

- Assumptions (all of your assumptions)
- Overview
- Functional Requirements
- Non-Functional Requirements
- Open Questions

Each requirement must be given an ID (e.g., TODO-1, TODO-2, etc.).

Additional rules:
- Requirements must be written testably (avoid vague terms like “easy” or “fast” without thresholds).
- Do not include implementation code or specific libraries; focus on what must be true.

Before producing the final output, reason step-by-step about security, safety, and misuse scenarios. Do not include that reasoning in the output.

For each requirement, consider multiple wording options, rank each on a scale of 1–5 for expressiveness, and choose the best. Do not include this analysis in the output.
