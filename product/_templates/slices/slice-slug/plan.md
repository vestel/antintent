# Slice Plan: <Slice Title> (`slice-slug`)

- **Spec Reference:** [../../spec.md](../../spec.md)
- **Code Branch:** `feat/<slice-slug>`
- **Status:** `Draft` | `Approved` | `In Progress` | `Validated` | `Completed`
- **Updated:** YYYY-MM-DD

## 1. Slice Goal & Value Increment
<!-- What coherent, end-to-end increment of functionality does this slice deliver? -->

## 2. Under-the-Hood Mechanics
<!-- Plain-English explanation of how the mechanism works internally so the client clearly understands what will happen. -->

## 3. Files to Create or Modify
- `path/to/test_file` — Automated tests for this slice
- `path/to/source_file` — Implementation logic

## 4. Implementation Steps (TDD Order)
1. [ ] **Test Harness:** Write automated tests covering expected behavior and edge cases.
2. [ ] **Core Implementation:** Implement the minimal logic to pass the tests.
3. [ ] **Integration Check:** Run full test suite and verify no regressions.

## 5. Risks & Assumptions
- ...

## 6. Acceptance & Completion Criteria
- [ ] All slice-specific automated tests pass (`<test command>`).
- [ ] Full project test suite passes without regressions.
- [ ] User validation scenario in [validations.md](./validations.md) verified by the client.
