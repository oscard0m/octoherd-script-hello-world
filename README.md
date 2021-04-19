# octoherd-script-hello-world

> The "Hello, World!" of all Octoherd Scripts!

[![@latest](https://img.shields.io/npm/v/octoherd-script-hello-world.svg)](https://www.npmjs.com/package/octoherd-script-hello-world)
[![Build Status](https://github.com/oscard0m/octoherd-script-hello-world/workflows/Test/badge.svg)](https://github.com/oscard0m/octoherd-script-hello-world/actions?query=workflow%3ATest+branch%3Amain)

## Usage

Minimal usage

```js
npx octoherd-script-hello-world
```

Pass all options as CLI flags to avoid user prompts

```
npx octoherd-script-hello-world \
  --greeting-name Oscar \
  -T ghp_0123456789abcdefghjklmnopqrstuvwxyzA \
  -R "oscard0m/*"
```

## Options

| option                       | type             | description                                                                                                                                                                                                                                 |
| ---------------------------- | ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `--greeting-name`            | string           | The name you want to be greeted with. Example `--greeting-name Oscar`                                                                                                                                                                       |
| `--octoherd-token`, `-T`     | string           | A personal access token ([create](https://github.com/settings/tokens/new?scopes=repo)). Script will create one if option is not set                                                                                                         |
| `--octoherd-repos`, `-R`     | array of strings | One or multiple space-separated repositories in the form of `repo-owner/repo-name`. `repo-owner/*` will find all repositories for one owner. `*` will find all repositories the user has access to. Will prompt for repositories if not set |
| `--octoherd-bypass-confirms` | boolean          | Bypass prompts to confirm mutating requests                                                                                                                                                                                                 |

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md)

## About Octoherd

[@octoherd](https://github.com/octoherd/) is project to help you keep your GitHub repositories in line.

## License

[ISC](LICENSE.md)
