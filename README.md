# Github Actions

A collection of Github Actions to integrate NodeScript with Github.

## Releasing

- Update the version in the [VERSION](./VERSION) file
- Run `script/release`

## Actions:

### Invoke

Invokes an HTTP exposed graph with an optional body payload.

Usage:

```yaml
jobs:
  your-job:
    runs-on: ubuntu-latest
    steps:
      - name: Execute a NodeScript graph
        uses: docker://NodeScriptLang/invoke:latest
        with:
          url: https://xxxxxxxxxxxxxxxx.run.nodescript.dev/xxxxxxxxxxxxxxxx
          method: POST
          body: "{\"input\": \"value\"}"
```
