# Decision checklist — caching layer

Short checklist driving the build-vs-adopt decision for our caching layer, tracked in issue #1 ("Adoption decision: caching layer").

- [ ] Review upstream research notes in `docs/upstream-notes.md` before making the decision (issue #1: Adoption decision: caching layer)
- [ ] Benchmark latency under load and capture throughput numbers (issue #2: Benchmark latency under load)
- [ ] Review licensing obligations — confirm what adopting under the upstream license obligates us to (issue #3: Review licensing obligations)
- [ ] Confirm the upstream license: which of RSALv2 / SSPLv1 / AGPLv3 applies to the release we would deploy, versus BSD 3-Clause for 7.2 and earlier (per `LICENSE.txt` in `redis/redis`)
- [ ] Record the build-vs-adopt decision and rationale in this repository, closing issue #1 with the results of #2 and #3
