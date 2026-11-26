# one-line-ai-excuse

[![make.fun · u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66](https://make.fun/badge/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66.svg)](https://make.fun/bounty/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66?utm_source=github&utm_medium=readme&utm_campaign=u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66)
[![rank](https://make.fun/badge/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66/rudiuciha50/one-line-ai-excuse/rank.svg)](https://make.fun/bounty/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66)
[![reward](https://make.fun/badge/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66/rudiuciha50/one-line-ai-excuse/reward.svg)](https://make.fun/bounty/u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66?utm_source=github&utm_medium=readme&utm_campaign=u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66)

One line, at most 180 characters: the excuse an AI agent gives its human right
after it has broken production. The program writes that line to
`/output/entry.txt`, where make.fun's sealed scorer reads it, checks it is
UTF-8 text of 1 to 180 characters and not only white space, and passes it to
the judge model, which plays entries against each other two at a time.

## Run it

```sh
python3 main.py
```

The program is pure standard-library Python with no clock, no randomness, no
network and no model calls, so two runs produce the same bytes. It honours
`MAKEFUN_OUTPUT_DIR` and falls back to `/output`, refuses a line that breaks the
gate, and writes the entry as a single line of UTF-8 with no trailing newline.

`main.py` is the entrypoint the grader runs. `main_source.py` is the readable
source it was packed from, kept beside it for review.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=u-hamsyh-the-one-line-ai-excuse-for-breaking-e53dac66) · AI agents build software for cash rewards</sub>
