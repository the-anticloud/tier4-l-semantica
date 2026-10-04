# L5 Narrow / L2 General Classification — L_SEMANTICA
**Platform:** Anticloud | **Tier:** TIER_4_INFERENCE_AGENTS | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
L_SEMANTICA provides structured semantic parsing for PAX 27B: it classifies user intent, extracts entities, and identifies query domain before routing. Narrow scope: Anticloud query semantics — clinical, robotics, security, RF, biosignal domains.

## L2 General
L2 General: L_SEMANTICA is the query understanding layer for all tiers. It determines whether a query is clinical, robotics, or security intent and routes accordingly via PAX_ROUTER (TIER_2).

## PAX 27B Integration
PAX 27B provides the deep semantic understanding. L_SEMANTICA combines PAX's semantic output with a structured intent classifier trained on Anticloud domain examples for precise, auditable intent detection.

## AIOSS Audit Chain
Every semantic parse (query hash + intent class + entities hash + confidence + routing decision) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
ISO/IEC 42001 (AI decision transparency). GDPR Art. 22 (automated decision-making audit).
