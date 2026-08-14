# ncdu mirror

A public, automated Git mirror of [ncdu](https://g.blicky.net/ncdu.git/), the NCurses Disk Usage tool by Yorhel.

> This is **not** a GitHub-native fork: the upstream is hosted outside GitHub. It is a transparent mirror maintained by `sync-upstream.yml`.

## License and provenance

The upstream `zig` branch includes the [MIT License](https://g.blicky.net/ncdu.git/tree/LICENSES/MIT.txt?h=zig). Mirrored branches and tags retain the upstream history, copyright notices, and license files. This repository does not claim authorship or add source-code changes.

- Upstream: <https://g.blicky.net/ncdu.git/>
- Current upstream default branch: `zig`
- Mirror branch namespace: `upstream/<upstream-branch>` (for example, `upstream/zig` and `upstream/master`)
- Upstream tags: kept under their original names

## Synchronization

GitHub Actions runs the mirror job monthly, at **05:17 UTC on the first day of each month**, and can also be started manually from the **Actions → Sync ncdu upstream → Run workflow** page.

The `upstream/*` branches and all tags are managed by the mirror. Do not create commits or tags in those namespaces: a later synchronization may replace them to match upstream. The `main` branch contains only this mirror documentation and its automation.

## Local clone

```sh
git clone https://github.com/AlbertoOS/ncdu.git
# Source is available at, for example:
git switch --track origin/upstream/zig
```
