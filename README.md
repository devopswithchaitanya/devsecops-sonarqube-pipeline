# 🔒 DevSecOps Pipeline — SonarQube + OWASP + Trivy

A complete DevSecOps CI/CD pipeline integrating static code analysis, dependency scanning, and container vulnerability scanning. Security is shifted left — every commit is scanned automatically.

## Security Stages

```
Code Push
    │
    ├── SonarQube SAST (Static Code Analysis)
    ├── OWASP Dependency Check (CVE scanning)
    ├── Trivy (Container image vulnerability scan)
    ├── Quality Gate (fail if critical issues found)
    └── Deploy only if all gates pass ✅
```

## Setup

```bash
# Start SonarQube locally
docker-compose -f docker-compose-sonar.yml up -d
# Access: http://localhost:9000 (admin/admin)
```

## Tools

| Tool | Purpose |
|------|---------|
| SonarQube | SAST — code quality & security |
| OWASP Dependency Check | Known CVEs in dependencies |
| Trivy | Container image vulnerabilities |
| GitHub Actions | Pipeline orchestration |

## Tech Stack
`SonarQube` `OWASP` `Trivy` `GitHub Actions` `Jenkins` `Docker`
