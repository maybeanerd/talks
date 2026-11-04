# talks

A collection of (technical) talks, built with [Slidev](https://sli.dev/).

Each talk lives in its own folder (`<talk>/slides.md` with its own `public/`) and is deployed under `/<talk>/`.

| Talk | Path |
| --- | --- |
| let's talk nix | [`nix/`](./nix/slides.md) |
| Abusing ActivityPub to federate game servers | [`activitypub/`](./activitypub/slides.md) |

## Development

Enter the dev environment with [devenv](https://devenv.sh/) (`direnv allow`, or `devenv shell`). This installs node, pnpm and the dependencies.

- `pnpm dev:<talk>`, e.g. `pnpm dev:nix`
- visit http://localhost:3030

## Build

`pnpm build` builds every talk into `dist/<talk>/`.

## Adding a talk

1. Create `<talk>/slides.md`, and put its assets in `<talk>/public/`, referenced as `/images/...`.
2. Add `build:<talk>` and `dev:<talk>` scripts to `package.json`, following the existing ones.
