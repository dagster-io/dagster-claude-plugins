<div align="center">
  <img width="auto" height="38px" alt="dagster-hearts-claude" src="https://github.com/user-attachments/assets/b162dddf-6a7e-459e-be06-29d34d637650" />
</div>

# Dagster Skills

[![Lint](https://github.com/dagster-io/skills/actions/workflows/lint.yml/badge.svg)](https://github.com/dagster-io/skills/actions/workflows/lint.yml)

AI assistant skills for building workflows and data pipelines using Dagster.

**Compatible with Claude Code, OpenCode, OpenAI Codex, Pi, and other Agent Skills-compatible
tools.**

## Installation

### Claude Code

Install using the
[Claude plugin marketplace](https://code.claude.com/docs/en/discover-plugins#add-from-github):

```
/plugin marketplace add dagster-io/skills
```

### Using `npx skills`

Install using the [`npx skills`](https://skills.sh/) command-line:

```bash
npx skills add dagster-io/skills
```

### Manual Installation

<details>
<summary>See full instructions...</summary>

Clone the repository and copy skills to your tool's skills directory:

**OpenCode:**

```bash
git clone https://github.com/dagster-io/skills.git
cp -r skills/plugins/* ~/.config/opencode/skill/
```

**OpenAI Codex:**

```bash
git clone https://github.com/dagster-io/skills.git
cp -r skills/plugins/* ~/.codex/skills/
```

**Pi Agent:**

```bash
git clone https://github.com/dagster-io/skills.git
cp -r skills/plugins/* ~/.pi/agent/skills/
```

</details>

## Skills

### dg

Commands for building, executing, and debugging Dagster projects.

<table>
  <thead>
    <tr>
      <th width="30%">Command</th>
      <th width="70%">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>/dg:list</code></td>
      <td>List and inspect Dagster definitions, components, environment variables, and project structure</td>
    </tr>
    <tr>
      <td><code>/dg:create-project &lt;name&gt;</code></td>
      <td>Create a new Dagster project with recommended structure</td>
    </tr>
    <tr>
      <td><code>/dg:create-workspace &lt;name&gt;</code></td>
      <td>Initialize a workspace for managing multiple projects</td>
    </tr>
    <tr>
      <td><code>/dg:scaffold</code></td>
      <td>Scaffold Dagster components, assets, schedules, sensors, and integrations</td>
    </tr>
    <tr>
      <td><code>/dg:prototype &lt;requirements&gt;</code></td>
      <td>Build production-ready Dagster implementations with best practices, testing, and validation</td>
    </tr>
    <tr>
      <td><code>/dg:launch</code></td>
      <td>Launch (materialize) Dagster assets with comprehensive guidance on partitions, configuration, environment setup, and troubleshooting</td>
    </tr>
    <tr>
      <td><code>/dg:logs &lt;run-id&gt; [level] [limit]</code></td>
      <td>Retrieve and display logs for a run</td>
    </tr>
    <tr>
      <td><code>/dg:troubleshoot &lt;run-id&gt;</code></td>
      <td>Debug failing runs by analyzing error logs</td>
    </tr>
  </tbody>
</table>

### dagster-conventions

Comprehensive Dagster development conventions and best practices.

This skill provides expert guidance for Dagster data orchestration including assets, resources,
schedules, sensors, partitions, testing, and ETL patterns.

### dagster-integrations

Comprehensive index of 82+ Dagster integrations including cloud platforms, data warehouses, ETL
tools, AI/ML, data quality, monitoring, and more.

This skill helps you discover and integrate with the right tools for your data pipelines.

### dignified-python

Production-tested Python coding standards with version-aware type annotations, LBYL exception
handling, and modern typing patterns.

This skill provides comprehensive guidance for writing dignified Python code including:

- Automatic Python version detection (3.10-3.13)
- LBYL exception handling patterns
- Modern type syntax (list[str], str | None)
- Pathlib operations and ABC-based interfaces
- CLI patterns and subprocess handling
- API design and code organization best practices

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md).

<div align="center">
  <img alt="dagster logo" src="https://github.com/user-attachments/assets/6fbf8876-09b7-4f4a-8778-8c0bb00c5237" width="auto" height="16px">
</div>
