# Police Accountability & Discovery Audit Engine

Open-source Python accountability engine for defense counsel and transparency advocates. Ingests institutional records and police disclosure logs into a tamper-evident, SHA-256 cryptographic chain of custody via SQLite. A zero-dependency, mobile-first tool ensuring absolute record integrity and verifiable counter-surveillance oversight.

---

## Overview

The **Police Accountability Engine** is a lightweight Python utility designed to help defense counsel and civil rights advocates ingest, secure, and verify the integrity of institutional records, police disclosure logs, and investigative timelines. 

By applying cryptographic parent-child hashing chains (SHA-256) stored in a local SQLite ledger, this tool creates a tamper-evident audit trail that instantly flags backdated files, missing notes, or altered records.

### Key Features:
1. **Zero-Dependency Core:** Built using pure Python 3 standard libraries (`sqlite3`, `hashlib`, `csv`).
2. **Cryptographic Chaining:** Each record links directly to the hash of the preceding entry, making silent deletions mathematically impossible.
3. **Bulk CSV Ingestion:** Quickly ingest raw disclosure dumps or public oversight logs to verify chain integrity across hundreds of data points.

---

## Quick Start

Run the audit engine locally in your terminal:
```bash
python main.py
