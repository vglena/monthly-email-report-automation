# 🧱 Architecture – Monthly Email Report Automation

## Overview

This automation is designed to generate a **periodic email report** based on Gmail labels.

Each label represents a classification category, and Gmail itself acts as the data store.  
The system performs read-only operations and produces a summarized output.

---

## High-Level Flow

1. Execute Gmail search queries for each target label
2. Retrieve the total number of matching emails
3. Aggregate counts across categories
4. Generate a human-readable report
5. Deliver the report via email

---

## Design Characteristics

- Stateless execution
- No external database required
- Clear separation between data retrieval and presentation
- Minimal operational cost

---

## Output

The final output is a plain-text email report summarizing email volumes per category.
