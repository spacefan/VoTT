# Overview

Instruction on how to release preview and final artifacts

## Versioning

Follow [NPM Semantic Versioning](https://docs.npmjs.com/about-semantic-versioning#incrementing-semantic-versions-in-published-packages)

| Code status                               | Stage         | Rule                                                               | Example version |
| ----------------------------------------- | ------------- | ------------------------------------------------------------------ | --------------- |
| First release                             | New product   | Start with 1.0.0                                                   | 1.0.0           |
| Backward compatible bug fixes             | Patch release | Increment the third digit                                          | 1.0.1           |
| Backward compatible new features          | Minor release | Increment the middle digit and reset last digit to zero            | 1.1.0           |
| Changes that break backward compatibility | Major release | Increment the first digit and reset middle and last digits to zero | 2.0.0           |

### Commands

Use [npm-version](https://docs.npmjs.com/cli/version) to update version

### Pre

All version with `pre`, ie. `preminor` will append `-0` to the new version

Examples:

1. `npm version prepatch` - v2.3.0 --> v2.3.1-0
1. `npm version preminor` - v2.3.0 --> v2.4.0-0

### Major

v2.x.x --> v3.0.0

### Minor

v2.2.0 --> v2.3.0

## GitHub Release

1. Generate Changelog
1. Update `package.json` version
    - Use script(?)
1. Create PR
1. Merge PR
1. Tag Branch
1. Kick off release pipeline
    - Same pipeline for preview & non-preview?

### Preview

### Non-Preview

### FAQ

Q) What is consider preview?
A) `Dev` branch release?

## Web Release

### Dev Static Site

Manually queue the [Create Web Release]() pipeline off `develop` branch.

### Prod Static Site

Manually queue the [Create Web Release]() pipeline off `master` branch.
