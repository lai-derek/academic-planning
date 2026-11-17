# Academic Planning

Plan UCLA undergraduate courses and build ranked section schedules with your AI
agent (Claude Code or Codex). Your degree requirements, awarded credit, goals
and course decisions stay in your private student workspace. The tool checks
them and generates an Excel planner, an advising PDF and a readable academic
record. It never enrolls you or changes MyUCLA on its own.

## Install

Academic Planning installs with [Student Workspace](https://github.com/lai-derek/student-workspace).
You need Windows, Python 3.14 or newer (setup can install it), and an AI agent
with file, command and web access.

1. Download [Student-Tools-Setup.zip](https://github.com/lai-derek/student-workspace/releases/latest/download/Student-Tools-Setup.zip), extract it and run `Install.cmd`.
2. Choose Academic Planning in the wizard.

To update, download the latest setup ZIP and run it on the same workspace.

## Use

Open your workspace in your AI agent. To start, give it your degree audit (DARS)
and ask it to set up your academic records. It follows
`knowledge/academics/INTAKE.md`: it saves the original audit, shows you what it
read and what's unclear, and adds the records only after you've reviewed them.
After that, ask things like "plan winter" or "build me a schedule".

The generated files are in `artifacts/academic-planning/`:
`Academic-Planner.xlsx`, `Academic-Advising.pdf` and `Current-Academic-Record.md`
(plus `Abroad-Brief.pdf` if you plan study abroad).

To see a finished example first, open [examples/](examples/), or build a
synthetic one from PowerShell in your workspace folder:

```powershell
.\tools\.venv\Scripts\academic-planning.exe --workspace "$env:TEMP\academic-demo" demo
```

More: [record formats](docs/records.md) (mostly for your agent),
[how it fits the workspace](docs/integration.md), [validation](VALIDATION.md).

## License

MIT; see [LICENSE](LICENSE) and [NOTICE.md](NOTICE.md).
