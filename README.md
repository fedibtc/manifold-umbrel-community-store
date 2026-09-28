# Manifold Community App Store (retired)

> **Manifold Fedimint Guardian is now in the official Umbrel App Store.**
> Install it from there: https://apps.umbrel.com/app/manifold-fedimint-guardian
>
> **Do not add this store for new installs.** Umbrel will show
> "This app ID conflicts with another app" and the Install button will be
> grayed out, because this store uses the same app ID as the official listing.

## New install

1. In Umbrel, open the main **App Store** and search for
   **Manifold Fedimint Guardian**.
2. Select **Install**. It requires Umbrel's **Bitcoin Node** (or Bitcoin Knots)
   on mainnet.
3. Open Guardian and use the app password shown by Umbrel. Follow the
   [Guardian guide](https://manifold.fedi.xyz/guardian-guide.html) to finish
   setup and authorization.

If you already added this store and see the conflict message, remove it:
**App Store → ⋯ menu → Community App Stores → Manifold → Remove**, then
install from the main App Store as above.

## Already installed from this store?

1. Remove **Manifold** from Community App Stores.
2. **Do not uninstall Guardian.** Uninstalling deletes its data.
3. Keep using your installed Guardian. It uses the same app ID and data paths
   as the official listing, so updates come from the official store with no
   reinstall or data move.

## Existing Fedi Dev installations

The [Fedi Dev store](https://github.com/fedibtc/manifold-umbrel-store) is
separate and unchanged. Its apps have different IDs. Existing Fedi Dev users
should keep using their installation; moving it requires a separately planned
transfer.

## Support

Issues with the Umbrel package: open an issue in this repository.
Issues with the guardian software: https://github.com/fedibtc/manifold/issues
