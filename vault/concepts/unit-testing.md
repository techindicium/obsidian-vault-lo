---
type: concept
name: "Unit Testing"
aliases: ["Unit Tests"]
description: "Developer-written automated tests that cover individual pieces of code, forming the wide base of the software testing pyramid."
related_to: ["[[shift-left-testing]]", "[[software-testing-pyramid]]", "[[static-code-analysis]]"]
sources:
  - url: "https://www.stickyminds.com/article/shift-left-approach-software-testing"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["shift_left_approach_software_testing_unit_testing"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# Unit Testing

> Automated tests, written by developers, that cover the code reasonably well at the smallest scale — the base layer of the software testing pyramid.

## Description

Unit tests are a core part of a mature [[shift-left-testing|shift-left testing]] practice: because they run at the developer desktop without external dependencies, they can be executed continuously, giving fast feedback as code changes land. In the [[software-testing-pyramid|software testing pyramid]] model, unit tests form the large base, with functional/API tests above them and manual/UI tests as only a thin top layer meant to confirm — not discover — functionality.

## Key Characteristics

- Owned and written by developers, covering individual units of code in isolation.
- Cheap and fast to run continuously, unlike later-stage functional tests with external dependencies.
- Complements [[static-code-analysis|static code analysis]] as one of the two foundational, developer-owned quality practices.

## Where it Applies

- [[software-testing-pyramid]] — unit tests form its base layer
- [[shift-left-testing]] — unit testing is a prerequisite practice for shifting left

## Related Concepts

- [[static-code-analysis]] — the other foundational developer-owned practice
- [[software-testing-pyramid]] — the model that positions unit tests as the base layer
