

```yaml
name: Build

on:
  push:
    branches: [ main ]

jobs:
  build:
    uses: maurosoft1973/actions-common-for-net/.github/workflows/workflow-common-setup-and-build.yml@main
    with:
      configuration: Release
      srcFolder: "./"
```
