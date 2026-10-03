# Antigravity AWS Plugin

This plugin integrates AWS skills and an AWS MCP server into your Antigravity agent, giving it the ability to interact directly with AWS services and infrastructure.

## Features

- Configures the `aws-mcp` Model Context Protocol (MCP) server.
- Includes 24 pre-built AWS skills for Antigravity, such as:
  - `amazon-bedrock`
  - `aws-compute`
  - `aws-database`
  - `aws-iam`
  - `aws-serverless`
  - ...and more!

## Requirements

- Python's `uv` command-line tool (to run `uvx`).
- Valid AWS credentials configured in your environment.
- Antigravity AI agent.

## Installation

You can install this plugin into your Antigravity plugins directory:

```bash
cd ~/.gemini/config/plugins/
git clone <repository-url> aws-plugin
```

## Permissions

For safety, plugins cannot self-grant access. Ensure you have authorized the `aws-mcp` server. Your Antigravity instance may prompt you for permission on first use.

## Publishing

If you want to publish this to GitHub:

```bash
cd ~/.gemini/config/plugins/aws-plugin
git init
git add .
git commit -m "Initial commit of AWS plugin"
gh repo create aws-plugin --public --source=. --remote=origin --push
```
