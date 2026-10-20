# Upstream notes: official Redis repository

Research collected for our caching-layer build-vs-adopt evaluation. Source: the official open-source Redis repository on GitHub, observed at the time of writing.

- **Full name:** `redis/redis`
- **Star count (at time of lookup):** 77,041
- **README self-description:** "For developers, who are building real-time data-driven applications, Redis is the preferred, fastest, and most feature-rich cache, data structure server, and document and vector query engine."
- **License (from the root `LICENSE.txt`):** Tri-licensed. Starting with Redis 8, new code is governed by a choice of (a) Redis Source Available License v2 (RSALv2), (b) Server Side Public License v1 (SSPLv1), or (c) GNU Affero General Public License v3 (AGPLv3). Redis Open Source 7.2 and prior releases remain subject to the BSD 3-Clause (BSDv3) license.

## Notes for the adoption decision

- RSALv2 and SSPLv1 are source-available licenses, not OSI-approved open source licenses, and both restrict offering the software's functionality to third parties as a service. AGPLv3 is a strong copyleft license with network-distribution obligations.
- Any adoption path must account for which of the three licenses applies to the version we would deploy, and for the fact that releases 7.2 and earlier carry a different (BSD 3-Clause) license than 8.0+.
