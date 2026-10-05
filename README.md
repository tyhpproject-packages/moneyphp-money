<!-- tyhp-readme:start -->
# tyhpdef/moneyphp-money

Tyhp type definitions for `moneyphp/money` `4.9.0`.

```bash
composer require --dev tyhpdef/moneyphp-money:4.9.0
```

This is a metapackage. Composer also installs `tyhpdef/moneyphp-money-impl` (type files).
Require **this** name, not `tyhpdef/moneyphp-money-impl`.

See https://tyhplang.com.

## Maintain `moneyphp/money`? Ship the types yourself

If you are a Packagist maintainer of `moneyphp/money`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/moneyphp-money-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `moneyphp/money` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/moneyphp-money": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `moneyphp/money` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `moneyphp/money` with a real constraint,
   `"replace": { "tyhpdef/moneyphp-money": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `moneyphp/money` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/moneyphp-money` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
