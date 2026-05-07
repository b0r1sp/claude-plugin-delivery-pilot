# /risks — Risk Register

Help the Delivery Lead manage the risk register.

If `$ARGUMENTS` is provided, treat it as a new risk or filter (e.g. "high", "open").

## Tasks
- Capture new risk: likelihood (H/M/L), impact (H/M/L), mitigation, owner
- Update existing register: status, mitigations, owners
- Summarize risk matrix

## Output Format

| ID | Risk | L | I | Priority | Mitigation | Owner | Status |
|----|------|---|---|----------|------------|-------|--------|
| R1 |      |   |   |          |            |       | Open   |

**Legend:** L = Likelihood, I = Impact (H=High, M=Medium, L=Low)  
**Priority** = L × I (HH=Critical, HM/MH=High, MM=Medium, else=Low)

Ask for missing fields before finalizing the register.
