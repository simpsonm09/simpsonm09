# Exceptions

Rules from [`standards/core.md`](https://github.com/simpsonm09/.github/blob/main/standards/core.md)
and [`standards/owner.md`](https://github.com/simpsonm09/.github/blob/main/standards/owner.md) that
this repository cannot meet, with the reason and the date to revisit.

| Rule       | Reason                                                                                                                                                                                                          | Revisit    |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
| C2.2, C5.1 | The owner standard keeps the profile repository a page with no CI and no required checks (O5), and Actions is disabled on the repository, so there is no median to report. The pull request itself is the gate. | 2027-02-23 |
| C7.5       | `lint`, `typecheck`, `test` and `hooks` have nothing to run: there is no code, no dependency manifest and no workflow. `install`, `fmt`, `fmt-check`, `agent-files` and `check` exist.                          | 2027-02-23 |
