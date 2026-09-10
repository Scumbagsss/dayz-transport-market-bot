# DayZ Transport Market Bot

> **Portfolio showcase — production source is private and this repository is intentionally non-runnable.**

Moderated Discord vehicle marketplace with ownership registry, listings, reservations and complaints.

## What it demonstrates

- Market rules and access role
- Sell/buy/rent forms
- Ownership registry
- Staff moderation
- Approved listing publication
- Reservation and close actions
- Complaint workflow
- Blacklist, logs and archive

## Technology

Python • discord.py 2.x • SQLite/WAL • Persistent Views • Discord Modals

## High-level workflow

1. Player chooses market action
2. Validate access/ownership state
3. Create moderated application
4. Staff approves or rejects
5. Publish and manage listing lifecycle

## Public interface preview

The public skeleton exposes only the architectural surface:

- `submit_market_application(...)`
- `validate_registry_state(...)`
- `review_application(...)`
- `publish_listing(...)`
- `reserve_listing(...)`
- `close_listing(...)`

The production implementations behind these methods are withheld. See [`NOTICE.md`](NOTICE.md).

## Repository contents

- `src/public_interface.py` — non-runnable interface skeleton;
- `docs/ARCHITECTURE.md` — high-level design;
- `examples/config.example.jsonc` — sanitized configuration shape;
- `LICENSE` — explicit all-rights-reserved notice.

## Status

Production-tested private project / portfolio edition.
