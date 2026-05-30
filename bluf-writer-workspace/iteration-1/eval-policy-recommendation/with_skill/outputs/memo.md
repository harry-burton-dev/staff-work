MEMORANDUM FOR Chief Information Security Officer

FROM:    Information Security Team
DATE:    30 May 2026
SUBJECT: Approve £340K PAM Remediation Programme to Close Critical Access Control Gaps

1. BLUF. The organisation's privileged access management posture contains three material control failures — unreviewed accounts, standing admin privileges, and incomplete CyberArk coverage — exposing the organisation to up to £2.1M in regulatory penalties; the IT Risk Committee recommends a £340K, six-month remediation programme requiring CISO approval to proceed.

2. BACKGROUND. A 90-day review of privileged access management, conducted by Information Security with support from Meridian Security Partners, examined 847 privileged accounts and assessed the existing CyberArk deployment following Q1 audit findings. The review identified gaps significant enough to warrant a structured remediation programme.

3. DISCUSSION.
   a. 34% of privileged accounts (approximately 288) have not been reviewed in over 12 months, creating direct exposure to the Q1 audit findings.
   b. 12 service accounts retain standing admin privileges in breach of just-in-time (JIT) access guidance — each one an unmitigated lateral movement risk.
   c. CyberArk covers only 61% of in-scope systems; the remaining 39% are legacy manufacturing systems excluded from the original deployment.
   d. Unmitigated, these gaps carry regulatory penalty exposure of up to £2.1M under GDPR and NIS2.
   e. The proposed three-phase programme addresses all findings: access reviews (0–30 days), JIT implementation and CyberArk extension (30–90 days), and behavioural analytics deployment (90–180 days).
   f. Total programme cost is £340K — a 6:1 return on risk reduction against maximum penalty exposure.

4. RECOMMENDATION. Approve the three-phase PAM remediation programme at a cost of £340K.
   a. Phase 1 (by 30 Jun 26): Information Security to complete access reviews for all 847 accounts and revoke unnecessary privileges.
   b. Phase 2 (by 30 Aug 26): Information Security to implement JIT for 12 service accounts and extend CyberArk to remaining in-scope systems.
   c. Phase 3 (by 30 Nov 26): Information Security to deploy behavioural analytics for anomalous privileged access detection.

5. POC. Information Security Team — see sender above.
