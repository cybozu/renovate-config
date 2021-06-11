# @cybozu/renovate-config

[![npm version](https://badge.fury.io/js/%40cybozu%2Frenovate-config.svg)](https://badge.fury.io/js/%40cybozu%2Frenovate-config)

A sharable Renovate config for Cybozu.

## Usage

* `renovate.json`

```json
{
  "extends": ["github>cybozu/renovate-config"]
}
```

## Settings

See the settings in [renovate.json](https://github.com/cybozu/renovate-config/blob/master/renovate.json) and [Configuration Options](https://renovatebot.com/docs/configuration-options/) in Renovate Docs

### GitHub Actions

If you have a branch protection rule for GitHub Actions, you have to run the GitHub Action on pushing branches to allow Renovate create pull requests.
Otherwise, Renovate won't create pull requests due to the pending status.

```yaml
on:
  push:
    branches:
      - master
      - 'renovate/**' # branches Renovate creates
  pull_request:
```

## License

MIT License
