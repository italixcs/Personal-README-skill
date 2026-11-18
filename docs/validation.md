# Validation

## Package and security

| Check | Result |
| --- | --- |
| Agent Skills structure | Passed the existing skill creator validator. All three bundled reference links and the package license resolve. |
| Installation files | Byte-identical local copies created in isolated Codex and Claude Code directory layouts. Native host discovery and ChatGPT upload remain documentation-checked. |
| Static security | NVIDIA SkillSpector 2.12.0, source revision `a09091e0ebf6c96ff327457529d7b0d372125884`, ran on 18 November 2026. Five of five installable files were inspected. Zero issues, zero suppressions, and no excluded files. |
| Security scope | The scan used `--no-llm --fail-on-incomplete`. It reported complete coverage with a nonfatal reference-resolution caveat for the `README.md` the skill creates at runtime. The three bundled references resolve. The installable package has no scripts, dependency manifests, hooks or credential requirements. |
| Example preview | The terminal-style Italixcs draft and this repository’s README rendered locally at 390 and 1024 px in light and dark. The check covered banner crops, button and icon sizing, links, and public repository destinations. The profile placement check applies after merge. |

The [hash manifest](candidate.sha256) identifies the exact reviewed installable package. The repository documentation and example image sit outside that package. Static findings apply to this scope and are one part of review.

## Paired diagnostic

The evaluated pre-refinement package had manifest digest `200b7ae2aed88f703cde18fb172c7b2b6f5a964b6cf29097485907294d70e111`. Two fresh workers per case received the same public snapshots and prompt, with explicit skill loading in one run per case. An independent reviewer scored anonymously labeled drafts against five frozen criteria. The files were accessible through a shared filesystem, so the isolation was best effort. Model and reasoning were inherited equally. Native discovery, tokens, and precise comparative elapsed times were unmeasured.

| Scenario | Guided | Baseline | Blind verdict |
| --- | --- | --- | --- |
| Create an open-source tool profile from a public snapshot | 10/10 | 9/10 | Guided draft. More legible visual details on mobile and a more compact introduction. |
| Redesign the Italixcs profile using the public source and assets | 10/10 | 10/10 | Tie. The guided draft made install links more prominent and reduced image weight. The baseline kept the project actions and supporting example together and used less vertical space. |

Both drafts passed the critical checks in each case. A linked attachment was initially missed in the redesign review packet. It was restored and the same reviewer regraded the affected criterion under the original blind labels, changing the redesign verdict to a tie.

The release candidate adds first-screen and project-action-to-evidence checks and guidance for buttons, icons, and public statistics. The paired scores refer to the earlier package. Results from two offline scenarios describe those runs, with other audiences and native skill discovery still open.

A fresh guided check of the refined package used a fictional profile with a tall existing wordmark. It preserved the artwork, put the install and example links adjacent and above it, and kept the name and purpose visible on mobile. The draft rendered in both themes at 390 and 1024 px with no measured overflow. This was a targeted follow-up with one guided run.
