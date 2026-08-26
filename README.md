## Ryan Hartsfield

Cybersecurity and GRC professional building hands-on cloud architecture.

I spent [N] years assessing cloud environments — risk assessments, incident response
planning, BCDR, SOC 2 and HITRUST audits. This portfolio is me building the
architectures I used to evaluate, so I can argue about them from both sides.

Each project is deployed with Terraform, verified with committed scripts rather than
screenshots, documented with the decisions and the alternatives rejected, and destroyed
afterwards.

### Portfolio

| # | Project | Focus | Status |
|---|---|---|---|
| 1 | [aws-secure-static-site](https://github.com/shrimpy215/aws-secure-static-site) | S3 + CloudFront with OAC, security headers, threat model | Complete |
| 2 | [aws-multi-tier-app](https://github.com/shrimpy215/aws-multi-tier-app) | Segmented VPC, no egress from the app tier, SSH replaced by Session Manager | Complete |
| 3 | aws-security-automation | GuardDuty → EventBridge → Lambda automated incident response | In progress |
| 4 | aws-backup-dr | RTO/RPO design, Vault Lock, tested cross-region restore | Planned |
| 5 | aws-landing-zone-lite | Multi-account governance, SCPs, Config aggregation | Planned |
| 6 | aws-ai-findings-analyzer | Bedrock-assisted triage of Security Hub findings | Planned |

### How I build

- Everything in Terraform. Nothing configured by hand in the console.
- Every non-obvious choice recorded with the alternative rejected — see any repo's
  `docs/decisions.md`.
- Failures kept, not deleted. `docs/troubleshooting.md` is part of the deliverable.
- Controls mapped to MITRE ATT&CK, honestly: what a control *prevents* versus what it
  merely *records*.
- Verification committed as scripts, so the claims are reproducible rather than asserted.

**Tools** — Terraform · AWS · Python · GitHub Actions · Checkov

[LinkedIn](your-url) · [email](mailto:rchartsfield@gmail.com)
