# .NET Build and Test Action

This GitHub Action builds and tests .NET applications using the specified .NET SDK version.

## Inputs

| Name            | Description                    | Required | Default  |
|-----------------|--------------------------------|----------|----------|
| `dotnet-version`| The version of .NET SDK to use | `true`   | `8.0.x`  |

## Outputs

| Name            | Description                      |
|-----------------|----------------------------------|
| `build-status`  | The status of the build process  |

## Example Usage

```yaml
jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Use .NET Build and Test Action
        uses: yashmahi88/build-01@v1
        with:
          dotnet-version: '8.0.x'

