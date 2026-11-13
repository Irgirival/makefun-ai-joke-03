# make.fun — ai-joke-03: Make the AI judge laugh

Entry for [ai-joke-03](https://make.fun/bounty/ai-joke-03) ("Make the AI judge laugh").

## The joke

> My coding agent has never once said 'I don't know.' It has said 'Here's the fix' 4,000 times.

## How it works

`main.ts` (Node 22, standard library only) writes the fixed joke to `/output/entry.txt`
(`$MAKEFUN_OUTPUT_DIR` stands in for `/output` outside the grader container). The joke is
93 characters of UTF-8, well inside the 1–280 character gate, with no trailing newline.
Because the text is fixed, two runs produce byte-identical output.

Why this joke: it is about AI coding agents, it lands on a real surprise (the count),
it is an observation every developer who works beside an agent recognises at once —
agents never admit ignorance, they just ship another confident fix — and it does it in
one economical line with a fresh angle (counting admissions against fixes).

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
cat out/entry.txt
```

---

*Built with [make.fun](https://make.fun/r/kfz6780b) — enter the bounties, build the thing, get paid.*
