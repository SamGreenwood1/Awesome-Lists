---
name: List Submission
about: Submit a new Awesome List for review.
title: ''
labels: ''
assignees: ''

---

title: "[LIST SUBMISSION]: "
labels: [list-submission, awaiting-review]
assignees:
  - your-github-username # Replace with a maintainer's username

body:
  - type: markdown
    attributes:
      label: Before You Submit
      description: |
        Please make sure you have read and followed our [Contribution Guidelines](link to contribution guidelines).  Specifically, ensure your list meets the quality criteria outlined in the guidelines.

  - type: input
    id: list-name
    attributes:
      label: List Name
      description: The name of your awesome list (e.g., Awesome Python)
      placeholder: Awesome [Topic]
    validations:
      required: true
  - type: input
    id: list-url
    attributes:
      label: List URL
      description: The URL to your list's README.md file in this repository.
      placeholder: lists/awesome-topic/README.md
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
        - label: The list is focused on a specific topic.
          required: true
        - label: The resources in the list are high-quality and actively maintained.
          required: true
        - label: The list is well-organized and easy to navigate.
          required: true
        - label: The list is free of bias or promotional content.
          required: true

  - type: textarea
    id: additional-context
    attributes:
      label: Additional Context
      description: Add any additional context or information about your list here.
