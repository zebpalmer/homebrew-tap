# homebrew-tap

Homebrew tap for [zebpalmer](https://github.com/zebpalmer)'s tools.

## Install

```sh
brew tap zebpalmer/tap
brew install zebpalmer/tap/<formula>
```

Or, in one step:

```sh
brew install zebpalmer/tap/<formula>
```

## Available formulas

| Formula | Description |
|---|---|
| [`stratt`](https://github.com/zebpalmer/stratt) | A polyglot task runner that replaces Makefiles, manages release versions, and handles Kustomize image bumps. |

## Updating

```sh
brew update
brew upgrade <formula>
```

## How this tap is maintained

The formulas under `Formula/` are **auto-generated** by each tool's release pipeline (typically via [GoReleaser](https://goreleaser.com/)). Do not edit them by hand — changes will be overwritten on the next release.

To update a formula:

1. Push a semver tag (`vX.Y.Z`) on the tool's source repo.
2. The release workflow there builds binaries, publishes a GitHub Release, and force-pushes the new formula to this tap.
3. `brew update` picks up the change for end users.

## License

The tap itself is unlicensed metadata. Each formula installs a tool with its own license — see the tool's source repo for details.
