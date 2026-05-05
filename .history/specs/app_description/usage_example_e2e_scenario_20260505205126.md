# Usage Example — End-to-End Scenario

## Users
- You (User A)
- Partner (User B)

---

## 1. Add Simple Expense

**Input**
80 pizza dinner

**System flow**
- Parse: amount=80, note="pizza dinner"
- Classify: Food (rule: “pizza”)
- Open UI:

You paid by default

Split:
You        40  
Partner    40  

Category: Food (auto)

**Result stored**
- amount: 80
- payer: You
- split_you: 40
- split_partner: 40
- category: Food

---

## 2. Add Unequal Expense

**Input**
120 groceries

**User edits split in UI**
You        90  
Partner    30  

**Result**
Partner owes you 30

---

## 3. Balance Calculation

- Pizza → Partner owes 40
- Groceries → Partner owes 30

**Net balance**
Partner owes you 70

---

## 4. Budget Warning

Food limit = 200

After expenses:
- 80 + 120 = 200

System shows:
⚠️ Food budget reached 100%

---

## 5. Edit Expense

Edit groceries:
- amount: 120 → 100
- split auto-adjusted

New split:
You        75  
Partner    25  

New balance:
Partner owes you 65

---

## 6. Search Notes

Search: “dinner”

Returns:
- pizza dinner

---

## 7. Delete Expense

User selects:
☑ pizza dinner

Action: Delete Selected

System:
- soft delete applied
- balance recalculated

New balance:
Partner owes you 25

---

## 8. Dashboard View

Shows:
- Balance: Partner owes you 25
- Budget: Food 125 / 200
- Pie chart: Food dominant
- Trend: spending over time

---

## 9. Settlement

Click: Settle Up

System:
- net balance = 25
- creates settlement transaction

Result:
Balance = 0

---

## 10. New Expense After Settlement

50 taxi

Split:
25 / 25

New balance:
Partner owes you 25

---

## Key Outcome

The system demonstrates:
- fast expense entry
- UI-driven splitting (Splitwise-like)
- rule-based classification
- ledger-based correctness
- budget enforcement
- full edit/delete capability
- settlement reset cycle