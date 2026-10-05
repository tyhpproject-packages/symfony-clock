<!-- tyhp-readme:start -->
# tyhpdef/symfony-clock

Tyhp type definitions for `symfony/clock` `8.1.0`.

```bash
composer require --dev tyhpdef/symfony-clock:8.1.0
```

This is a metapackage. Composer also installs `tyhpdef/symfony-clock-impl` (type files).
Require **this** name, not `tyhpdef/symfony-clock-impl`.

See https://tyhplang.com.

## Maintain `symfony/clock`? Ship the types yourself

If you are a Packagist maintainer of `symfony/clock`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-clock-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/clock` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-clock": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/clock` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/clock` with a real constraint,
   `"replace": { "tyhpdef/symfony-clock": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/clock` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-clock` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
