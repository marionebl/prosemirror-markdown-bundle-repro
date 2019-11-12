# prosemirror-markdown

This demonstrates issues where ES2015 code ends up in bundles
due to webpack preference of using `module` over `main`.

```
git clone git@github.com:marionebl/prosemirror-markdown-bundle-repro.git
cd prosemirror-markdown-bundle-repro
yarn
yarn build
grep -nr 'class MarkdownParser' dist/ # breaks ie IE
```