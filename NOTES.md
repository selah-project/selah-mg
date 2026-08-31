# Naoty momba ny fandikana — Translation Notes

*Ity rakitra ity dia mampiseho ny andininy rehetra nokasihin'ny tanan'olona na
fanapahan-kevitra. Ny naoty sisa dia amin'ny teny anglisy — miresaka ny rafitry
ny hebreo sy ny fanondroana izy.*

This file records every verse where a human hand or a ruling touched the Malagasy
rendering — so any verse can be audited: was it machine-pressed under the rails,
hand-rendered, or ruled, and why. Rails: the Selah Malagasy discipline
(Yahveh / Elohim at the Name seat; ⟨את⟩ total; ⟨…⟩ marks supplied words only;
Sheol never *helo*; Mesia never *Kristy*; the Malagasy alphabet has no c q u w x).

## The burn and the gleaning (2026-08-31)

The relay rendered the 23,213 verses through the rails. The census then flagged
content faults and every flagged verse was deleted and re-rendered, round by
round: **584 → 73 → 12**. The twelve that survived three renders were repaired by
hand (below). After the Tekoa and aleph-tav re-renders a further 8 survivors were
hand-repaired, and Numbers 26:56 — rendered token-less — had its tokens written by
hand against the 8 Hebrew surfaces. Final census: Yahveh 5,823 · Elohim 1,577 ·
every leak class zero · ⟨את⟩ in 7,482 verses.

## Hand-rendered / hand-repaired verses (2026-08-31)

The stubborn faults were patterned, not random (`dev/scripts/mg_hand_fixes.clj`,
`mg_at_hand_fixes.clj`, `mg_final_fixes.clj` in the Selah repo hold every pair):

- **The suffix-bracket class** — ⟨אתם⟩/⟨אתו⟩ left unrendered in the text.
  *Genesis 40:11* → **azy ireo** (the grapes); *Esther 8:11* → **mbamin'ny**;
  *Zechariah 2:4* → **azy ireo**; *Deuteronomy 8:6* → **Azy** (and the stray
  "h " particles healed: **ka handeha … ary hatahotra**).
- **The ⟨מאת⟩ class** — the compound from-with marker bled raw. *Jeremiah 11:1*
  and *2 Kings 6:33* now follow the en pattern: **⟨את⟩ avy amin'i Yahveh**.
- **Hebrew bleed in the text** — *Proverbs 18:13* אולת → **fahadalana**;
  *Psalm 78:25* אַבִּירִים → **ny mahery** (bread of the mighty; the gloss had
  also seated an Andriamanitra — un-seated); *Job 34:18* the two vocatives laid
  bare: **hoe: Belial! ary amin'ny lehibe hoe: Ratsy fanahy!**
- **A Yiddish bleed** (!) — *Ezekiel 19:13* carried ⟨⟨זי איז⟩⟩, *it is* — dropped.
- **The ⟨is⟩ class** — an English copula filled into a zero-copula language:
  *Job 6:29*, both dropped.
- **Cyrillic bleed + garble** — *1 Samuel 16:18*: Betlehemitа (Cyrillic а) →
  **Betlehemita**; עמו *with him* → **momba azy** (the render had "no mbamina").

## Per-token review — the Andriamanitra floor (2026-08-31)

The census counted 147 verses carrying the common god-word. Read per token
against the Hebrew seat (`dev/scripts/mg_tekoa_fixes.clj`), three classes:

- **True-God seat, singular** (an אלהים-family word glossed bare Andriamanitra,
  no idol-word in the verse): the common noun leaves the Name seat → **Elohim**
  — **35 verses**.
- **Plural / idol seat** (ireo andriamanitra, andriamanitra hafa, the gods of
  the nations, possessives of foreign gods): **lawful common elohim, kept — 82
  verses**. Andriamanitra stands in the witness column, as the rails say; it
  never stands at the Name seat.
- **Garble** — andriamanitra written on non-elohim surfaces, self-corrections,
  doubles: **30 verses re-rendered** through the rails rather than pair-fixed.
  After the round the floor stands at **93 lawful**.

The Tompo review floor pressed to **zero** — no title ever reached the Name seat
in the final text.

## The aleph-tav audit (2026-08-31)

Against the graph's H853/H854 token indices: 119 verses examined; **58 misaligned**
(token count differed from the Hebrew) were re-rendered; 4 missing ⟨את⟩ markers
added, 46 stray ones stripped, 23 sentences patched mechanically. The 17 the
repairer could not resolve were read one by one (`mg_at_hand_fixes.clj`):

- **Prepositions and nouns glossed as the marker** — בין (*2 Sam 19:36*), על
  (*Esther 10:1*, *Micah 3:7*, *Lev 14:31*), אל (*Haggai 2:12*), איש
  (*Isaiah 21:9*), שקוציך (*Jeremiah 13:27*) — each given its own word.
- **The Aramaic** יתהון *them* (*Daniel 3:12*) → **azy ireo**.
- **את the pronoun** (H859, *you*) glossed as the marker — un-marked by hand →
  **ianao**: *Eccl 7:22*, *Judges 13:3*, *Zech 9:11*, *Ezek 22:24*, *Ezek 16:48*,
  *Isa 51:12*, *Job 1:10*, *Neh 9:6* (**Hianao no nanao ny lanitra** — You made
  the heavens), and *Ezek 28:14* — **Ianao no kerob**: you were the cherub. The
  same letters that mark the object are the word for *you*; the audit's truth
  (H853/H854) knows the difference and so, now, does the chair.

Final alignment: **0 misaligned, 0 stray, 0 missing**.

## Issues met on the way (exposed on purpose)

- The Tekoa classifier was cloned from the isiZulu one and its ref-printer still
  searched `/zu/` in the path — the classification was sound but the garble refs
  printed mangled until the clone-artifact was fixed. Recorded here because the
  groove is only as honest as its tools.
- A first hand-repair of *Psalm 78:25* missed because the pattern carried nikud
  the file did not; the translation was then set whole rather than patched.
- Two glosses carried brackets the census rightly refused (⟨אתנו⟩ inside a
  marker gloss in *Genesis 44:26*; a ⟨is⟩ in *2 Chr 18:32*) — both re-glossed.

## Open flags

- Catalog straggler flags (ui/mg.edn): 10, registered at lighting
  (`docs/language/stragglers/mg.md`).
- Andriamanitra witness column: 93 lawful stand; a native reader's pass is
  welcome on the 35 seat-corrections, and on this file's Malagasy prose.

## Addendum (2026-08-31, evening) — a dead check, re-run by hand

The census's Tompo review regex was written with a doubled backslash inside a
Clojure regex literal (`\\btompo`), which matches a literal backslash — the
check was dead and reported 0 without looking. Discovered while cloning the
scripts for the Dutch chair. Re-verified token-level against the Hebrew
surfaces: **Tompo at the Name seat = 0** (יהוה → tompo: 0; אֲדֹנָי Adonay →
tompo: 0). The 219 *tompoko / tompony / tompon'ny* glosses in the store all sit
on **אֲדֹנִי, the human "my lord"** (spoken to David, Joab, kings) — lawful.
The chair stands; the tool is fixed and the miss is exposed here on purpose.
