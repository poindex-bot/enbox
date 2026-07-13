---
"@enbox/api": patch
---

chore: republish to re-pin internal dependencies (@enbox/agent 0.8.23, @enbox/dwn-sdk-js 0.4.12, @enbox/dids 0.1.6 → @enbox/crypto 0.1.6) so consumers resolve a single dependency graph that includes the AES-KW WebCrypto fallback (#1270, #1272). `workspace:*` pins only refresh when the package itself releases, which left @enbox/api@0.6.60 holding @enbox/agent@0.8.22 → @enbox/crypto@0.1.5 alongside the new graph.
