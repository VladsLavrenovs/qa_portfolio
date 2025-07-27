# Equivalence Class Partitioning (ECP)

**Test Scenario:** Mobile number input field must accept only a 10-digit number.

---

## Classes Identified:

- ✅ **Valid Class**: Any 10-digit number (e.g., `9876543210`)
- ❌ **Invalid Class 1**: Less than 10 digits (e.g., `123456`)
- ❌ **Invalid Class 2**: More than 10 digits (e.g., `123456789012`)
- ❌ **Invalid Class 3**: Contains alphabets/symbols (e.g., `abc123!@#`)

---

## Test Cases:

| Test ID | Input             | Class Type     | Expected Result |
|---------|------------------|----------------|-----------------|
| TC001   | `9876543210`      | Valid          | Accepted        |
| TC002   | `123456`          | Invalid Class 1| Rejected/Error  |
| TC003   | `123456789012`    | Invalid Class 2| Rejected/Error  |
| TC004   | `abc123!@#`       | Invalid Class 3| Rejected/Error  |
