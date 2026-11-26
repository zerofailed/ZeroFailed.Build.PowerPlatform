# ZeroFailed.Build.PowerPlatform

[![Build Status](https://github.com/zerofailed/ZeroFailed.Build.PowerPlatform/actions/workflows/build.yml/badge.svg)](https://github.com/zerofailed/ZeroFailed.Build.PowerPlatform/actions/workflows/build.yml)
[![License](https://img.shields.io/github/license/zerofailed/ZeroFailed.Build.PowerPlatform.svg)](https://github.com/zerofailed/ZeroFailed.Build.PowerPlatform/blob/main/LICENSE)

A [ZeroFailed](https://github.com/zerofailed/ZeroFailed) extension that provides build features for Microsoft Power Platform and Dataverse solutions.

> **Status:** under development. The extension has no features yet, and no version has been released.

## Overview

| Component Type | Included | Notes |
| -------------- | -------- | ----- |
| Tasks          | planned  | |
| Functions      | planned  | |
| Processes      | no       | Designed to be compatible with the default process provided by the [ZeroFailed.Build.Common](https://github.com/zerofailed/ZeroFailed.Build.Common) extension |

For more information about the different component types, please refer to the [ZeroFailed documentation](https://github.com/zerofailed/ZeroFailed/blob/main/README.md#extensions).

The planned feature groups are listed below. Each one will be documented on the [HELP page](./HELP.md) as it is added.

- Exporting a solution from a development environment and unpacking it into source control
- Packing a solution from source, unmanaged or managed
- Stamping the solution version from the build version
- Running the Solution Checker, with configurable thresholds
- Packaging the solution and its deployment settings template as build artefacts

These run as part of the build process provided by [ZeroFailed.Build.Common](https://github.com/zerofailed/ZeroFailed.Build.Common). Use them together with [ZeroFailed.Deploy.PowerPlatform](https://github.com/zerofailed/ZeroFailed.Deploy.PowerPlatform), which deploys the artefacts this extension produces.

## Pre-requisites

Using the features in this extension requires:

- PowerShell 7.4 or later
- The [Power Platform CLI](https://learn.microsoft.com/power-platform/developer/cli/introduction) (`pac`)

## Building this extension

```pwsh
./build.ps1
```

This runs the build and the Pester tests, using [ZeroFailed.Build.PowerShell](https://github.com/zerofailed/ZeroFailed.Build.PowerShell).
