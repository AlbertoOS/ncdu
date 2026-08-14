# ncdu mirror metadata

`main` is the public default branch for this mirror. Its source tree is rebuilt from the verified tip of upstream's default `zig` branch on every synchronization.

The branch additionally contains only this metadata file and `.github/workflows/sync-upstream.yml`, so GitHub Actions can continue to run monthly and accept manual dispatches. Do not commit directly to `main`; the next synchronization rewrites it from upstream.

The exact unmodified upstream ref is available as `upstream/zig`. All other source branches are mirrored under `upstream/*`, and upstream tags retain their names.

Upstream: <https://g.blicky.net/ncdu.git/>
License: upstream `LICENSES/MIT.txt` (MIT License).
