# Qmoosa Shield — Internal Evidence Report

Generated: `2026-10-02T15:58:22.168Z`  
SHA-256: `022dad84004c90a88df8cd9953119764db242b5abec5eb1cf36e536cdfc5a5cc`  
ML-DSA signature length: `3309 bytes`

## Repository checks executed

- truth/status verification
- TypeScript type checking
- application-layer ML-KEM / ML-DSA integration checks
- repository-defined adversarial cases
- RFC 5869 HKDF known-answer test
- repository-internal reality gates

## Important boundary

The current Express `/api/pqc/handshake` uses real X25519 and HKDF but
**does not implement ML-KEM on the server**. It uses explicitly labeled
PQ-shaped placeholder data.

## Limitations

This report is created and signed by this repository. It is **not**:

- an independent security or cryptographic audit;
- FIPS validation of Qmoosa Shield as a module;
- proof of official NIST PQC KAT/ACVP vector execution;
- proof that Project Wycheproof vectors were imported;
- a production-readiness certificate.

The ML-DSA signature authenticates the generated report only.
