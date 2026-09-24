# Manifold Community App Store

Install **Manifold Fedimint Guardian** on Umbrel while its
[official listing](https://github.com/getumbrel/umbrel-apps/pull/6110) is under review.
This store is maintained by Fedi and uses the same app ID and runtime package
as the submission. Only the listing's artwork links differ.

## Install

1. In Umbrel, open **App Store → Community App Stores** (under the menu).
2. Add `https://github.com/fedibtc/manifold-umbrel-community-store`.
3. Open the **Manifold** store and install **Manifold Fedimint Guardian**.
   It requires Umbrel's **Bitcoin Node** on mainnet.
4. Open Guardian and use the app password shown by Umbrel. Follow the
   [Guardian guide](https://manifold.fedi.xyz/) to finish setup and authorization.

## When the official listing is available

1. Confirm the official Umbrel store lists app ID `manifold-fedimint-guardian`.
2. Remove **Manifold** from Community App Stores. **Do not uninstall Guardian:**
   uninstalling the app deletes its data.
3. Keep using the installed Guardian. Future updates come from the official
   store; no reinstall or data move is needed when the ID and data paths match.

Both stores may list Guardian during the handoff. They refer to the same
installation. Keep this store added until the official listing appears on
your device so updates remain available.

## Existing Fedi Dev installations

The [Fedi Dev store](https://github.com/fedibtc/manifold-umbrel-store) is separate
and unchanged. Its apps have different IDs, so this store does not adopt their
data. Existing Fedi Dev users should keep using their installation; moving it
requires a separately planned transfer.

## Package maintenance

The initial package is version `0.1.0`, copied from official submission commit
[`a5ca25b7`](https://github.com/fedibtc/umbrel-apps/commit/a5ca25b7d5cb832d37308527cffc5815d6e7c1b4).
Keep the app ID, image pin, version, storage paths and password setup aligned
with that submission and the eventual official package. Never rename the app
or replace a released version with a different image. Compare the final
official package before announcing the handoff.

Package preparation and verification: Codex (GPT-6), agent `/root`.
