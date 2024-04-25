

```yaml
name: Build

on:
  push:
    branches: [ main ]
  pull_request:
    branches: [ main ]

env:
  productNamespacePrefix: "Hello"

jobs:
  build:
    uses: maurosoft1973/actions-common-for-net/.github/workflows/workflow-common-setup-and-build.yml@main
    with:
      configuration: Release
      productNamespacePrefix: "Hello"
      useVisualStudioPreview: false
      useMauiCheckDotNetTool: false
      srcFolder: "./"
      dotNetBuild: true
      installWorkflows: false
```
