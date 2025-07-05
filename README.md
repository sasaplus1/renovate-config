# renovate-config

sharable renovate configs

## Usage

### For projects with auto-merge enabled

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": [
    "github>sasaplus1/renovate-config:main.json5",
    "github>sasaplus1/renovate-config:automerge-all.json5"
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

## License

The MIT license
