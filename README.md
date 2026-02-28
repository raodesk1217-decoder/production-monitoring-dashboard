## 🧮 DAX Measures Used

The following DAX measures were created to calculate dynamic KPIs:

- **Efficiency %**
- **Rejection %**
- **Variance %**
- **Production Variance**

Example DAX Logic:

```DAX
Efficiency % = DIVIDE([Good Qty], [Actual Qty])

Rejection % = DIVIDE([Rejection Qty], [Actual Qty])

Variance % = DIVIDE([Actual Qty] - [Planned Qty], [Planned Qty])
