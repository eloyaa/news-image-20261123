# News Image — 23 November 2026

A make.fun entry for the `news-image-20261123` bounty: one image summing up
the world news of **Monday 23 November 2026**.

## The image

`entry.png` is a newspaper front page, "THE WORLD TODAY", built in the
session that wrote this repository from the day's reporting (Reuters, CNN,
Associated Press, BBC, France 24, The Times, Le Monde, The Hindu BusinessLine
and others, each story cross-checked in at least two sources):

1. **Ukraine sinks Russian warship off Libya** — naval drones sink the
   corvette Merkury at Benghazi; the cargo ship Angara is also hit. A Russian
   strike on Dymer, in the Kyiv region, kills 11.
2. **COP31 collapses** — climate talks in Antalya end with no deal on fossil
   fuels, the first COP failure since Copenhagen in 2009.
3. **Democrats win 258 House seats** — the biggest US House majority since
   1992, clinched by Chuck Hubbard's North Carolina recount win.
4. **24 dead in Indonesia factory fire** — blaze at a candy plant in Cikande,
   Banten; about 30 workers still missing.
5. **Asian markets tumble** — Taiwan bans short-selling as AI stock fears
   spread across the region.
6. **Trump warns Iran** — "inclined" to resume conflict if no deal is reached
   by the New Year.

## The program

`main.ts` (Node 22, standard library only) copies `entry.png` to the
output directory and checks the copy is non-empty and at most 1 MiB:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

It is deterministic: two runs write byte-identical files (verified with
`sha256sum`).

## License

MIT — see `LICENSE`.
