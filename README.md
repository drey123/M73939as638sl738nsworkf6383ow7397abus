# M73939as638sl738nsworkf6383ow7397abus

Public GitHub Actions workspace for **MassLens**.

Private repo `drey123/Masslens` is the product and the permanent agent memory (append-only WORKLOG.md). Chat is temporary.

This public repo exists only for workflows that cannot run on the private repo because of GitHub Actions limits (minutes, concurrency, self-hosted, matrix size, or secret exposure rules). Agents with their own VMs still prefer the VM; they outsource here when the VM is not enough, then monitor the run and write the outcome back into the private WORKLOG.

## Rules

- No product source of truth lives here. GOAL.md and AGENTS.md stay private.
- Workflows are self-contained and disposable. Prefer ephemeral runners.
- After a run finishes, the agent that launched it appends a dated block to `Masslens/WORKLOG.md` with the run URL, exit status, and any artifacts worth keeping.
- Commit messages: imperative, present-tense, short.

## Grammar for pushes

- "Add workflow X for Y"
- "Wire matrix for Z"
- "Record Actions handoff for container-mass experiment"

No fluff.
