---
title: Hackathon KB Test Overview
type: note
permalink: hackathon-test/overview
tags:
  - hackathon
  - test
---

## Overview

This repo is a test KB used to demonstrate the `pvm validate` command and the `basic-memory-validate` pre-commit hook built during the Planview Hackathon June 2026.

## What this demos

- Valid notes pass validation and can be committed
- Malformed notes (missing frontmatter, broken wikilinks) are caught before they land in the repo
- The pre-commit hook runs automatically on every `git commit` without any manual steps

## Related

- Hook definition: [[MANIFEST]]
- CLI source: https://github.com/Tasktop-Cloud-PVS/hackathon-kb-cli
