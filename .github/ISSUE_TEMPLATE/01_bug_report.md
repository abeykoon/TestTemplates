---
name: 🐞 Bug Report
about: Create a report about something that is not working
labels: 'Type/Bug'
body:
  - type: dropdown
    id: version
    attributes:
      label: Version
      description: What version of our software are you running?
      options:
        - 1.0.2 (Default)
        - 1.0.3 (Edge)
    validations:
      required: true
---

**Description:**
<!-- Give a brief description of the bug -->

**Steps to reproduce:**

**Affected Versions:**

**OS, DB, other environment details and versions:**

**Related Issues (optional):**
<!-- Any related issues such as sub tasks, issues reported in other repositories (e.g component repositories), similar problems, etc. -->

**Suggested Labels (optional):**
<!-- Optional comma separated list of suggested labels. Non committers can’t assign labels to issues, so this will help issue creators who are not a committer to suggest possible labels-->

**Suggested Assignees (optional):**
<!--Optional comma separated list of suggested team members who should attend the issue. Non committers can’t assign issues to assignees, so this will help issue creators who are not a committer to suggest possible assignees-->