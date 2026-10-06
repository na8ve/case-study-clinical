# Case study: clinical (synthetic)

Patient **P-0000** has three findings: recurrent fatigue, a high serum
ferritin, and a subtle bronze tint to the skin. Each one alone points at
several conditions. Which single condition explains all three, and what would
confirm it?

This repository is a small synthetic world to try that question on: a
knowledge base of 30 conditions (`kb/`), 461 generated patients with their
findings (`patients/`), and a few encounter notes (`notes/`). Seed it into
your own memory at na8ve.com and ask.

## Run it

With [na8ve agent](https://github.com/na8ve/na8ve-agent):

```
na8ve-agent
/login            # choose na8ve; sign in or create your account in the browser
/demo clinical    # fetches this repository, seeds it into a space, asks the question
```

New to na8ve.com? Your first `/demo` makes a free workspace for you.

Then ask follow-ups, for example:

- What explains P-0000's findings, and what confirms it?
- Why not the other conditions that cause fatigue?
- Which other patients look like P-0000?

## What a good answer does

- It names **one** condition that accounts for all three findings, rather
  than one per finding.
- It says why that condition leads over the others that share some of the
  same findings.
- It names the test that would confirm it, as the knowledge base states.
- It cites the memories it relied on: the patient's findings, and the
  textbook, guideline or review facts behind each step.

## Synthetic data

Every patient here is generated; none is a real person. The knowledge base is
simplified for the demo. **This is not medical advice.**

Licensed under Apache-2.0 (see [LICENSE](LICENSE)). Security reports:
[SECURITY.md](SECURITY.md).
