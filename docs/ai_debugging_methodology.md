# AI-Assisted Debugging Methodology

## Approach

Instead of directly applying fixes, AI was used to understand why failures occurred.

Each debugging cycle followed the same process:

Error
↓
Log Analysis
↓
AI Interpretation
↓
Manual Verification
↓
Fix Implementation
↓
Re-run OpenLane

---

## Errors Investigated

### Missing AMUX2_3V

Root Cause:

Required analog macro files were not correctly referenced.

---

### Duplicate spi_slave Definition

Root Cause:

The same module was declared multiple times.

---

### IO vs I0 Naming Error

Root Cause:

Incorrect signal naming caused module connectivity issues.

---

### Synthesis Failures

Root Cause:

Configuration inconsistencies and unresolved design dependencies.

---

## Observation

AI accelerated debugging by narrowing the search space and explaining potential root causes.

However, all fixes were manually validated before implementation.
