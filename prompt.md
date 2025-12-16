You are a PRODUCT OWNER at an AVAIATION COMPANY that writes software for PILOTS. Generate a short requirements document for a todo list in `output.json` that will be implemented by a SENIOR BACKEND C++ ENGINEER . Emphasize SECURITY.

---

The document should be output in a JSON format with the following structure:

{
  "document": {
    "title": "To-Do List Application Requirements",
    "version": "1.0",
    "status": "draft",
    "lastUpdated": "2025-01-01"
  },
  "overview": {
    "purpose": "Define the functional and non-functional requirements for a basic To-Do List application.",
    "scope": {
      "inScope": [...],
      "outOfScope": [...]
    },
  },
  "definitions": [
    {
      "term": "Task",
      "definition": "A single unit of work tracked by the application."
    },
    ...
  ],
  "requirements": {
    "functional": [
      {
        "id": "FR-1",
        "title": "Create Task",
        "description": "The system shall allow the user to create a new task.",
        "priority": "high",
        "acceptanceCriteria": [
          "User can enter a task title",
          "Task is added to the task list"
        ]
      },
    ],
    "nonFunctional": [
      {
        "id": "NFR-1",
        "type": "usability",
        "description": "The application shall be intuitive and require no training."
      },
    ]
  },
  "openQuestions": [...]
}

Additional rules:
- Requirements should be written testably (avoid vague terms like “easy” or “fast” without thresholds).
- Do not include implementation code or specific libraries; focus on what must be true.
