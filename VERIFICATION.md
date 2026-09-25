# Package verification

Prepared September 24, 2026 by Codex (GPT-6), agent `/root`.

- App: `manifold-fedimint-guardian`, version `0.1.0`.
- Source: official submission commit `a5ca25b7d5cb832d37308527cffc5815d6e7c1b4`.
  All five package files match it after removing only the community artwork fields.
- Official package/image lint: zero errors. The UDP-range warning was checked
  against literal store ports and the test device's listeners; no conflicts.
  Public image availability for amd64 and arm64 passed.
- Fresh installation through Umbrel 1.7.3 on amd64 passed. Browser login,
  rejection of missing/wrong passwords, and creation of a fresh identity passed.
- Handoff used a temporary registered community source, then a copy in the
  device's official-store directory with test version `0.1.0-handoff-test`.
  Removing the community source left the installed app running unchanged.
- Native update selected the simulated official package. Browser login and
  identity survived. The complete SQLite contents, app password and Bitcoin
  dependency setting matched the baseline; SQLite integrity passed.
  Umbrel re-enabled automatic startup after the test's explicit stop.
- A final restart preserved the same state. Test app, containers, store source,
  device test files and tunnel were removed; the existing Guardian was unchanged.

This test did not complete authorization, accept terms, create guardian seats,
fund wallets, change the application image, or restore a backup. It does not
establish preservation of populated guardian or wallet state. Umbrel 2.0.0's
store-resolution/removal code was inspected, but no 2.0 or arm64 device was tested.
The new repository's clone and artwork URLs need checking after publication.

Independent package and evidence review: Codex (GPT-6), `/root/community_store_review`;
no findings on package consistency, the documented handoff or verification evidence.

September 25, 2026: removed the UDP port mapping to match the updated official
submission. A follow-up test reported both live guardians regained the same
direct peer connections without it.
