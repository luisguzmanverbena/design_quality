# Evaluation Personas

## 1. The Administrator
**Daily Operator**

Manages Vault itself — clusters, namespaces, auth methods, policies, replication, upgrades. CLI/Terraform-native, uses the UI for monitoring and debugging.

- **Primary goal:** Confirm cluster health and take operational action without leaving the page.
- **Frustration trigger:** Having to navigate elsewhere to answer basic operational questions (seal status, replication, standby count).
- **Interaction pattern:** Daily visits. Scans for anomalies, then drills into specifics. Wants a control room, not a spec sheet.
- **Dimensions:** Model & Feedback, Risk Audit, Leverage & Autonomy

---

## 2. The Secret Consumer
**Application Developer**

Needs secrets for their app. Doesn't care how Vault works internally — just wants credentials delivered reliably. Explores via UI, automates via SDK/API.

- **Primary goal:** Get to secrets or configure their app to retrieve them. Cluster details are irrelevant.
- **Frustration trigger:** Landing on an infrastructure page when their job is "get a secret." Being shown actions they can't perform.
- **Interaction pattern:** Occasional UI visits during setup. Once automated, never returns. The overview page is a waypoint, not a destination.
- **Dimensions:** Model & Feedback, Reduction & Necessity, Leverage & Autonomy

---

## 3. The Governance & Compliance Owner
**Security / Policy Lead**

Enforces access control, audits access patterns, ensures rotation policies are met. Needs to verify permissions, trace events, and produce compliance evidence.

- **Primary goal:** Assess security posture at a glance — who has access, what's exposed, is the audit trail intact.
- **Frustration trigger:** Risky configurations presented as neutral facts. High-privilege actions without governance context or audit visibility.
- **Interaction pattern:** Periodic reviews. Needs to quickly determine "is this cluster configured securely?" and export evidence.
- **Dimensions:** Risk Audit, Model & Feedback, Leverage & Autonomy

---

## 4. The CI/CD Integrator
**Platform / DevOps Engineer**

Wires Vault into pipelines — dynamic credentials, lease management, secret injection at deploy time. Lives in automation, hits the UI when things break.

- **Primary goal:** Get the connection details and auth method guidance needed to configure a pipeline.
- **Frustration trigger:** Being guided toward manual/admin auth patterns (token generation) when machine auth (AppRole, K8s) is the correct approach.
- **Interaction pattern:** One-time setup visit, then rare debugging visits. Needs the page to accelerate automation, not assume manual interaction.
- **Dimensions:** Leverage & Autonomy, Risk Audit, Model & Feedback

---

## 5. The Newcomer
**First-Time User**

First encounter with Vault. Needs to build a mental model of tokens, policies, auth methods, and secret engines without breaking anything. UI-dependent, documentation-dependent.

- **Primary goal:** Understand what this cluster is, what they can do with it, and what to do first.
- **Frustration trigger:** Unexplained domain terms (HVN, HA, replication). High-consequence actions without educational guardrails.
- **Interaction pattern:** Exploratory. Reads everything. Afraid to click destructive-looking actions. Needs progressive disclosure and sequenced guidance.
- **Dimensions:** Model & Feedback, Reduction & Necessity, Risk Audit

---

## 6. The Infrequent Overseer
**Engineering Manager / Team Lead**

Checks in weekly or monthly — reviews access patterns, approves policy changes, tracks adoption. Re-learns the interface every visit.

- **Primary goal:** Answer "is this cluster healthy, secure, and being used correctly?" in under 30 seconds.
- **Frustration trigger:** No temporal context — no activity, no trends, no "what changed since last time." Static facts don't support oversight.
- **Interaction pattern:** Infrequent, scan-heavy. Needs the page to surface what matters without requiring deep navigation.
- **Dimensions:** Model & Feedback, Leverage & Autonomy, Reduction & Necessity
