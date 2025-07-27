# Decision Table Testing

**Test Scenario:** Determine whether a user gets a discount based on age and membership.

---

## Rules:

- Users aged **60 or older** get a discount.
- **Premium members** get a discount regardless of age.
- All others do **not** get a discount.

---

## Decision Table:

| Condition                     | Rule 1 | Rule 2 | Rule 3 | Rule 4 |
|-------------------------------|--------|--------|--------|--------|
| Age ≥ 60                      | ❌     | ❌     | ✅     | ✅     |
| Is Premium Member?            | ❌     | ✅     | ❌     | ✅     |
| **→ Discount Applied?**       | ❌     | ✅     | ✅     | ✅     |

---

## Test Cases:

| Test ID | Age | Member | Expected Outcome  |
|---------|-----|--------|-------------------|
| TC001   | 45  | No     | No Discount       |
| TC002   | 45  | Yes    | Discount Applied  |
| TC003   | 60  | No     | Discount Applied  |
| TC004   | 65  | Yes    | Discount Applied  |
