## Releasing New Versions

1. Run the following to create a new release in both PDF and HTML format. Replace `v1` below with the desired version:

```
npm i -g md-to-pdf &&
mkdir ./v1 &&
md-to-pdf --as-html ./README.md \
  --config-file ./config.json \
  ./v1/whitepaper.html &&
md-to-pdf ./README.md \
  --config-file ./config.json \
  ./v1/whitepaper.pdf
```

Note: `headerIds` must be `true` otherwise TOC links do not work.

2. Update resources that depend on the latest version (e.g. website, documentation website, and whitepaper download link in the README file of this repository)
