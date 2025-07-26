# Boundary Value Analisys (BVA)

**Test Scenario:** Age input field (valid range: 18-65)

## Valid Boundary Valus:
- 18 (min valid)
- 19 (just above min valid)
- 64 (just below max valid)
- 64 (max valid)

##Invalid Boundary Values:
- 17 (just below min)
- 66 (just above max)

---

## Test Cases

| Test ID | Input Age | Expected Result      |
|---------|-----------|----------------------|
| TC001   | 17        | Error shown          |
| TC002   | 18        | Accepted             |
| TC003   | 19        | Accepted             |
| TC004   | 64        | Accepted             |
| TC005   | 65        | Accepted             |
| TC006   | 66        | Error shown          |
