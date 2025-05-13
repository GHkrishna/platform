name: "\U0001F680 Feature Request"
description: Suggest an idea or enhancement for this project
labels: [enhancement, needs-triage]
body:
  - type: checkboxes
    id: preliminary-checks
    attributes:
      label: "✅ Preliminary Checks"
      description: "Please confirm the following before submitting."
      options:
        - label: "I have searched [existing issues](https://github.com/credebl/platform/issues) and [pull requests](https://github.com/credebl/platform/pulls) to avoid duplicates."
          required: true
        - label: "I'm willing to create a PR for this feature (if applicable)."
          required: false

  - type: textarea
    id: problem-statement
    attributes:
      label: "🧩 Problem Statement"
      description: "Is your feature request related to a problem? Please describe it clearly."
      placeholder: "Ex: I'm always frustrated when [...]"
    validations:
      required: true

  - type: textarea
    id: proposed-solution
    attributes:
      label: "💡 Proposed Solution"
      description: "A clear and concise description of what you want to happen."
      placeholder: "Ex: It would be great if [...]"
    validations:
      required: true

  - type: textarea
    id: alternatives-considered
    attributes:
      label: "🔄 Alternatives Considered"
      description: "Have you considered any alternative solutions or features?"
      placeholder: "Ex: I also thought about [...], but [...]"
    validations:
      required: false

  - type: textarea
    id: additional-context
    attributes:
      label: "📎 Additional Context"
      description: "Add any other context, references, mockups, or screenshots here."
    validations:
      required: false

  - type: textarea
    id: acceptance-criteria
    attributes:
      label: "✅ Acceptance Criteria"
      description: "List specific tasks or outcomes that define when this request is complete."
      placeholder: |
        - A new endpoint `/v1/...` is added
        - Docs updated
        - Tests written and passing
    validations:
      required: false
