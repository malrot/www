This repo backs `https://www.malrot.org`

## Good to know

- `docs/` is programmatically generated/build (except `CNAME` which must not be modified)
- `docs/` is served as GH Pages at `https://www.malrot.org`
- `src/` contains source files, including `css`/`js` assets for `spec.malrot.org`

## How to build and deploy?

1. Run `npm run build` to build assets (= `/docs`)
2. Push to `master` to deploy to `https://www.malrot.org`

## How to build and modify locally?

```
npm install
npm run serve
```

Then access the site at [http://localhost:8080/](http://localhost:8080/) (your port may vary).

## License

Except as otherwise noted, content of MALROT GitHub repositories and MALROT files are licensed under the `CC BY SA 4.0`, code under the `MIT`.

MALROT is based on an idea from [Charles-Henri ARNOULD](https://github.com/charnould) — info@malrot.org
