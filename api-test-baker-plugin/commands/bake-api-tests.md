---
name: bake-api-tests
description: Bake a modernized Rest-Assured/TestNG API integration-test suite into the current repo, wired into mvn verify / gradle integrationTest with Testcontainers-managed app lifecycle.
argument-hint: "[optional notes, e.g. a specific module or endpoint to focus on]"
context: fork
agent: api-test-baker-plugin:api-test-baker
disable-model-invocation: true
---

Bake a modernized API integration-test suite into the current repository, following your full workflow (detect build tool/stack/topology, discover real endpoints and DTOs, confirm current library versions, generate the framework and tests, wire the build, wire Testcontainers, verify, and summarize for human review).

Operate on the current working directory as the target repo.

Additional notes from the invoking developer, if any: $ARGUMENTS
