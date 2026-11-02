![A breakwater in a November gale with no lettering: huge sodden near stones at the lower left with foam draining back, the stone arm reaching to its fixed lit lamp, spray breaking over it, and the harbour sheltering behind with oil lanterns and a lit office window](intro-banner.png)


# codeintel-Build-Process-Integrity-Checker

![The long stone arm in a November gale running lower left to centre, spray carried clean over the top, the lit lamp small at its far end, oil lanterns and tarred barrels in the lee, and codeintel-build-process-integrity-checker painted on the lamp room door in foam white](banner.png)

![A breakwater lamp close up: a square tar black iron housing with a chamfered cap on a stub of teal stone pier, one glass face burning lantern amber, foam white spray bursting at the pier foot, and the name underneath in foam white, the heading plate](logo.png)

![The breakwater in three depths: waves rise, travel, and break in a slow heavy sequence in the far depth while driven cloud moves fast and low, spray breaks over the stones wave by wave in the middle depth and runs back while the lamp does not move at all and brightens only as spray crosses it, and tarred barrels in the near depth drip after each spray fall and stop between falls](scene.svg)

Verifies the integrity of the build process by checking build scripts, dependency files, and compiler settings files against supplied SHA256 baseline hashes, and alerts on mismatches. The build script is the primary artifact: a named build script with no baseline hash exits 1. Any other named file with no baseline hash is logged as skipped, one line per file, and a closing summary counts checked and skipped files. A run that checked zero files exits 1. If a scanner the operator asked for with --run-bandit, --run-flake8, --run-pylint, or --run-pyre is missing or returns non zero, the run ends with a line naming the scanner outcomes and exits 1.

![Major separator: a fine tide table rule in deep sea teal across the full width, with a single spray mark breaking over it at wide intervals](sep-heavy.svg)

## Install
`git clone https://github.com/ShadowStrikeHQ/codeintel-build-process-integrity-checker`

> **Harbour notice: the address names another organisation.** The install line above points to ShadowStrikeHQ, not to ShadowGuard-AI. It is preserved as printed and flagged here, not quietly corrected.

![Minor separator: a fine tide table rule with a single centred spray break](sep-light.svg)

## Usage
`./codeintel-build-process-integrity-checker [params]`

![Major separator: a fine tide table rule in deep sea teal across the full width, with a single spray mark breaking over it at wide intervals](sep-heavy.svg)

## Parameters
- `--build-script`: No description provided
- `--dependency-file`: No description provided
- `--compiler-settings`: No description provided
- `--baseline-hash-build-script`: Baseline SHA256 hash of the build script. If provided, script hash will be checked against it.
- `--baseline-hash-dependency-file`: Baseline SHA256 hash of the dependency file. If provided, dependency file hash will be checked against it.
- `--baseline-hash-compiler-settings`: Baseline SHA256 hash of the compiler settings file. If provided, compiler settings file hash will be checked against it.
- `--run-bandit`: Run Bandit security scanner.
- `--run-flake8`: Run Flake8 code linter.
- `--run-pylint`: Run Pylint code analyzer.
- `--run-pyre`: Run Pyre type checker.
- `--offensive-scan`: No description provided

> **Harbour notice: no description provided, as printed.** Three entries in the list above, --build-script, --dependency-file, and --compiler-settings, carry the words No description provided in the README, and a fourth flag, --offensive-scan, carries the same words with nothing anywhere in the file saying what it scans or how its result changes a run. All four are preserved as printed and flagged here; no purpose is invented for the unexplained flag.

![Major separator: a fine tide table rule in deep sea teal across the full width, with a single spray mark breaking over it at wide intervals](sep-heavy.svg)

## License
Copyright (c) ShadowStrikeHQ

> **Harbour notice: the address names another organisation.** The closing line above reads Copyright (c) ShadowStrikeHQ, preserved as printed and flagged here. The README names no licence in that line.
