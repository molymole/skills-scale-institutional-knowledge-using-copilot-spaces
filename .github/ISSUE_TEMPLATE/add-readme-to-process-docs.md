---
name: "Add README for Project Management Process Docs"
description: "Propose and track the addition of a README with process summary and doc links."
title: "[Process Doc Update]: README, project management processes summary, and links for OctoAcme Project Management Docs"
labels: ["documentation", "process improvement"]
body:
  - type: dropdown
    id: process_doc
    attributes:
      label: "Which process document do you want to update? (If this is a new document, select '<new document>')"
      options:
        - "<new document>"
    validations:
      required: true

  - type: textarea
    id: content_summary
    attributes:
      label: "Summary of New Content"
      description: "Briefly describe the new README: should provide a process overview and organized links to all docs."
      placeholder: "E.g., README with summary and links to every process doc in docs/"
    validations:
      required: true

  - type: textarea
    id: rationale
    attributes:
      label: "Why is this update needed?"
      description: "Explain the reason for this addition. Is it to address a gap, improve clarity, etc.?"
      placeholder: "E.g., Helps onboarding, provides one entrypoint for process docs, prevents knowledge silos."
    validations:
      required: true

  - type: textarea
    id: example_content
    attributes:
      label: "Suggested Content (optional)"
      description: "Paste the proposed README markdown with clickable doc links and a brief summary. (Optional)"
      placeholder: "E.g., Example README markdown file."

  - type: checkboxes
    id: acceptance_criteria
    attributes:
      label: "Acceptance Criteria"
      description: "Check all that apply:"
      options:
        - label: "Content aligns with existing process docs"
        - label: "Update improves clarity or closes a documented gap"
        - label: "Proposed content has been reviewed with stakeholders (if needed)"
---
