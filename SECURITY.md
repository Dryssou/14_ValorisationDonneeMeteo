# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| main    | :white_check_mark: |

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues.**

If you discover a security vulnerability in this project, please report it responsibly:

1. **Email**: Send details to the project maintainers via the contact listed in the repository
2. **GitHub Private Vulnerability Reporting**: Use the "Report a vulnerability" button in the Security tab of this repository

### What to include in your report

- Type of vulnerability (e.g., SQL injection, XSS, CSRF, etc.)
- Full path of the source file(s) related to the vulnerability
- Location of the affected source code (tag/branch/commit or direct URL)
- Step-by-step instructions to reproduce the issue
- Proof-of-concept or exploit code (if possible)
- Impact of the vulnerability

### What to expect

- We will acknowledge receipt of your report within **48 hours**
- We will provide a more detailed response within **7 days**
- We will work to validate and fix the vulnerability
- We will notify you when the fix is deployed

## Security Measures

This project implements the following security practices:

- **Dependency scanning**: Automated with Dependabot and pip-audit
- **SAST**: CodeQL analysis on every push and pull request
- **Container scanning**: Trivy scans all Docker images
- **Secret detection**: Pre-commit hooks prevent secrets from being committed
- **Minimal permissions**: GitHub Actions workflows use least-privilege permissions
- **Pinned dependencies**: GitHub Actions are pinned to specific versions

## Known Issues (VEX)

Vulnerability disclosure information is documented in [vex.json](vex.json) at the root of this repository.
This file follows the OpenVEX specification and documents the exploitability status of known CVEs.
