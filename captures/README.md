# captures/

Evidence captures: primary and derived.

The git repo contains only the counsel-handoff documents (`dossier.md`, `ledger.md`, `charter.md`, `MANIFEST.md`, `AUDIT_LOG.md`, `prior_artifacts.md`, `doj_ada_analysis.md`). The `captures/` directory remains on the operator's local disk because the 628 captured files (168 MB) exceed practical git limits on the capture volume at the time of publication.

**Every capture's URL, HTTP status, byte count, and SHA-256 hash is recorded in `MANIFEST.md` at the repo root.** This allows counsel or any third party to independently re-fetch and verify each primary by hash. Request specific captures from GMRI by sha256 if the manifest is not sufficient.

Tier labels per capture: VERIFIED (primary on disk, hash-verified), VERIFIED-BY-WORKER (worker fetch shown, no disk capture), SECONDHAND (relay/news), UNCONFIRMED (blocked, with reason). See `dossier.md` tier key.
