# lib-str

The `str` port contract — axioms/laws every backend (`str-handl`, `str-c`, `str-js`) must satisfy.

Part of the `handl-lang` org split (ADR-0128). History is a `git subtree
split` of `host/handl-packages/handl-packages/str/`.

## Layout

```text
src/        the .hnl sources
pkg.hnl     dependencies, when any: `{ deps: { <name>: "branch:<ref>" } }`
```

## Gate

```bash
HNL=../host-cli/target/debug/hnl scripts/hnl-gate.sh
```

## License

MIT.
