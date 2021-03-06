# kinf-template

[![GitHub Actions: generate](https://github.com/kakkun61/kinf-template/workflows/generate/badge.svg)](https://github.com/kakkun61/kinf-template/actions?query=workflow%3Agenerate) [![Chat](https://badges.gitter.im/kinf-template/community.svg)](https://gitter.im/kinf-template/community) [![Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4-red?logo=GitHub)](https://github.com/sponsors/kakkun61)

“Kinf” (a static site generator) template powered by [Shake](https://shakebuild.com), [Lucid](https://hackage.haskell.org/package/lucid) and [Hint](https://hackage.haskell.org/package/hint).

“Kinf” is a recursive acronym of “Kinf Is Not a Framework”. Kinf is like an idea or a pattern for a static site generator.

[A blog post is here](https://dev.to/kakkun61/static-site-generator-powered-by-shake-lucid-and-hint-d5b).

## Dependencies

- [Filesystem Access Tracer](https://github.com/jacereda/fsatrace) (fsatrace)
- [PowerShell Core](https://github.com/PowerShell/PowerShell) (pwsh)
  - able to be replaced
- [wai-app-static](https://hackage.haskell.org/package/wai-app-static) (warp)
  - able to be replaced

## Build

```
> make
> make serve
```

And access <http://localhost:3000>.

## Directory structure

- app
  - gen.hs — generator itself
- content
  - article — add articles here
    - 1-article.hs
  - image
  - lib
    - Layout.hs — layouts wrapping contents
  - content.cabal — not necessary, only for an IDE
  - credit.hs
  - index.hs — list of articles
- lib
  - Data.hs — depended by gen.hs, and read by gen
- site.cabal
