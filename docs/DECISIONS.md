# 🧠 Technical Decisions – Monthly Email Report Automation

## Scenario Independence

This automation is intentionally independent from other systems to:

- Allow flexible scheduling
- Avoid cross-scenario dependencies
- Simplify maintenance and troubleshooting

---

## Use of Gmail as Data Source

Gmail labels are used as the single source of truth, eliminating the need for:

- External databases
- Synchronization logic
- Redundant data storage

---

## Aggregation Strategy

The automation uses the total number of bundles returned by each query instead of iterating through individual emails.

Benefits:
- Faster execution
- Lower operation cost
- Clear alignment with reporting requirements

---

## Report Format

Plain text is used to ensure:
- Universal compatibility
- Ease of reading
- Simple extensibility

---

## Future Improvements

- Configurable reporting periods
- Multi-recipient distribution
- Export to Airtable or Google Sheets
- Visual dashboards
