# Validation

Version 0.3.0, checked 2026-11-16 on native Windows 11 with Python 3.15.2:

- `python -m unittest discover -s tests`: 89 tests passed.
- Registered in a fresh Student Workspace: setup created the records, the skill
  pointers and the WORKSPACE.md section; `student-workspace check` reported
  current, then stale after a goals change.
- The synthetic example in `examples/workspace/` was regenerated with `demo`.

Not verified yet: other operating systems, GitHub CI, and live MyUCLA operation
(tests never use a real browser session).
