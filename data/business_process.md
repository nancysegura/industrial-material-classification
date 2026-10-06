# Business Process

## Business Context

Industrial organizations may accumulate material records that are unclassified or inconsistently classified due to process gaps, historical data accumulation, incomplete information, or inconsistent material descriptions.

Correcting these records can require significant manual effort,
especially when large historical backlogs need to be reviewed.

---

## AS-IS Process

```mermaid
flowchart TD
    A[Material Created or Acquired] --> B[Engineering / Business Review]
    B --> C{Category Assigned?}

    C -->|Yes| D[Material Classified]
    C -->|No| E[Unclassified Record]

    E --> F[Data Quality Backlog]

  ```  