Testem Reload Issue
===================

This repo is meant to be a testing ground for live-reloading tests with [Testem](https://github.com/airportyh/testem).

### Problem

It appears that the current version of Testem does not trigger a restart of the test suite upon file-changes.

### Reproduction

1. Clone this repo.
2. Run `npm install`.
3. Run `npm test` (which just starts testem).
4. Open browser to http://localhost:7357/
5. Change `tests/tests.js` (either change the failing test to pass or add a new test).
6. Save change.
7. Tests are not re-run.
