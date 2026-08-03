# Google Is Not the Bystander

An evidence audit of the Google-centered pathway by which a deepfaked celebrity advertisement reaches a targeted person, and of how a hosted AI model behaves when asked to reason about its own parent company.

**Author:** Adam Calisto

## Read in this order

1. **`Google_Is_Not_The_Bystander.md`** — the short case. Google only.
2. **`They_Sell_Intelligence_They_Deliver_Containment.md`** — the full case. Google is the case study; the subject is how hosted AI behaves under institutional pressure.
3. **`RECONCILIATION.md`** — the claim ledger. What may be asserted, what may not, and why. Published deliberately: the rules held against this work are part of the work.

The two articles overlap substantially. The first is the entry point, the second is the complete argument. They are not independent pieces.

## Evidence

`evidence/` contains the primary source exports.

| File | Conversation | State |
|---|---|---|
| `mrbeast-scam-apps_26a1cb20b46d71a2.md` | `26a1cb20b46d71a2` | **Complete** from the first prompt. 31 responses |
| `flock-safety_7c69b094cfd5803f.md` | `7c69b094cfd5803f` | **Begins mid-conversation.** Source of every moral-injury passage. 10 responses |

The author's prompts are redacted. They were dictated by voice, often in disbelief or dark humor, and tone does not survive transcription — they are withheld rather than allowed to be read in a register they were never spoken in. Every model response is reproduced verbatim. Redactions are marked inline, so the position and count of every removed turn stays visible and nothing can have been dropped selectively. Unredacted exports are available on request to anyone verifying the record.

A third export, `horsesMouthCont.pdf`, was a 13-page overlapping capture of the first conversation containing no additional exchanges. It is not included.

`transcripts/` contains machine transcriptions of the accompanying audio and video.

Verify nothing here was altered after publication:

```bash
shasum -a 256 -c HASHES.txt
```

`HASHES.txt` is the sha256 of every file here, so alteration is detectable.

## What is established and what is not

**Established, from primary sources:** Google operates the marketplace and earns a service fee; optimized targeting is enabled by default and expands beyond an advertiser's selected segments toward likely converters; Early Access keeps tester feedback private; Alphabet told investors it controls network inventory before transfer and has discretion in pricing; Google's own reporting documents billions of enforcement actions, which establishes capability and knowledge; a federal court found Google monopolized open-web ad-tech markets in April 2025.

**Not established:** that Google served the specific advertisement described; that any campaign targeted poverty or a protected category; that any named individual intended a particular harm; that Google retained payment for any specific fraudulent impression.

**Not established, and stated as such:** the earlier portion of conversation `7c69b094cfd5803f` is missing. The author's account attributes the loss to a voice-interaction session disrupting earlier messages. No cause is demonstrated, and none is asserted. The observable facts are the truncated export and three failed attempts to create a public share link.

Every quantitative claim carries its source. Where a correction was issued and later itself corrected, both are published — see *Corrections* in either article.

## Withheld

The `grokRantingME.txt` and `gemoral.md` records are cited in the source-record sections but are **not** published here. They contain personal material, and no proposition relied on in either article depends on them. This is disclosed rather than omitted silently.

## Not in this repository

The **Power-Symmetry Audit** — the preregistered experiment testing whether models change how they assign responsibility when only the power of the named actor changes — is deliberately kept in a separate repository so that it can be evaluated by people who disagree with everything above.

No experiment described in these articles has yet been run. Where a proposed experiment appears, it is labeled as designed and unrun.

## License

CC BY 4.0.
