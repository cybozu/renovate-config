# @cybozu/renovate-config

[![npm version](https://badge.fury.io/js/%40cybozu%2Frenovate-config.svg)](https://badge.fury.io/js/%40cybozu%2Frenovate-config)

A sharable Renovate config for Cybozu.

## Usage

* `renovate.json`

```json
{
  "extends": ["@cybozu"]
}
```

This config is based on [@teppeis/renovate-config](https://github.com/teppeis/renovate-config)
`@cybozu/renovate-config` overrides the following settings.

* Update Circle CI images at before 9 am on Monday
* Always Update peerDeps wider

## License

MIT License
