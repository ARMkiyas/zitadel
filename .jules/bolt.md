## 2026-05-21 - [Event Push Loop Optimization]
**Learning:** `fmt.Sprintf` creates significant overhead in hot loops compared to direct string concatenation in Go, especially around string casting.
**Action:** Always favor string concatenation (`+`) over `fmt.Sprintf` when dealing with simple string constructions in loops for performance-critical backend paths like event pushing.
