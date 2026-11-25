# lib-str

The `str` port contract — axioms/laws every backend (`str-handl`, `str-c`,
`str-js`) must satisfy.

## Layout

```text
src/index.hnl   the .hnl sources
pkg.hnl         package manifest — modules, deps, description, license
workflows/gate.yaml           bupha entry (handl-gates) → scripts/hnl-gate.sh
```

## Gate

```bash
HNL=../host-cli/target/debug/hnl scripts/hnl-gate.sh
```

## License

MIT.
