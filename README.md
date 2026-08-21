# renovate-config

sharable renovate configs

## Usage

### For projects with auto-merge enabled

The automerge presets only configure automerge. Always extend them together with
`main.json5`, which defines the `minimumReleaseAge` cooldown.

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>sasaplus1/renovate-config:main.json5",
    "github>sasaplus1/renovate-config:automerge-all.json5"
  ]
}
```

Use `automerge-minor.json5` instead to limit auto-merge to minor and patch
updates.

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>sasaplus1/renovate-config:main.json5",
    "github>sasaplus1/renovate-config:automerge-minor.json5"
  ]
}
```

### For npm library projects

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>sasaplus1/renovate-config:main.json5",
    "github>sasaplus1/renovate-config:npm.json5",
    "github>sasaplus1/renovate-config:npm-lib.json5"
  ]
}
```

### For npm application projects

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>sasaplus1/renovate-config:main.json5",
    "github>sasaplus1/renovate-config:npm.json5",
    "github>sasaplus1/renovate-config:npm-app.json5"
  ]
}
```

### For npm monorepo projects

`npm-monorepo.json5` pins dependencies per workspace: `packages/**` is treated as
libraries and `apps/**` as applications.

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>sasaplus1/renovate-config:main.json5",
    "github>sasaplus1/renovate-config:npm.json5",
    "github>sasaplus1/renovate-config:npm-monorepo.json5"
  ]
}
```

## Links

- https://docs.renovatebot.com/
- https://docs.renovatebot.com/presets-default/
- https://developer.mend.io/github/sasaplus1/renovate-config

## License

The MIT license
