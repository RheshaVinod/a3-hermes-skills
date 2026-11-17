---
name: deadline-risk
description: Assess a synthetic project deadline against estimated remaining work and recommend a focus action.
version: 0.1.0
author: Rhesha Vinod
license: MIT
platforms: [linux, macos]
metadata:
  hermes:
    category: productivity
    tags: [planning, deadlines, risk]
---

# Deadline Risk

Assess a synthetic project deadline and recommend the next focus action.

## Prerequisite

This skill is designed for the CSCI 599 Assignment 3 assistant and requires
the `a3ctl` command supplied by that project.

## Run

```sh
a3ctl deadline-risk "LABEL" "ISO-8601-DEADLINE" REMAINING_WORK_HOURS
```

Use a timezone-aware ISO-8601 deadline. Treat remaining work as a non-negative
estimate in hours.

Report:

- the project label;
- hours remaining until the deadline;
- risk as `low`, `medium`, `high`, or `overdue`; and
- the recommended action.

Use synthetic project names and dates only. Never edit a calendar or send a
message without a separate user request. Never include credentials, personal
data, or private calendar details in the command.
