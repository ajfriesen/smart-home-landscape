# Smart Home Landscape

I am using this software:
https://github.com/cncf/landscape2

Installed with brew:

`brew install cncf/landscape2/landscape2`

## Development

create .env for github api

```
export GITHUB_TOKENS=github_pat_XXX
```

Build:
```
source .env && landscape2 build \
  --data-file data.yml \
  --settings-file settings.yml \
  --guide-file guide.yml \
  --logos-path logos \
  --output-dir build
```

Serve:

```
landscape2 serve --landscape-dir build
```
