# Campus Automation System (MARVEL)

Comprehensive Campus Automation System for college management, student services, attendance tracking, and administrative workflows.

## Architecture & Repository Structure

This repository is the parent workspace and orchestrator for the Campus Automation System, incorporating the core application as a Git submodule:

```
Campus-Automation-System/
├── MARVEL-main/                     # Core application submodule (FastAPI backend + Express frontend)
│   ├── backend/                     # FastAPI backend (endpoints, ORM models, auth, migration engine)
│   ├── frontend/                    # Express.js frontend server & web interface
│   ├── alembic/                     # Database schema migrations
│   └── docs/                        # Architecture documentation & migration audits
├── logs/                            # Local application & test logs
└── test.db                          # Local development SQLite database fixture
```

## Technology Stack

- **Backend:** Python 3.12, FastAPI, SQLAlchemy 2.0, Pydantic v2, SQLite / PostgreSQL 16+
- **Frontend:** Node.js, Express.js, TailwindCSS, Vanilla JS UI components
- **Database Architecture:** Dual-engine SQLite & PostgreSQL cross-dialect support with topological migration planning and TLVE binary integrity verification

## Documentation

Comprehensive architecture specifications, data quality audits, and migration designs are located in `MARVEL-main/docs/`:
- `MARVEL-main/docs/database/PHASE_19F_1_DATA_MIGRATION_ARCHITECTURE_AUDIT.md`: Complete 22-table data audit and type conversion matrix.
- `MARVEL-main/docs/database/PHASE_19F_2_A_MIGRATION_ENGINE_FOUNDATION.md`: Cross-dialect migration engine foundation architecture.
- `MARVEL-main/docs/database/PHASE_19F_2_A_FINAL_IMPLEMENTATION_PLAN.md`: Final corrected implementation plan (Phase 19F.2-A-C).
