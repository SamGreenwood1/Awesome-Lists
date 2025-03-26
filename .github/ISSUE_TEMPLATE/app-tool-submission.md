---
name: App/Tool Submission
about: App/Tool Submission
title: ''
labels: ''
assignees: ''

---

title: "[APP SUBMISSION]: "
labels: [app-submission, awaiting-review]
assignees:
  - your-github-username  # Replace with a maintainer's username

body:
  - type: markdown
    attributes:
      label: Important Notes Before Submitting
      description: |
        *   Please ensure you've read the [Contribution Guidelines](link to contribution guidelines) to understand our criteria for inclusion.
        *   Submissions should be for tools that are actively maintained and provide genuine value.
        *   Avoid submitting personal projects unless they are exceptionally well-documented and useful to a broad audience.

  - type: input
    id: app-name
    attributes:
      label: Application/Tool Name
      description: The name of the application or tool.
      placeholder: My Awesome Tool
    validations:
      required: true

  - type: input
    id: app-url
    attributes:
      label: Application/Tool URL
      description: The official website or repository URL.
      placeholder: https://example.com/my-awesome-tool
    validations:
      required: true

  - type: dropdown
    id: list-suggestion
    attributes:
      label: Suggested Awesome List
      description: To which Awesome List do you think this tool belongs?  If unsure, select "General".
      options:
        - Programming Languages (Replace with your categories)
        - Web Development
        - Data Science
        - DevOps
        - Security
        - General  # Use as a fallback if the category is unclear.
    validations:
      required: true

  - type: textarea
    id: description
    attributes:
      label: Description
      description: Briefly describe the application/tool and its key features.
      placeholder: A short description of the application and what it does.
    validations:
      required: true

  - type: textarea
    id: justification
    attributes:
      label: Justification
      description: Why do you think this application/tool should be included in the Awesome List?  What problem does it solve or what unique value does it provide?
      placeholder: Explain the benefits of this tool and why it's a good fit.
    validations:
      required: true

  - type: checkboxes
    id: checklist
    attributes:
      label: Submission Checklist
      description: Please confirm the following:
      options:
        - label: I have read and followed the [Contribution Guidelines](link to contribution guidelines).
          required: true
        - label: The application/tool is actively maintained.
          required: true
        - label: The application/tool provides genuine value and is not simply promotional.
          required: true
        - label: The application/tool is well-documented (if applicable).
          required: true

  - type: textarea
    id: additional-context
    attributes:
      label: Additional Context
      description: Add any other context, screenshots, or information that might be helpful.
