# Invoke

This action sends a really simple slack notification to a given channel. Nothing fancy, just a simple message to a channel.

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
