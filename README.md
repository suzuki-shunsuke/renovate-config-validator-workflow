# renovate-config-validator-workflow

GitHub Actions Reusable Workflow for renovate-config-validator

## How to use

```yaml
name: renovate-config-validator

permissions: {}

on:
  pull_request:
    branches:
    - main
    paths:
    - .github/workflows/renovate-config-validator.yaml
    - renovate.json5
  push:
    branches:
    - main
    paths:
    - .github/workflows/renovate-config-validator.yaml
    - renovate.json5

jobs:
  renovate-config-validator:
    uses: suzuki-shunsuke/renovate-config-validator-workflow/.github/workflows/validate.yaml@37f3b320ff7dd6fbf4fa25ce9e704ed817437a4c # v0.1.0
    permissions: {}
```

## LICENSE

[MIT](LICENSE)
