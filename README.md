# Jayce Hill

**Principal AI Security Architect** · I build and secure agentic AI systems — threat modeling, MCP and tool-call security, non-human identity, and cloud security architecture.

20+ years across national security and enterprise: offensive and defensive work for DoD, ATO and continuous monitoring for classified cloud systems, and five years as a Principal Engineer in Microsoft's Industry Solutions Engineering group, where I co-led CRISP (MCP-based threat modeling, 100+ enterprise engagements) and was security lead on HVE-Core (a 34-agent engineering platform).

---

### 🔐 Featured: Secure MCP Execution Runtime
A zero-trust control plane for AI agent tool calls → **[jaycehilleng.github.io](https://github.com/jaycehilleng/jaycehilleng.github.io)**

| Layer | What it does | Status |
| :--- | :--- | :--- |
| `SecureMCPProxy` | Policy enforcement point: verified caller identity, tool-level RBAC, recursive argument sanitization (CWE-88, path traversal, command chaining), structured telemetry | Implemented · CI |
| `PoPTokenValidator` | ES256 signature verification (rejects forged and `alg: none` tokens), 15-min TTL, audience, scope, RFC 7800 `cnf` binding | Implemented · CI |
| OPA / Rego policy | Default-deny tool authorization | Authored · sidecar wiring next |
| Azure IaC | Container Apps (private ingress), APIM `validate-jwt` + out-of-band inspection, KQL detections | Implemented |
| Execution sandboxing | gVisor / Wasm isolation for tool runtimes | Designed |

### 🧭 Now building
- Per-request DPoP proof verification (RFC 9449)
- FastAPI inspection endpoint + one-command Docker demo
- Prompt-injection evaluation suite with published block / false-positive rates

### 🛠 Toolbox
Python · Azure (Solutions Architect Expert) · AWS · Bicep / Terraform · OPA/Rego · Entra ID · Defender XDR / Sentinel / KQL · MITRE ATT&CK · OWASP Top 10 for LLM · NIST AI RMF · FedRAMP / DoD IL4–6 / ICD 503

### 📫 Contact
[hillsecadvisors.com](https://hillsecadvisors.com) · [LinkedIn](https://www.linkedin.com/in/jaycehilleng/) · jayce@hillsecadvisors.com
