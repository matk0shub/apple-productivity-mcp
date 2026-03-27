# Changelog

All notable changes to this repository will be documented in this file.

## 0.1.0 - 2026-03-27

### Added

- `apple-calendar` plugin with:
  - EventKit backend
  - agenda, free-window, search, update, delete
  - reminders management
  - recurring events
  - `.ics` export and import

- `apple-reminders` plugin with:
  - EventKit backend
  - due, overdue, alarms-today
  - add, update, done, reopen, delete
  - move between lists
  - recurring reminders
  - AppleScript fallback for flag and unflag

- shared local `apple-productivity` stdio MCP server exposing both domains

- integration smoke tests for:
  - CLI workflows
  - MCP workflows

- install helper for local path rewriting and marketplace setup

## 0.1.1 - 2026-03-27

### Changed

- separated installable Codex plugins from the shared MCP server layer
- moved the shared server to `mcp/apple-productivity/`
- simplified marketplace layout to install only the user-facing plugins
- added a generated `mcp.local.json` flow through the installer

### Improved

- clearer top-level onboarding and repository structure
- clearer distinction between plugin UX and shared MCP infrastructure
- added architecture documentation for the split between `plugins/` and `mcp/`
