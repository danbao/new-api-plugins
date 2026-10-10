---
changelogVersion: 1
plugin: "typesafe"
version: "1.1.1"
locale: "zh-CN"
---
# Changelog

## [1.1.1]

### Fixed

- 渠道模型重定向现在可以正确到达 System One 兼容的后端。渠道可以声明一个 Jev 模型（如 `jev-1.13.0`）并把它映射到其他后端模型（例如 Ollama 上的 `clef-flash:latest`）；之前的版本会拒绝重定向后的名称，所有这类请求都以 "Unsupported TypeSafe model" 失败，尽管模型映射本是文档推荐的用法。
- 通过网关级别别名把自定义模型名映射到 Jev 模型的调用现在也能被接受。
