# Yamada-UI: Tips for Testing

This document summarizes tips related to testing for Yamada-UI.

## How to Run Tests

**To run all tests**

```bash
pnpm test
```

**To run tests for a single component**

```bash
pnpm test <component_name>

# Example for Modal component
pnpm test modal
```

## How to Check Test Coverage

**Local Environment**

1. Execute `pnpm test:coverage`
2. Access `http://localhost:4173/`

## Frequently Asked Questions

- Should I add tests when making changes?

  - Yes. However, adding tests is not necessary for typo corrections, documentation updates, or code refactoring.

- Is it necessary to add a changeset file for a PR that only adds tests?

  - No, it is not necessary.

- What is Codecov?
  - At Yamada-Ui, we use [Codecov](https://about.codecov.io/) to visualize test coverage after creating a PR. If you receive a warning from Codecov, it may indicate that the changes have not been tested. Therefore, it is necessary to either fix the untested changes or add new tests.
