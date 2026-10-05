<!-- tyhp-readme:start -->
# tyhpdef/filament-filament

Tyhp type definitions for `filament/filament` `5.8.2`.

```bash
composer require --dev tyhpdef/filament-filament:5.8.2
```

This is a metapackage. Composer also installs `tyhpdef/filament-filament-impl` (type files).
Require **this** name, not `tyhpdef/filament-filament-impl`.

See https://tyhplang.com.

## Maintain `filament/filament`? Ship the types yourself

If you are a Packagist maintainer of `filament/filament`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/filament-filament-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `filament/filament` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/filament-filament": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `filament/filament` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `filament/filament` with a real constraint,
   `"replace": { "tyhpdef/filament-filament": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `filament/filament` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/filament-filament` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
