**MEMORANDUM**

**TO:** Chief Information Security Officer
**FROM:** Information Security Team
**DATE:** 30 May 2026
**SUBJECT:** Privileged Access Management — Remediation Required; £340K Investment Avoids £2.1M Regulatory Exposure

---

**BLUF:** A 90-day PAM review identified three material gaps — 34% of privileged accounts unreviewed, 12 service accounts with standing admin privileges, and CyberArk covering only 61% of in-scope systems. The IT Risk Committee unanimously endorses a three-phase, £340K remediation programme to close these gaps and avoid up to £2.1M in GDPR/NIS2 penalties.

---

**SITUATION**

The Information Security team, supported by Meridian Security Partners, completed a 90-day review of the organisation's privileged access management posture following Q1 audit findings. The review covered 847 privileged accounts, 23 system owner interviews, and a technical assessment of the existing CyberArk deployment.

**FINDINGS**

Three gaps were identified:

1. **Account reviews overdue.** 34% of privileged accounts (approximately 288) have not been reviewed in over 12 months, creating material risk exposure.
2. **Standing admin privileges on service accounts.** 12 service accounts retain permanent admin access contrary to just-in-time (JIT) guidance.
3. **Incomplete CyberArk coverage.** The current deployment covers only 61% of in-scope systems; the remaining 39% are legacy systems in the manufacturing division excluded from the original scope.

**RECOMMENDATION**

Approve the three-phase remediation programme:

| Phase | Timeframe | Action |
|-------|-----------|--------|
| 1 | 0–30 days | Complete access reviews for all 847 accounts; revoke unnecessary privileges |
| 2 | 30–90 days | Implement JIT access for 12 service accounts; extend CyberArk to remaining 39% of systems |
| 3 | 90–180 days | Deploy behavioural analytics to detect anomalous privileged access patterns |

**Total cost:** £340K over six months.

**Without action:** Regulatory penalties under GDPR and NIS2 could reach £2.1M.

**COORDINATION**

The IT Risk Committee has reviewed and unanimously endorsed this recommendation.

**ACTION REQUIRED:** CISO approval to proceed to Phase 1.
