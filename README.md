# GateBill Enterprise — Official Releases

This repository hosts the official standalone single-binary production executables (GateBill.exe) and cryptographic SHA-256 checksums for the **GateBill Enterprise ISP Billing, Accounting & Subscription Management System**.

## Single-Binary Architecture
Each GateBill.exe release is a self-contained executable that embeds:
- **Backend Server**: Go REST API & background schedulers
- **Frontend SPA**: Production React bundle
- **Database Migrations & Seed**: Embedded SQL schema migrations (migrations/*.sql) and initial seed data (db/seed.sql)
- **Release Metadata**: Full version & changelog manifest (ersion.json)

## Online Self-Update
GateBill servers automatically check this repository's [Releases](https://github.com/virusworld/GateBill-Releases/releases) and [latest.json](./latest.json) manifest to provide 1-click online updates directly from the GateBill Dashboard and About dialog.
