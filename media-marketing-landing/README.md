# PointSav Showcase: media-marketing-landing
### *The Autonomous Edge Node & Cookieless Intelligence Loop*

**Status: Active Sandbox** | **Substrate: os-mediakit**

## 📜 Mandate
This deployment operates as the public-facing edge node for PointSav Digital Systems™. It mathematically proves the Autonomous Edge Node architecture. The presentation layer (`app-mediakit-knowledge`) and the telemetry ingestion engine (`app-mediakit-telemetry`) coexist within a strictly isolated, 100% portable Linux userspace.

> **DATA SOVEREIGNTY POSTURE:** This userspace acts as a self-contained micro-vault. It enforces DS-ADR-06 (Zero-State Telemetry) by masking IPs in memory and writing directly to a local flat-file ledger. Zero data is transmitted to third-party cloud analytics.

## 🏛️ Autonomous Userspace Architecture
This directory visually maps the live execution environment running on `cluster-totebox-corporate-1` under the `svc-mediakit-pointsav` service account.

    USERSPACE: svc-mediakit-pointsav
    ├── app-mediakit-knowledge/             <-- (Zero-Execution Static Assets)
    │   └── pointsav-monolith.html          <-- (System Monolith Aesthetic | DS-ADR-08)
    │
    ├── app-mediakit-telemetry/             <-- (Stateless Rust HTTP Server | Port 8081)
    │
    ├── assets/                             <-- (Local Micro-Vault | Write-Only)
    │   ├── GeoLite2-City.mmdb              <-- (Offline Geolocation Database)
    │   └── ledger_telemetry.csv            <-- (Pre-Resolved Data Target)
    │
    └── outbox/                             <-- (4:00 AM Synthesizer Egress)
        └── REPORT_POINTSAV_TIMESTAMP.md

---
*© 2026 PointSav Digital Systems™.*
