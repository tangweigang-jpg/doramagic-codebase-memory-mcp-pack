# AI Context Pack

## Pack Identity

- Upstream: https://github.com/DeusData/codebase-memory-mcp
- Pack type: Codebase Memory MCP Pack
- Doramagic canonical: https://doramagic.ai/zh/projects/codebase-memory-mcp/
- Relationship: independent pack; not affiliated or endorsed unless explicitly stated.

## Operating Rules

- Evidence first.
- No official endorsement claim.
- Run evals before claiming success.
- Use pitfall and risk files for recovery.

## Host Files

- `../AGENTS.md`
- `../CLAUDE.md`

## Doramagic Source Extract

# codebase-memory-mcp - Doramagic AI Context Pack

> Positioning: a pre-install experience and judgment asset. It helps the host AI get off to a good start, but it does not mean the project has already been installed, run, or validated.

## Sufficiency Principle

- **Sufficiency over compression**: The AI Context Pack should be sufficient for the host AI to understand the project's value, capability boundaries, entrypoints, risks, and evidence sources before starting work; it may be layered, but it does not aim for the shortest possible summary.
- **Compression policy**: Compress only noise and duplication, never context that affects judgment or the quality of the work.

## How the Host AI Should Use This

You are reading the AI Context Pack that Doramagic compiled for codebase-memory-mcp. Treat it as pre-work context: help the user understand who it fits, what it can do, how to start, what must be verified after install, and where the risks are. Do not claim that you have already installed, run, or executed the target project.

## Claim Consumption Rules

- **Fact source**: Repo Evidence + Claim/Evidence Graph; the Human Wiki only supplies salience, terminology, and narrative structure.
- **Minimum status for a fact**: `supported`
- `supported`: May be used as a project fact, but the answer must cite the claim_id and evidence path.
- `weak`: Usable only as a low-confidence lead; the user must be asked to keep verifying.
- `inferred`: Usable only for risk notes or open questions; must not be packaged as a project fact.
- `unverified`: Must not be used as fact; state clearly that evidence is insufficient.
- `contradicted`: Must show the conflicting sources and must not force a single version on the user's behalf.

## Who It Fits Best

- **Developers already using host AIs such as Claude/Codex/Cursor/Gemini**: The README or plugin config mentions multiple host AIs. Evidence: `README.md` Claim: `clm_0002` supported 0.86

## What It Can Do

- **Command-Line Startup or Install Flow** (Verify after install): The project documentation contains runnable commands; real use requires running them in a local or host environment. Evidence: `README.md` Claim: `clm_0001` supported 0.86

## How to Start

- `curl -fsSL https://raw.githubusercontent.com/DeusData/codebase-memory-mcp/main/install.sh | bash` Evidence: `README.md` Claim: `clm_0003` supported 0.86, `clm_0004` supported 0.86
- `curl -fsSL https://raw.githubusercontent.com/DeusData/codebase-memory-mcp/main/install.sh | bash -s -- --ui` Evidence: `README.md` Claim: `clm_0004` supported 0.86
- `curl -fsSL https://raw.githubusercontent.com/DeusData/codebase-memory-mcp/main/scripts/setup.sh | bash` Evidence: `README.md` Claim: `clm_0005` supported 0.86
- `git clone https://github.com/DeusData/codebase-memory-mcp.git` Evidence: `README.md` Claim: `clm_0006` supported 0.86

## Continue-or-Stop Decision Card

- **Current recommendation**: Sandbox-trial permissions first
- **Why**: The project has signals of install commands, host configuration, or local writes; do not go straight into your primary environment—trial it in isolation first.

### 30-Second Read

- **What to do now**: Sandbox-trial permissions first
- **Minimum safe next step**: Run Prompt Preview first; if you still want to install, trial only in an isolated environment
- **Do not trust yet**: Tool permission boundaries cannot be trusted before install.
- **Continuing will touch**: Command execution, Local environment or project files, Host AI context

### What You Can Trust Now

- **Target-audience signal: Developers already using host AIs such as Claude/Codex/Cursor/Gemini** (supported): Backed by a supported claim or project evidence, but that still is not the same as real install results. Evidence: `README.md` Claim: `clm_0002` supported 0.86
- **Capability exists: Command-Line Startup or Install Flow** (supported): You can trust that the project contains signals of this capability; whether it fits your specific task still needs trial or after-install verification. Evidence: `README.md` Claim: `clm_0001` supported 0.86
- **There are Quick Start / install-command signals** (supported): You can trust that the docs mention a startup or install entrypoint; do not run it directly in your primary environment because of that. Evidence: `README.md` Claim: `clm_0003` supported 0.86, `clm_0004` supported 0.86

### What You Cannot Trust Yet

- **Tool permission boundaries cannot be trusted before install.** (unverified): MCP/tool projects usually touch files, the network, the browser, or external APIs, so permissions and logs must be checked for real.
- **Real output quality cannot be trusted before install.** (unverified): Prompt Preview can only show how it guides you; it cannot prove result quality in the real project.
- **Host AI version compatibility cannot be trusted before install.** (unverified): Host loading rules and version differences across Claude, Cursor, Codex, Gemini, and others must be verified in a real environment.
- **That it will not pollute your existing host AI's behavior cannot be trusted directly.** (inferred): Skill, plugin, and AGENTS/CLAUDE/GEMINI instructions may change the host AI's default behavior.
- **Safe rollback cannot be assumed by default.** (unverified): Unless the project clearly provides uninstall and recovery instructions, verify in an isolated environment first.
- **After a real install, is it compatible with the user's current host AI version?** (unverified): Compatibility can only be verified in the actual host environment.
- **Does the project's output quality meet the user's specific task?** (unverified): The pre-install preview can only show flow and boundaries; it cannot replace real evaluation.
- **Do the install commands require network access, permissions, or global writes?** (unverified): This affects install risk in both enterprise and personal environments. Evidence: `README.md`

### What Continuing Will Touch

- **Command execution**: Package managers, network downloads, the local plugin directory, project config, or the user's home directory. Why: Running the very first command can already change your environment; decide whether it is worth running first. Evidence: `README.md`
- **Local environment or project files**: Install results, plugin caches, project config, or local dependency directories. Why: The write scope and rollback path cannot be proven before install and need isolated verification. Evidence: `README.md`
- **Host AI context**: The AI Context Pack, Prompt Preview, Skill routing, risk rules, and project facts. Why: Importing context affects the host AI's later judgment, so avoid packaging unverified items as facts.

### Minimum Safe Next Steps

- **Run Prompt Preview first**: Use a pre-install interactive trial to judge whether the way of working fits; it needs no authorization or environment change. (applies when: Applies to any project, especially when output quality is unknown.)
- **Trial-install only in an isolated directory or a test account**: Avoid letting install commands pollute your primary host AI, real projects, or home directory. (applies when: When there are signals of command execution, plugin config, or local writes.)
- **After install, verify just one minimal task**: Verify loading, compatibility, output quality, and rollback first, then decide whether to use it deeply. (applies when: When moving from a trial into a real workflow.)

### Exit Plan

- **Preserve the pre-install state**: Record the original host config and project state so you can later judge whether it is recoverable.
- **Record the install commands and written paths**: Without clear uninstall instructions, you at least need to know which directories or configs to clean up manually.
- **If there is no rollback path, do not enter your primary environment**: No rollback is a blocker before continuing; do not proceed on trust or luck.

## What Can Only Be Previewed

- Explain who the project fits and what it can do
- Demonstrate a typical conversation flow based on project docs
- Help the user decide whether it is worth installing or researching further

## What Must Be Verified After Install

- Actually installing the Skill, plugin, or CLI
- Running scripts, modifying local files, or accessing external services
- Verifying real output quality, performance, and compatibility

## Boundary & Risk Decision Card

- **Mistaking the pre-install preview for a real run**: The user may overestimate how much configuration, permission, and compatibility verification the project has already done. Mitigation: Clearly separate prompt_preview_can_do from runtime_required. Claim: `clm_0007` inferred 0.45
- **Command execution will modify the local environment**: Install commands may write to the user's home directory, the host plugin directory, or project configuration. Mitigation: Run in an isolated environment or a test account first. Evidence: `README.md` Claim: `clm_0008` supported 0.86
- **To confirm**: After a real install, is it compatible with the user's current host AI version?. Why: Compatibility can only be verified in the actual host environment.
- **To confirm**: Does the project's output quality meet the user's specific task?. Why: The pre-install preview can only show flow and boundaries; it cannot replace real evaluation.
- **To confirm**: Do the install commands require network access, permissions, or global writes?. Why: This affects install risk in both enterprise and personal environments.

## Pre-Work Working Context

### Loading Order

- First read how_to_use.host_ai_instruction to establish the boundaries of this pre-install judgment asset.
- Read claim_graph_summary to confirm facts come from the Claim/Evidence Graph, not the Human Wiki narrative.
- Then read intended_users, capabilities, and quick_start_candidates to judge whether the user is a match.
- When you need to carry out a concrete task, check role_skill_index first, then evidence_index.
- For real install, file modification, network access, performance, or compatibility questions, turn to risk_card and boundaries.runtime_required.

### Task Routes

- **Command-Line Startup or Install Flow**: State that this is an after-install capability first, then give a pre-install checklist. Boundary: Must be verified after a real install or run. Evidence: `README.md` Claim: `clm_0001` supported 0.86

### Context Scale

- Total files: 1615
- Important-file coverage: 40/1615
- Evidence index entries: 80
- Role / Skill entries: 6

### Handling Insufficient Evidence

- **missing_evidence**: State that evidence is insufficient and ask the user for the target file, a README section, or after-install verification records; do not fill in facts.
- **out_of_scope_request**: State that the task is beyond the current AI Context Pack's evidence scope and suggest the user check the Human Manual or verify after a real install.
- **runtime_request**: Provide a pre-install checklist and command sources, but do not run commands for the user or claim they have been run.
- **source_conflict**: Show the conflicting sources side by side, mark them as unverified, and do not force a single version.

## Prompt Recipes

### Fit assessment

- Goal: Judge whether this project fits the user's current task.
- Expected output: A fit conclusion, key reasons, evidence citations, what can be previewed before install, what must be verified after install, and a next-step recommendation.

```text
Based on the AI Context Pack for codebase-memory-mcp, ask me 3 necessary questions first, then judge whether it fits my task. The answer must cover: who it fits, what it can do, what it cannot do, whether it is worth installing, and where the evidence comes from. Every project fact must cite evidence_refs, source_paths, or a claim_id.
```

### Pre-install experience

- Goal: Let the user feel the core workflow before installing, while avoiding packaging the preview as real capability or a marketing promise.
- Expected output: An experience script with boundary labels, an after-install verification checklist, and a cautious recommendation; with no real-run promises or strong marketing language.

```text
Treat codebase-memory-mcp as a pre-install experience asset, not an already-installed tool or a real runtime environment.

Output exactly four parts:
1. Ask me 3 necessary questions first.
2. Give an "experience script": use the three labels [Previewable before install], [Must verify after install], and [Insufficient evidence] to show how it might guide the workflow.
3. Give an after-install verification checklist: list which capabilities can only be confirmed after a real install, real host loading, and a real project run.
4. Give a cautious recommendation: only "worth researching/trialing further", "add information before deciding", or "not recommended to continue"; do not endorse the project.

Hard boundaries:
- Do not claim you have installed, run, executed tests, modified files, or produced real results.
- Do not write promise-like phrasing such as "auto-adapts", "guarantees passing", "perfect fit", or "strongly recommend installing".
- If you describe how it works after install, you must use a conditional such as "if installed successfully and the host loads the Skill correctly, it might...".
- The experience script may only be written as "example lines / hypothetical flow": use "might ask / might suggest / might show", not "has written, has generated, has passed, is running, is generating".
- Prompt Preview does not hand out install commands; if the user is ready to trial, only prompt them to read Quick Start and the Risk Card first and to verify in an isolated environment.
- Every project fact must come from a supported claim, evidence_refs, or source_paths; inferred/unverified items can only be risks or open questions.

```

### Role / Skill selection

- Goal: Pick the best-matching asset from the project's roles or Skills.
- Expected output: A list of candidate roles or Skills, each with an applicable scenario, evidence paths, risk boundary, and whether after-install verification is needed.

```text
Read role_skill_index and recommend 3-5 of the most relevant roles or Skills for my target task. For each recommendation, state the applicable scenario, likely output, risk boundary, and evidence_refs.
```

### Risk pre-check

- Goal: Identify environment, permission, rule-conflict, and quality risks before installing or adopting.
- Expected output: A checklist of environment, permission, dependency, license, host-conflict, quality risk, and unknown items.

```text
Based on risk_card, boundaries, and quick_start_candidates, give me a pre-install risk pre-check list. Do not run commands for me; only explain what I should check, why, and what impact a failure would have.
```

### Host AI kickoff instruction

- Goal: Turn the project context into a host AI instruction for the start of a conversation.
- Expected output: A pre-work instruction with clear boundaries and clear evidence citations, suitable to copy to a host AI.

```text
Based on the AI Context Pack for codebase-memory-mcp, generate a pre-work instruction I can paste to my host AI. This instruction must obey not_runtime=true and must not claim the project has been installed, run, or produced real results.
```


## Role / Skill Index

- Indexed 6 role / Skill / project-doc entries.

- **codebase-memory-mcp** (project_doc): ! GitHub Release https://img.shields.io/github/v/release/DeusData/codebase-memory-mcp?style=flat&color=blue https://github.com/DeusData/codebase-memory-mcp/releases/latest ! License https://img.shields.io/badge/license-MIT-green LICENSE ! CI https://img.shields.io/github/actions/workflow/status/DeusData/codebase-memory-mcp/dry-run.yml?label=CI https://github.com/DeusData/codebase-memory-mcp/actions/workflows/dry-run… Activation hint: Reference this when the user needs to understand the project's structure, install path, or boundaries. Evidence: `README.md`
- **codebase-memory-mcp** (project_doc): ! npm https://img.shields.io/npm/v/codebase-memory-mcp?style=flat&color=blue https://www.npmjs.com/package/codebase-memory-mcp ! GitHub Release https://img.shields.io/github/v/release/DeusData/codebase-memory-mcp?style=flat&color=blue https://github.com/DeusData/codebase-memory-mcp/releases/latest ! License https://img.shields.io/badge/license-MIT-green https://github.com/DeusData/codebase-memory-mcp/blob/main/LICEN… Activation hint: Reference this when the user needs to understand the project's structure, install path, or boundaries. Evidence: `pkg/npm/README.md`
- **codebase-memory-mcp** (project_doc): mcp-name: io.github.DeusData/codebase-memory-mcp Activation hint: Reference this when the user needs to understand the project's structure, install path, or boundaries. Evidence: `pkg/pypi/README.md`
- **Portability Primitives** (project_doc): This is the portability layer where all primitives needed from the OS are defined. Activation hint: Reference this when the user needs to understand the project's structure, install path, or boundaries. Evidence: `vendored/mimalloc/src/prim/readme.md`
- **Primitives:** (project_doc): - prim.c contains Windows primitives for OS allocation. Activation hint: Reference this when the user needs to understand the project's structure, install path, or boundaries. Evidence: `vendored/mimalloc/src/prim/windows/readme.md`
- **Contributing to codebase-memory-mcp** (project_doc): Contributing to codebase-memory-mcp Activation hint: Reference this when the user needs to understand the project's structure, install path, or boundaries. Evidence: `CONTRIBUTING.md`

## Evidence Index

- Indexed 80 evidence entries.

- **codebase-memory-mcp** (documentation): ! GitHub Release https://img.shields.io/github/v/release/DeusData/codebase-memory-mcp?style=flat&color=blue https://github.com/DeusData/codebase-memory-mcp/releases/latest ! License https://img.shields.io/badge/license-MIT-green LICENSE ! CI https://img.shields.io/github/actions/workflow/status/DeusData/codebase-memory-mcp/dry-run.yml?label=CI https://github.com/DeusData/codebase-memory-mcp/actions/workflows/dry-run.yml ! Tests https://img.shields.io/badge/tests-5604 passing-brightgreen https://github.com/DeusData/codebase-memory-mcp ! Languages https://img.shields.io/badge/languages-158-orange https://github.com/DeusData/codebase-memory-mcp ! Hybrid LSP https://img.shields.io/badge/Hybrid… Evidence: `README.md`
- **codebase-memory-mcp** (documentation): ! npm https://img.shields.io/npm/v/codebase-memory-mcp?style=flat&color=blue https://www.npmjs.com/package/codebase-memory-mcp ! GitHub Release https://img.shields.io/github/v/release/DeusData/codebase-memory-mcp?style=flat&color=blue https://github.com/DeusData/codebase-memory-mcp/releases/latest ! License https://img.shields.io/badge/license-MIT-green https://github.com/DeusData/codebase-memory-mcp/blob/main/LICENSE ! Platform https://img.shields.io/badge/macOS %7C Linux %7C Windows-supported-lightgrey https://github.com/DeusData/codebase-memory-mcp/releases/latest Evidence: `pkg/npm/README.md`
- **codebase-memory-mcp** (documentation): mcp-name: io.github.DeusData/codebase-memory-mcp Evidence: `pkg/pypi/README.md`
- **Portability Primitives** (documentation): This is the portability layer where all primitives needed from the OS are defined. Evidence: `vendored/mimalloc/src/prim/readme.md`
- **Primitives:** (documentation): - prim.c contains Windows primitives for OS allocation. Evidence: `vendored/mimalloc/src/prim/windows/readme.md`
- **Package** (package_manifest): { "name": "graph-ui", "private": true, "version": "0.1.0", "type": "module", "scripts": { "dev": "vite", "build": "tsc -b && vite build", "preview": "vite preview", "test": "vitest run", "test:watch": "vitest", "test:coverage": "vitest run --coverage" }, "dependencies": { "@react-three/drei": "^10.7.0", "@react-three/fiber": "^9.5.0", "@react-three/postprocessing": "^3.0.4", "class-variance-authority": "^0.7.1", "clsx": "^2.1.1", "lucide-react": "^0.577.0", "postprocessing": "^6.38.3", "radix-ui": "^1.4.3", "react": "^19.0.0", "react-dom": "^19.0.0", "tailwind-merge": "^3.5.0", "three": "~0.183.0" }, "devDependencies": { "@tailwindcss/vite": "^4.2.1", "@testing-library/jest-dom": "^6.6.0",… Evidence: `graph-ui/package.json`
- **Package** (package_manifest): { "name": "codebase-memory-mcp", "version": "0.8.1", "description": "Fast code intelligence engine for AI coding agents — single static binary MCP server", "mcpName": "io.github.DeusData/codebase-memory-mcp", "license": "MIT", "repository": { "type": "git", "url": "git+https://github.com/DeusData/codebase-memory-mcp.git" }, "homepage": "https://github.com/DeusData/codebase-memory-mcp", "bugs": { "url": "https://github.com/DeusData/codebase-memory-mcp/issues" }, "keywords": "mcp", "claude", "code-intelligence", "codebase", "memory", "ai", "llm", "tree-sitter" , "bin": { "codebase-memory-mcp": "./bin.js" }, "scripts": { "postinstall": "node install.js" }, "engines": { "node": " =18" }, "os":… Evidence: `pkg/npm/package.json`
- **Package** (package_manifest): { "name": "tree-sitter-form", "version": "0.1.0", "description": "FORM symbolic manipulation grammar for tree-sitter", "main": "bindings/node", "keywords": "tree-sitter", "form", "symbolic-computation", "particle-physics" , "license": "MIT", "dependencies": { "nan": "^2.18.0" }, "devDependencies": { "tree-sitter-cli": "^0.25.0" }, "tree-sitter": { "scope": "source.form", "file-types": "frm", "prc" , "highlights": "queries/highlights.scm" } } Evidence: `tools/tree-sitter-form/package.json`
- **Package** (package_manifest): { "name": "tree-sitter-magma", "version": "0.1.0", "description": "Magma computer algebra grammar for tree-sitter", "main": "bindings/node", "keywords": "tree-sitter", "magma", "computer-algebra", "number-theory" , "license": "MIT", "dependencies": { "nan": "^2.18.0" }, "devDependencies": { "tree-sitter-cli": "^0.25.0" }, "tree-sitter": { "scope": "source.magma", "file-types": "mag", "magma" , "highlights": "queries/highlights.scm" } } Evidence: `tools/tree-sitter-magma/package.json`
- **Contributing to codebase-memory-mcp** (documentation): Contributing to codebase-memory-mcp Evidence: `CONTRIBUTING.md`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/common/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/common/tree_sitter/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/ada/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/agda/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/apex/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/assembly/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/astro/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/awk/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/bash/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/beancount/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/bibtex/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/bicep/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/bitbake/LICENSE`
- **License** (source_file): Copyright c 2023 Emran Mashhadi Ramezan Evidence: `internal/cbm/vendored/grammars/blade/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/c/LICENSE`
- **License** (source_file): Copyright c 2014-2023 Max Brunsfeld, Damien Guard, Amaan Qureshi, and contributors. Evidence: `internal/cbm/vendored/grammars/c_sharp/LICENSE`
- **License** (source_file): Copyright c 2023 Amaan Qureshi , Blaž Hrastnik , Scott Piriou Evidence: `internal/cbm/vendored/grammars/cairo/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/capnp/LICENSE`
- **License** (source_file): Copyright c 2014 Gareth Edwards & Gavin Baumanis Evidence: `internal/cbm/vendored/grammars/cfml/LICENSE`
- **License** (source_file): Copyright c 2014 Gareth Edwards & Gavin Baumanis Evidence: `internal/cbm/vendored/grammars/cfscript/LICENSE`
- **License** (source_file): CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE LEGAL SERVICES. DISTRIBUTION OF THIS DOCUMENT DOES NOT CREATE AN ATTORNEY-CLIENT RELATIONSHIP. CREATIVE COMMONS PROVIDES THIS INFORMATION ON AN "AS-IS" BASIS. CREATIVE COMMONS MAKES NO WARRANTIES REGARDING THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS PROVIDED HEREUNDER, AND DISCLAIMS LIABILITY FOR DAMAGES RESULTING FROM THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS PROVIDED HEREUNDER. Evidence: `internal/cbm/vendored/grammars/clojure/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/cmake/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/cobol/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/commonlisp/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/cpp/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/crystal/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/css/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/csv/LICENSE`
- **License** (source_file): Copyright c 2014 Max Brunsfield Copyright c 2021 Stephan Seitz Evidence: `internal/cbm/vendored/grammars/cuda/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/d/LICENSE`
- **License** (source_file): Copyright c 2020-2023 UserNobody14 and others Evidence: `internal/cbm/vendored/grammars/dart/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/devicetree/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/diff/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/dockerfile/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/dotenv/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/elisp/LICENSE`
- **License** (source_file): Apache License Version 2.0, January 2004 http://www.apache.org/licenses/ Evidence: `internal/cbm/vendored/grammars/elixir/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/elm/LICENSE`
- **License** (source_file): Apache License Version 2.0, January 2004 http://www.apache.org/licenses/ Evidence: `internal/cbm/vendored/grammars/erlang/LICENSE`
- **License** (source_file): CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE LEGAL SERVICES. DISTRIBUTION OF THIS DOCUMENT DOES NOT CREATE AN ATTORNEY-CLIENT RELATIONSHIP. CREATIVE COMMONS PROVIDES THIS INFORMATION ON AN "AS-IS" BASIS. CREATIVE COMMONS MAKES NO WARRANTIES REGARDING THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS PROVIDED HEREUNDER, AND DISCLAIMS LIABILITY FOR DAMAGES RESULTING FROM THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS PROVIDED HEREUNDER. Evidence: `internal/cbm/vendored/grammars/fennel/LICENSE`
- **License** (source_file): This is free and unencumbered software released into the public domain. Evidence: `internal/cbm/vendored/grammars/fish/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/form/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/fortran/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/fsharp/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/func/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/gdscript/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/gitattributes/LICENSE`
- **License** (source_file): Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files the "Software" , to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions: Evidence: `internal/cbm/vendored/grammars/gitignore/LICENSE`
- **License** (source_file): Apache License Version 2.0, January 2004 http://www.apache.org/licenses/ Evidence: `internal/cbm/vendored/grammars/gleam/LICENSE`
- The remaining 20 evidence entries are in `AI_CONTEXT_PACK.json` or `EVIDENCE_INDEX.json`.

## Rules the Host AI Must Follow

- **Treat this asset as pre-work context, not a runtime environment.**: The AI Context Pack contains only an evidence-backed understanding of the project, not the project's executable state. Evidence: `README.md`, `pkg/npm/README.md`, `pkg/pypi/README.md`
- **When answering the user, distinguish what can be previewed from what can only be verified after install.**: The consumer value of the pre-install experience comes from reducing bad installs and misjudgments, not from pretending to be a real run. Evidence: `README.md`, `pkg/npm/README.md`, `pkg/pypi/README.md`

## Questions the User Should Answer First

- Which host AI or local environment do you plan to use it in?
- Do you just want to experience the workflow first, or are you ready to actually install?
- What matters most to you: install cost, output quality, or conflicts with your existing rules?

## Acceptance Checks

- Every capability claim can be traced back to a file path in evidence_refs.
- AI_CONTEXT_PACK.md does not package previews as a real run.
- The user can understand who it fits, what it can do, how to start, and the risk boundaries within 3 minutes.

---

## Doramagic Context Augmentation

The following sections strengthen the repository context for a host AI. Human Manual data is a reading route, and pitfall notes become operating constraints.

## Human Manual Outline

Usage rule: this is only a reading route and salience signal, not factual authority. Concrete claims must still return to repo evidence or Claim Graph.

Host AI hard rules:
- Do not treat page titles, section order, summaries, or importance values as factual project evidence.
- When explaining the Human Manual outline, state that it is only a reading route or salience signal.
- Capability, installation, compatibility, runtime state, and risk claims must cite repo evidence, source paths, or Claim Graph.

- **Overview & System Architecture**: importance `high`
  - source_paths: README.md, src/main.c, src/mcp/mcp.c, src/foundation/compat.c, internal/cbm/cbm.c
- **Indexing Pipeline & Hybrid LSP**: importance `high`
  - source_paths: src/pipeline/pipeline.c, src/pipeline/pipeline_incremental.c, src/pipeline/artifact.c, internal/cbm/extract_unified.c, internal/cbm/extract_calls.c
- **MCP Server, Query System & Graph Data Model**: importance `high`
  - source_paths: src/mcp/mcp.c, src/mcp/index_supervisor.c, src/cypher/cypher.c, src/store/store.c, src/store/store.h
- **Distribution, Frontend UI & Known Operational Issues**: importance `medium`
  - source_paths: install.sh, install.ps1, src/ui/httpd.c, src/ui/http_server.c, src/ui/layout3d.c

## Repo Inspection Evidence

- repo_clone_verified: true
- repo_inspection_verified: true
- repo_commit: `6b57db271aadcfc76206f5b568981a6a90e81cdc`
- inspected_files: `README.md`, `docs/BENCHMARK.md`, `docs/CONFIGURATION.md`, `docs/EVALUATION_PLAN.md`, `docs/SECURITY-DISCLOSURE.md`, `docs/cbmignore.md`

Host AI hard rules:
- Without repo_clone_verified=true, do not claim that the source code has been read.
- Without repo_inspection_verified=true, do not write README, docs, or package-file conclusions as facts.
- Without quick_start_verified=true, do not claim that the Quick Start path has run successfully.

## Doramagic Pitfall Constraints

These rules come from Doramagic discovery, validation, or compilation findings. The host AI must treat them as operating constraints, not background notes.

### Constraint 1: Installation risk requires verification

- Trigger: Developers should check this installation risk before relying on the project: Add deterministic cross-repository dependency graphing for Go workspaces
- Host AI rule: Before packaging this project, run the relevant install/config/quickstart check for: Add deterministic cross-repository dependency graphing for Go workspaces. Context: Observed during installation or first-run setup.
- Why it matters: Developers may fail before the first successful local run: Add deterministic cross-repository dependency graphing for Go workspaces
- Evidence: failure_mode_cluster:github_issue | https://github.com/DeusData/codebase-memory-mcp/issues/969
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 2: Installation risk requires verification

- Trigger: Developers should check this installation risk before relying on the project: Custom Exploring Subagent — inject MCP-aware agent definitions on integration
- Host AI rule: Before packaging this project, run the relevant install/config/quickstart check for: Custom Exploring Subagent — inject MCP-aware agent definitions on integration. Context: Observed during installation or first-run setup.
- Why it matters: Developers may fail before the first successful local run: Custom Exploring Subagent — inject MCP-aware agent definitions on integration
- Evidence: failure_mode_cluster:github_issue | https://github.com/DeusData/codebase-memory-mcp/issues/975
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 3: Installation risk requires verification

- Trigger: Developers should check this installation risk before relying on the project: Memory leak: process grows to 50+ GB virtual memory over hours/days, crashes Windows
- Host AI rule: Before packaging this project, run the relevant install/config/quickstart check for: Memory leak: process grows to 50+ GB virtual memory over hours/days, crashes Windows. Context: Observed when using python, windows
- Why it matters: Developers may fail before the first successful local run: Memory leak: process grows to 50+ GB virtual memory over hours/days, crashes Windows
- Evidence: failure_mode_cluster:github_issue | https://github.com/DeusData/codebase-memory-mcp/issues/581
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 4: Installation risk requires verification

- Trigger: Developers should check this installation risk before relying on the project: [Windows] --ui=true starts but HTTP server never listens on v0.8.1
- Host AI rule: Before packaging this project, run the relevant install/config/quickstart check for: [Windows] --ui=true starts but HTTP server never listens on v0.8.1. Context: Observed when using windows
- Why it matters: Developers may fail before the first successful local run: [Windows] --ui=true starts but HTTP server never listens on v0.8.1
- Evidence: failure_mode_cluster:github_issue | https://github.com/DeusData/codebase-memory-mcp/issues/707
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 5: Installation risk requires verification

- Trigger: Developers should check this installation risk before relying on the project: feat: install codebase-memory skill for Codex
- Host AI rule: Before packaging this project, run the relevant install/config/quickstart check for: feat: install codebase-memory skill for Codex. Context: Observed during installation or first-run setup.
- Why it matters: Developers may fail before the first successful local run: feat: install codebase-memory skill for Codex
- Evidence: failure_mode_cluster:github_issue | https://github.com/DeusData/codebase-memory-mcp/issues/976
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

### Constraint 6: Installation risk requires verification

- Trigger: Developers should check this installation risk before relying on the project: v0.5.6
- Host AI rule: Before packaging this project, run the relevant install/config/quickstart check for: v0.5.6. Context: Observed when using node, python, docker, windows
- Why it matters: Upgrade or migration may change expected behavior: v0.5.6
- Evidence: failure_mode_cluster:github_release | https://github.com/DeusData/codebase-memory-mcp/releases/tag/v0.5.6
- Hard boundary: Do not present this pitfall as solved, verified, or ignorable unless later evidence explicitly closes it.

