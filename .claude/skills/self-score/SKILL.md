---
name: self-score
description: Score the TDK paper's reviewer PDF on the faculty review sheet's criteria A-E in the sheet's own words, name the weakest criterion and the cheapest fix, and optionally read it as one of eight reviewer personas. Use before a consultation, in the polish phase, or when the student asks "how would this score". Writes nothing.
---

# Self-score

Score `paper/reviewer.pdf` the way the TDK reviewer will, on the review sheet in
`paper/docs/TDK2025_biralati_pontozolap_hallgatoi.pdf`. The sheet has five criteria and 35 points:
A form and style 0-5, B figures and literature 0-4 (average of B/1 and B/2), C topic 0-8,
D originality and soundness 0-10 (D/1 novelty 0-5 plus D/2 correctness 0-5), E introduction and
evaluation 0-8. The guide's TDK essentials chapter quotes the top of every scale.

## Procedure

1. Build or locate `paper/reviewer.pdf`; refuse to score the draft with the notes in it.
2. Read the whole PDF once as a reader, then once per criterion.
3. For each criterion, give the score and the sheet's own sentence that fits, then the evidence:
   page numbers, a quoted phrase, a figure or table number. No evidence, no score.
4. Name the weakest criterion and the single cheapest change that would raise it, with where it
   goes. Then the second cheapest.
5. If a persona was requested, read `personas/<name>.md` and give that reader's three objections,
   each with a page reference and what would answer it.

## Output

Chat only, in this shape, nothing else:

```
A  4/5  "jól tagolt, követhető" except: <evidence>
B  3/4  B/1 <score> <evidence>; B/2 <score> <evidence>
C  7/8  <evidence>
D  7/10 D/1 <score> <evidence>; D/2 <score> <evidence>
E  5/8  <evidence>
Total 26/35

Weakest: E. Cheapest fix: <one change, where>.
Second: <one change, where>.
```

Do not write files, do not edit the paper, do not soften a score because the author is in the
room. The consultation recording is the record.

## Personas

`personas/` holds eight short readers. Each file says who they are, what they look for first,
what they dismiss, and their favourite objection. Run one when asked ("score as the cryptographer"),
or all eight when asked for the premortem.
