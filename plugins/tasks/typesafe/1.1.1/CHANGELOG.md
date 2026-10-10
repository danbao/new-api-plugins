---
changelogVersion: 1
plugin: "typesafe"
version: "1.1.1"
locale: "en"
translations:
  zh-CN: "CHANGELOG.zh-CN.md"
---
# Changelog

## [1.1.1]

### Fixed

- Channel model redirects now reach System One-compatible backends. A channel can declare a Jev model such as `jev-1.13.0` and map it to a different backend model like `clef-flash:latest` on an Ollama server; earlier versions rejected the redirected name and failed every such request with "Unsupported TypeSafe model" even though mapping was the documented fallback.
- Gateway-level aliases that map a custom client model name to a Jev model are now accepted as well.
