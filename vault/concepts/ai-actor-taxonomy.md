---
type: concept
name: "AI Actor Taxonomy"
aliases: ["AI Actors", "AI Actor Task Categories"]
description: "The NIST AI RMF's taxonomy of roles ('AI Actors') across the AI lifecycle — design, development, deployment, operation, evaluation, and human/domain factors — plus the external stakeholders affected by or interacting with an AI system."
related_to: ["[[nist-ai-risk-management-framework]]", "[[ai-lifecycle-dimensions]]", "[[human-ai-interaction-risk]]"]
sources:
  - url: "https://www.nist.gov/itl/ai-risk-management-framework"
    type: "remote-binary"
    synced_at: "2026-09-10"
updated_at: "2026-09-10"
updated_by: "preserve@agent"
tags: [type/concept, domain/engineering]
graphify_node_ids: ["nist_ai_100_1_ai_actor", "nist_ai_100_1_ai_design", "nist_ai_100_1_ai_development", "nist_ai_100_1_ai_deployment", "nist_ai_100_1_operation_and_monitoring", "nist_ai_100_1_tevv", "nist_ai_100_1_human_factors", "nist_ai_100_1_domain_expert", "nist_ai_100_1_third_party_entities", "nist_ai_100_1_end_users", "nist_ai_100_1_affected_individuals_communities", "nist_ai_100_1_general_public"]
confidence: "EXTRACTED"
---

<!-- Zettelkasten role: permanent note -->

# AI Actor Taxonomy

> "AI Actor" is the NIST AI RMF's umbrella term (adapted from the OECD's AI actor definition) for anyone who plays an active role in the AI system lifecycle — including organizations and individuals that deploy or operate AI.

## Description

The AI RMF (Appendix A) breaks AI Actors into task categories mapped to the [[ai-lifecycle-dimensions|AI lifecycle]], then names additional actors who are affected by or interact with a system without necessarily building or operating it. Different actor categories carry different responsibilities under the [[ai-rmf-core-functions|GOVERN, MAP, MEASURE, and MANAGE functions]], and their interactions are central to the framework's treatment of [[human-ai-interaction-risk|human-AI interaction risk]].

## Task-Based Actor Categories (Appendix A)

- **AI Design** — defining the system's objectives, requirements, and specifications before development.
- **AI Development** — building, training, and implementing the system to meet its design.
- **AI Deployment** — putting the system into operational use, including integration and rollout.
- **Operation and Monitoring** — running the system day-to-day and tracking its behavior/performance over time.
- **TEVV (Test, Evaluation, Verification, and Validation)** — activities, potentially independent of the design/development/deployment teams, that confirm the system meets requirements and behaves as intended across its lifecycle.
- **Human Factors** — the discipline addressing how humans interact with, are affected by, and provide oversight of the system.
- **Domain Expert** — subject-matter expertise brought in to ensure the system's design and evaluation reflect real-world context correctly.

## Additional Actors

- **Third-Party Entities** — external suppliers, vendors, or partners contributing components, data, or services to the AI system.
- **End Users** — the people or systems that directly operate or consume the AI system's outputs.
- **Affected Individuals/Communities** — people impacted by the system's outputs or decisions without necessarily using it directly.
- **General Public** — the broader societal stakeholder group with an interest in how AI systems are governed, even absent direct interaction.

## Where it Applies

- [[nist-ai-risk-management-framework]] — the actor taxonomy is how the framework assigns responsibility across the lifecycle
- [[ai-lifecycle-dimensions]] — actor task categories map onto lifecycle stages

## Related Concepts

- [[human-ai-interaction-risk]] — actor interactions (especially end users, human factors) are central to this risk dimension
