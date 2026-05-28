# SurfGuard Power Apps Source Submission

This repository contains the source submission for the SurfGuard Assignment 2 Power Apps MVP.

## Included Files

- `SurfGuard.msapp` — exported Power Apps canvas application package
- `SurfGuardManualUnpack/` — manually extracted contents of the `.msapp` package

## Notes

Multiple attempts were made to unpack the `.msapp` file using Microsoft Power Platform CLI, including running the command from both VS Code and the macOS Terminal, refreshing the CLI path, and retrying the unpack process from different working directories.

The intended Microsoft Power Platform CLI command was:

`pac canvas unpack --msapp "./SurfGuard.msapp" --sources "./SurfGuardSource"`

However, each attempt failed with a non-recoverable `System.NullReferenceException`.

As a workaround, the `.msapp` file was manually extracted as a zip archive, which successfully produced the app source structure, including Power Apps YAML screen definitions, control metadata, references, tests, and assets.

This repository therefore includes both the original `.msapp` file and the manually extracted source contents.
