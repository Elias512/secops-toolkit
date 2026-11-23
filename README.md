# SecOps Toolkit

A collaborative security operations learning and demonstration repository for Kente Logistics.

SecOps Toolkit provides a structured collection of security detection rules, incident response runbooks, synthetic security logs, and supporting resources for practising security operations workflows.

## Project Objectives

The project aims to:

- Organize and maintain security detection rules.
- Document repeatable incident response procedures.
- Provide sample security logs for testing and analysis exercises.
- Practise collaborative security engineering using Git and GitHub.
- Apply repository security and version control best practices.

## Features

### 1. Security Detection Rules

The `detections/` directory contains experimental YAML-based detection rules covering:

- Multiple failed login attempts.
- SSH brute-force activity.
- New administrator account creation.
- Suspicious PowerShell activity.

These rules are examples for learning and development. They are not currently connected to a production SIEM or automated detection engine.

### 2. Incident Response Runbooks

The `runbooks/` directory contains documented response procedures for:

- Account compromise.
- Malware incidents.
- Phishing incidents.

### 3. Synthetic Security Logs

The `samples/` directory contains sample authentication and network logs for security analysis and testing exercises.

All included log samples are synthetic.

### 4. Repository Security

The repository includes:

- CODEOWNERS configuration.
- Pull request templates.
- A security policy.
- GitHub branch protection rules.
- GitHub secret push protection.

## Repository Structure

```text
secops-toolkit/
├── .github/
│   ├── CODEOWNERS
│   └── PULL_REQUEST_TEMPLATE/
│       └── pull_request_template.md
├── detections/
│   ├── multiple_failed_logins.yml
│   ├── new_admin_user.yml
│   ├── ssh_brute_force.yml
│   └── suspicious_powershell.yml
├── runbooks/
│   ├── account_compromise.md
│   ├── malware_response.md
│   └── phishing_response.md
├── samples/
│   ├── auth/
│   └── network/
├── tools/
│   ├── log_analyzer.py
│   └── README.md
├── .gitignore
├── README.md
└── SECURITY.md
```

## Getting Started

### Prerequisites

- Git
- A text editor or IDE
- Python 3 (only if developing Python-based tools)

### Clone the Repository

```bash
git clone git@github.com:Elias512/secops-toolkit.git
cd secops-toolkit
```

Alternatively, clone using HTTPS:

```bash
git clone https://github.com/Elias512/secops-toolkit.git
```

### Explore the Repository

Browse the directories to explore the detection rules, runbooks and sample logs.

The current repository primarily contains documentation, YAML examples and synthetic log files. The Python log analyzer is a placeholder and is not yet implemented.

## Technologies

- Git and GitHub
- Linux
- Python
- YAML
- Markdown

## Contributing

Contributions are welcome.

1. Create a feature branch.
2. Make your changes.
3. Test and review your changes.
4. Commit and push your branch.
5. Open a pull request against `main`.
6. Follow the repository's pull request template.

Please avoid committing credentials, API keys or other sensitive information.

## Security

For information about reporting security vulnerabilities, see [SECURITY.md](SECURITY.md).

## Project Status

Experimental learning and demonstration project.

Detection rules and response procedures require further validation before use in operational environments.

## Disclaimer

This repository is developed for educational and demonstration purposes.

It is not a production SIEM, endpoint detection platform or fully automated security operations solution. All sample logs and security scenarios are synthetic.

Use the detection rules and procedures only after appropriate testing and adaptation to your environment.
