# cybros labs Scoop Bucket

A [Scoop](https://scoop.sh) bucket containing manifests for cybros labs CLI tools.

## Prerequisites

[Scoop](https://scoop.sh) must be installed on your Windows system. No administrator privileges are required.

To install Scoop, open PowerShell and run:

```powershell
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Invoke-RestMethod -Uri https://get.scoop.sh | Invoke-Expression
```

## Usage

### Add this bucket

```powershell
scoop bucket add cybroslabs https://github.com/cybroslabs/scoop-tools
```

### Install a tool

```powershell
scoop install cybroslabs/<tool-name>
```

### Update a tool

```powershell
scoop update <tool-name>
```

### Uninstall a tool

```powershell
scoop uninstall <tool-name>
```

## How it works

This repository serves as a Scoop bucket -- a collection of JSON manifest files that describe how to download and install each tool. Each manifest contains the download URLs, checksums, and binary paths for the corresponding tool.

Manifests are automatically generated and updated by CI/CD pipelines whenever a new version of a tool is released. Manual edits to manifest files are not necessary and will be overwritten on the next release.

## About

Published and maintained by [cybros labs](https://www.cybroslabs.com).
