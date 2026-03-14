# @prsm/ms

parse time strings like "1h 30m" into milliseconds. zero dependencies.

## structure

```
src/index.js    - single file, default export
tests/          - vitest
```

## dev

```
make test       # run tests
make types      # generate .d.ts from JSDoc
```

## key details

- zero dependencies
- supports compound expressions: "1h 30m 15s"
- supports all common unit aliases (s, sec, secs, second, seconds, etc.)
- case insensitive
- results are cached internally
- default is milliseconds, convert with { unit: "s" } etc.
- rounding enabled by default, disable with { round: false }
- accepts a default value as second arg for invalid inputs
