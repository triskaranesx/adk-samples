# ADK Samples

A collection of sample agents and applications built with [Google Agent Development Kit (ADK)](https://google.github.io/adk-docs/).

> This is a fork of [google/adk-samples](https://github.com/google/adk-samples).

## Overview

This repository contains ready-to-use sample agents demonstrating various capabilities of the Agent Development Kit (ADK). Each sample is self-contained and includes setup instructions, dependencies, and example usage.

## Prerequisites

- Python 3.11+
- [Google ADK](https://pypi.org/project/google-adk/) (`pip install google-adk`)
- A Google Cloud project with the necessary APIs enabled
- Valid credentials (Application Default Credentials or a service account key)

## Repository Structure

```
adk-samples/
├── agents/                  # Individual agent samples
│   ├── README.md
│   └── <agent-name>/
│       ├── README.md
│       ├── pyproject.toml
│       └── <agent_name>/
│           ├── __init__.py
│           └── agent.py
├── .github/                 # GitHub Actions, templates, and Terraform configs
└── README.md
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/<your-org>/adk-samples.git
cd adk-samples
```

### 2. Set up authentication

```bash
gcloud auth application-default login
```

### 3. Navigate to a sample agent

```bash
cd agents/<agent-name>
```

### 4. Install dependencies

```bash
pip install -e .
```

### 5. Run the agent

```bash
adk run <agent_name>
```

Or launch the interactive web UI:

```bash
adk web
```

## Available Samples

| Agent | Description |
|-------|-------------|
| *(more coming soon)* | |

## Contributing

Contributions are welcome! Please read the [contribution guidelines](.github/ISSUE_TEMPLATE/bug_report.md) and open an issue or pull request.

### Adding a New Sample

1. Create a new directory under `agents/<your-agent-name>/`.
2. Follow the existing agent structure (see `agents/README.md`).
3. Include a `README.md` with setup and usage instructions.
4. Add tests where applicable.
5. Open a pull request against the `main` branch.

## License

This project is licensed under the Apache 2.0 License — see the [LICENSE](LICENSE) file for details.
