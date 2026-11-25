# lib-str

The `str` **port contract** — axioms/laws every backend (`str-handl`,
`str-c`, `str-js`) must satisfy. Pure `.hnl`.

## Layout

| path | role |
| --- | --- |
| `src/index.hnl` | the contract — signatures + laws |
| `pkg.hnl` | package manifest — `modules: ["str"]` |
| `scripts/hnl-gate.sh`, `ci.sh` | the gate / bupha entry |

## Contract

- Port/impl split: this repo declares the `str` surface only;
  backends implement it (`str-handl` is the pure-handl reference,
  `str-c` the C/ICU native backend, `str-js` the JS backend).

## Verification

```bash
HNL=../host-cli/target/debug/hnl scripts/hnl-gate.sh
```

## License

MIT.

<!-- myco:agent-awareness -->

## Agent awareness

- Session start / any work discussion: run `myco status --prompt`
  before proposing next steps — know the board first.
- User describes new work → offer to capture it (`myco todo add`,
  `issue new`, `proposal new`). Don't wait to be asked.
- Picking up a task: `myco resume <ID>` is the briefing.
- Wrapping up: `myco handoff <ID>` anything resumable; keep statuses
  honest (claimed → in-progress → blocked/done).

<!-- /myco:agent-awareness -->
