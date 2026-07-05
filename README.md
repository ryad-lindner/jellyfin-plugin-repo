# Jellyfin Plugin Repository

Plugin repository manifests for a self-hosted Jellyfin plugin catalog.

## Add to Jellyfin

**Dashboard → Plugins → Repositories → +**, then add the manifest URL matching
your server major:

| Jellyfin | Manifest URL |
|----------|--------------|
| 12.x     | `https://raw.githubusercontent.com/ryad-lindner/jellyfin-plugin-repo/master/manifest.json` |
| 10.11.x  | `https://raw.githubusercontent.com/ryad-lindner/jellyfin-plugin-repo/master/manifest-10.json` |

Each Jellyfin major has its own manifest so a server only ever sees a compatible
plugin build.

## Plugins

- **Gapless Player** — gapless Web Audio playback for eligible audio queues.
  Source: [jellyfin-plugin-gapless-player](https://github.com/ryad-lindner/jellyfin-plugin-gapless-player).

## Layout

- `manifest.json` — Jellyfin 12.x builds.
- `manifest-10.json` — Jellyfin 10.11.x builds.

Each version entry points to a release asset (with an md5 checksum) published on
the corresponding plugin's GitHub releases.
