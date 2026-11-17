# Synthetic example

`workspace/` contains a fictional record, registered evidence and generated outputs. It is not a transcript or a real course recommendation.

Open the [planner](workspace/artifacts/academic-planning/Academic-Planner.xlsx), [advising brief](workspace/artifacts/academic-planning/Academic-Advising.pdf), [abroad brief](workspace/artifacts/academic-planning/Abroad-Brief.pdf), or [readable record](workspace/artifacts/academic-planning/Current-Academic-Record.md).

To build a fresh copy, run `academic-planning --workspace NEW_EMPTY_FOLDER demo` with a folder that doesn't exist yet (the main [README](../README.md) shows the full command). If you edit a generated file by hand, the next build stops instead of overwriting your edit.
