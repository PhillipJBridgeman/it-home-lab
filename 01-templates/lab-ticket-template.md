
---

## `01-templates/lab-ticket-template.md` (ticket template)

```md
# LAB-ID — Title (Tier 1 Support Ticket)

## Ticket Information
- **Ticket ID:** LAB-______
- **Category:** Hardware / OS / Networking / Security / Software / Peripherals
- **Priority:** Low / Medium / High
- **Status:** Open / In Progress / Resolved / Escalated
- **Date Opened:** YYYY-MM-DD
- **Date Closed:** YYYY-MM-DD
- **Environment:** Home Lab (Learning)
- **Device / OS:** (e.g., Windows 11 Pro, version/build)
- **User Context:** (single user, multi-user, office/home, etc.)

---

## User Report (as the user said it)
> “Write the issue exactly how a user would describe it.”

---

## Scope & Impact
- Who is affected?
- What is broken (specific app/system/service)?
- Any time sensitivity?

---

## Initial Triage Questions (Tier 1 Script)
- When did it start? Any recent changes?
- Is it happening for other users/devices?
- Is it intermittent or constant?
- Exact error message? (Request screenshot)
- Wired or Wi-Fi? On VPN?

---

## Environment Details
- **Network:** (wired/wireless, SSID, router/switch info if relevant)
- **Account Type:** (standard/admin, local/Microsoft account)
- **Recent Changes:** (updates, installs, hardware changes)
- **Related Devices:** (printer, dock, headset, monitor, USB device)

---

## Troubleshooting Log (Steps + Results)

### Step 1 — Quick Checks (safe, reversible)
- Action:
- Result:
- Notes:

### Step 2 — Verify Configuration / Status
- Tool / location used (GUI/CLI):
- Output / observations:
- Result:

### Step 3 — Isolate the Cause
- What did I rule out?
- What remains likely?

### Step 4 — Fix Attempt(s)
- Change made:
- Result:

---

## Root Cause
Describe the underlying cause in clear terms.

---

## Resolution
- Final fix applied:
- Commands/settings changed:
- Any rollback performed:

---

## Validation (Proof it’s fixed)
- What I tested:
- Expected result:
- Actual result:

---

## Prevention / Recommendations
- User guidance:
- Configuration hardening:
- Runbook update needed?

---

## Escalation Notes (if applicable)
- Why escalation would be needed:
- What evidence/logs Tier 2 would need:
- What I would recommend next:

---

## Evidence
Attach references to files you saved in `evidence/` and `artifacts/`:
- `evidence/screenshot-01.png` — (what it shows)
- `artifacts/commands-used.md` — (commands & outputs)
- `evidence/eventviewer-error.txt` — (event ID / message)

---

## Lessons Learned
- What I’d do faster next time:
- What checks mattered most:
