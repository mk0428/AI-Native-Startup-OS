# Pre-Launch Checklist

> Every product must pass this checklist before any real user touches it.
> Orchestrator audits. Founder reviews findings. Both sign off.

---

## ☐ 1. Security Audit

### Authentication & Authorization
- [ ] Authentication is implemented correctly (no bypass)
- [ ] Session tokens are properly generated, stored, and expired
- [ ] Authorization checks exist on every protected endpoint
- [ ] No hardcoded credentials, API keys, or secrets in source code
- [ ] Secrets managed via environment variables or secret store

### Data Protection
- [ ] User data is not exposed in API responses beyond what's needed
- [ ] Personal data is encrypted at rest if stored
- [ ] No logging of sensitive data (passwords, tokens, API keys)
- [ ] CORS configuration restricts allowed origins

### Input Validation
- [ ] All user inputs are validated server-side (not just client-side)
- [ ] No SQL/NoSQL injection vectors in any query
- [ ] File uploads are validated: type, size, content scanning
- [ ] No command injection vectors

### Dependencies
- [ ] Dependencies scanned for known vulnerabilities
- [ ] No deprecated packages with known CVEs
- [ ] Lock file is up to date

## ☐ 2. Cost Verification

- [ ] API cost per user action is calculated and matches SCOPE.md projections
- [ ] Infrastructure cost per user/month is calculated
- [ ] Break-even user count is realistic
- [ ] Free tier costs are sustainable (not just "it'll work out")
- [ ] Payment processing fees included in unit economics

## ☐ 3. Monitoring & Observability

- [ ] Health endpoint exists and returns meaningful status
- [ ] Error logging is in place (failed requests, exceptions, timeouts)
- [ ] Server/process restart on failure is configured (systemd, supervisor, etc.)
- [ ] Resource monitoring basics: CPU, memory, disk usage triggers
- [ ] Cost monitoring: API usage tracked, spending alerts configured

## ☐ 4. Deployment

- [ ] Deployment is reproducible (scripted, not manual steps)
- [ ] Rollback plan exists and is tested
- [ ] DNS/SSL configured correctly (HTTPS enforced)
- [ ] Environment variables for production are set (not local values)
- [ ] Firewall/network rules restrict access appropriately

## ☐ 5. Production Readiness

- [ ] Rate limiting is configured (prevent abuse of free tier)
- [ ] Error pages are user-friendly (no stack traces exposed)
- [ ] Privacy policy is available and linked
- [ ] Terms of service are available (if accepting users)
- [ ] Contact/support channel exists

## ☐ 6. Pre-Launch Data

- [ ] Metrics tracking is in place before users arrive
- [ ] Activation criteria defined
- [ ] Day 7 / Day 30 retention targets set
- [ ] False positive signals identified (what looks good but isn't)

---

### Sign-off

| Area | Auditor (Orchestrator) | Reviewer (Founder) | Date |
|------|----------------------|-------------------|------|
| Security | ☐ Pass | ☐ Reviewed | |
| Cost | ☐ Pass | ☐ Reviewed | |
| Monitoring | ☐ Pass | ☐ Reviewed | |
| Deployment | ☐ Pass | ☐ Reviewed | |
| Production | ☐ Pass | ☐ Reviewed | |
| Metrics | ☐ Pass | ☐ Reviewed | |
| **Final** | **☐ Go** | **☐ Go** | |

*One NO across any category → Pause launch. Fix before proceeding.*
