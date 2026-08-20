# GSIM NanoPlotter — Script Customization

## What this is

This repo is for developing and version-controlling custom `.npl` scripts that run inside
GeSiM's **NanoPlotter Control (NPC16)** software, which drives the lab's NanoPlotter
piezo-dispensing "spotter" instrument.

**Scope**: we are not rebuilding or replacing NPC16. The goal is to write, review, and
version scripts (and supporting notes) that customize spotting/dispensing sequences for
our experiments, based on the vendor software and its manuals.

## Layout

- `scripts/` — our custom/customized `.npl` scripts. This is the actual tracked deliverable
  of this repo.
- `Spotter/` — a working copy of the NPC16 installation from the lab PC (binaries, vendor
  manuals, historical Data/Report logs, existing `Prog/` scripts). **Not tracked in git**
  (see `.gitignore`) — kept locally as reference material and as the folder the NPC16
  software actually runs from. Treat it as read/reference-only unless you're deliberately
  updating the local install.

## Background

- **NPC16** = NanoPlotter Control software v16, GeSiM's control application for the
  NanoPlotter spotting robot.
- **`.npl` files** are NPC16's script format for defining automated dispensing/motion
  sequences. See `Spotter/Prog/*.npl` for existing examples and
  `Spotter/Nanoplotter 2.1/*.pdf` for the vendor manuals.
- Scripts already customized by prior lab operators live in `Spotter/Prog/` (the vendor
  working folder, gitignored). New scripts developed here in `scripts/` are meant to be
  copied into `Spotter/Prog/` on the instrument PC to run.

## Status

Just getting organized. Add specifics here (target experiments, current script goals,
hardware notes) as the project develops.
