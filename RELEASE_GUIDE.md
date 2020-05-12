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
