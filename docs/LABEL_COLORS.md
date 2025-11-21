# Label Organization Guide

## Label Categories

| Label Name | Category | Description |
|------------|----------|-------------|
| bug | issue-type | Something isn't working |
| documentation | issue-type | Improvements or additions to documentation |
| enhancement | issue-type | New feature or request |
| question | issue-type | Further information is requested |
| duplicate | status | This issue or pull request already exists |
| has repro | status | Reproducible issue confirmed |
| platform:macos | platform | Issues affecting macOS |
| platform:linux | platform | Issues affecting Linux |
| platform:windows | platform | Issues affecting Windows |
| area:core | area | Core functionality and architecture |
| area:tools | area | Built-in tool behaviors and integrations |
| area:api | area | API layer and request handling |
| area:mcp | area | Model Context Protocol (MCP) integration |
| area:security | area | Security and permissions |
| area:ide | area | IDE plugins and integration |
| area:model | area | Model behavior and outputs |
| area:packaging | area | Packaging, distribution, and install |
| area:tui | area | Text-based UI and terminal interface |
| area:auth | area | Authentication and credentials |
| memory | topic | Memory features and persistence |
| perf:memory | performance | Performance issues related to memory |
| external | source | External dependency or environment issues |

## Usage Guidelines

- issue-type labels (bug, documentation, enhancement, question): Use these to classify the nature of the issue or pull request. Apply exactly one primary issue-type when possible.
- platform labels (platform:macos, platform:linux, platform:windows): Apply when an issue or change is specific to a particular operating system. Use multiple if reproduced across platforms.
- area labels (area:core, area:tools, area:api, area:mcp, area:security, area:ide, area:model, area:packaging, area:tui, area:auth): Use to indicate the codebase or product component impacted. Multiple area labels are acceptable for cross-cutting work.
- status labels (duplicate, has repro): Use "has repro" when a reproducible case is provided; use "duplicate" when closing in favor of an existing issue.
- performance labels (perf:memory): Apply to issues focused on performance characteristics; combine with an area label for scope.
- topic/source labels (memory, external): Use "memory" to flag memory feature-related items; use "external" when the issue is primarily driven by external tools, environments, or dependencies.

- When creating issues and PRs:
  - Select one issue-type label.
  - Add area labels to reflect impacted components.
  - Add platform when OS-specific.
  - Add status/performance/topic/source labels as needed.
  - Prefer adding labels as a demonstration of categorization to improve visual organization and triage.
