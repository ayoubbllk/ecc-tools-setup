# Security Policy

## ECC Security Audits

This repository uses Enterprise Code Cohesion (ECC) tools with AgentShield-backed security scanning.

### Audit Scope

The following areas are audited for security and compliance:

1. **Agent Configurations** - Validates agent setup and permissions
2. **Git Hooks** - Scans for malicious or problematic hooks
3. **Repository Rules** - Ensures compliance with defined patterns
4. **MCP Settings** - Validates Model Context Protocol configurations

### Security Features

- **Automated Scanning**: Continuous checks on PR and manual trigger via `/ecc-tools audit`
- **Risky Change Detection**: Identifies dangerous modifications to agent configs, hooks, rules, and MCP settings
- **Safe Repair Planning**: Suggests fixes without automatic application
- **Manifest-Driven Management**: Configuration-based approach for safety

### Audit Commands

- `/ecc-tools audit` - Run full security audit
- `/ecc-tools doctor` - Health check with issues
- `/ecc-tools repair` - Plan repairs with uninstall guidance

### Private Repository Support

This configuration supports private repository security scanning with appropriate authentication.

### Reporting Issues

If you discover a security vulnerability, please report it to the repository maintainers immediately. Do not create public issues for security vulnerabilities.

## Compliance

All hosted workflows follow GitHub's security best practices:
- Minimal required permissions
- Environment-based secrets management
- Audit logging for all operations

For more information, see the ECC documentation or contact the security team.
