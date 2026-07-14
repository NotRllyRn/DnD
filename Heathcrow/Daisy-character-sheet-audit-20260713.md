# Daisy Character Sheet Audit — 2026-07-13

<!-- markdownlint-disable MD013 -->

## Verdict

Daisy's level-12 sheet is **mostly arithmetically correct under the DM rulings recorded in `context.md`**. The level-12 Wizard chassis, final ability modifiers, saves, skills, spell statistics, slots, prepared-spell limit, subclass scaling, and most card results check out.

The sheet is **not a rules-as-written level-12 character**. Level 12, AC 23/27, the Bone Wand, Ring of Intellect, Beelzebub's necklace, and the casting ability for the Well cantrips all depend on explicit DM changes. That is valid for this campaign, but those entries should not be mistaken for the published card effects.

Corrections or additions are needed for:

1. Osteomantic Adept's omitted self-damage formula.
2. Tomb's one-year use deadline.
3. Costly spell components missing from the inventory, especially the 300 gp opal consumed by Graveyard Shuffle and the 1,500 gp statuette required by Contingency.
4. Ring card attunement handling.
5. Knight's published requirement that the fighter be the same race as Daisy.
6. The spellbook acquisition history, which cannot be reconciled exactly from the labels currently used without reordering level-up selections or recording copied/DM-granted spells.
7. HP 106 and the starting ability ledger remain conditional because the old rolls/source ledger are not preserved.

## Rules and sources used

Source priority followed:

1. Recorded Heathcrow DM rulings in `context.md`.
2. 2014 D&D 5e rules.
3. The adopted local Steinhardt PDF.
4. Official online sources and the source list in `SOURCES.md`.

Primary references:

- *Player's Handbook* (2014), especially pp. 113–115, 165, 168, and 177.
- Local *Steinhardt's Guide to the Eldritch Hunt*, especially printed pp. 110–113, 124–136.
- [Official 2014 Deck of Many Things entry](https://www.dndbeyond.com/magic-items/4617-deck-of-many-things).
- [Official Headband of Intellect entry](https://www.dndbeyond.com/magic-items/4652-headband-of-intellect).
- *The Book of Many Things*, p. 51, checked through the complete [Deck of Many More Things transcription](https://dnd5e.wikidot.com/wondrous-items:deck-of-many-more-things) because the official full text is not freely accessible.
- Volo's Kenku rules, *Volo's Guide to Monsters*, pp. 109–111.

The local Steinhardt PDF is the authority for this audit. Some online Steinhardt mirrors contain older playtest wording and differ from it. In particular, the adopted local book makes **Bone Shield off-list for Wizards** and makes Graveyard Shuffle consume an opal worth **300 gp**, not 150 gp.

## Level-12 Wizard audit

| Entry | Sheet | Audit |
| --- | ---: | --- |
| Proficiency bonus | +4 | Correct |
| Wizard cantrips | 5 | Correct |
| Spell slots | 4/3/3/3/2/1 | Correct |
| ASI/feat opportunities | Wizard 4, 8, 12 | Correct; all three are used |
| Spell save DC | 18 | Correct: 8 + 4 + 6 |
| Spell attack | +10 | Correct: 4 + 6 |
| Prepared spells | 18 | Correct: Wizard 12 + Intelligence modifier 6 |
| Arcane Recovery | 6 slot levels, no 6th-level slot | Correct |
| Hit Dice | 12d6 | Correct |

The three Wizard advancement choices are fully allocated:

- Wizard 4: +2 Intelligence.
- Wizard 8: Resilient (Constitution).
- Wizard 12: Osteomantic Adept, with +1 Wisdom.

## Ability scores

The final scores are internally consistent with the recorded sequence:

| Ability | Reconstructed before cards/level ASIs | Changes | Final |
| --- | ---: | --- | ---: |
| Strength | 11 | Lance +1 | 12 |
| Dexterity | 13 | Lance +1, Expert +2 | 16 |
| Constitution | 15 | Lance +1, Resilient +1 | 17 |
| Intelligence | 17 | Lance +1, Wizard ASI +2, Star +2 | 22 |
| Wisdom | 14 | Lance +1, Osteomantic Adept +1 | 16 |
| Charisma | 11 | Lance +1 | 12 |

This ordering is important. Lance cannot raise a score above 20, an ordinary ASI cannot raise a score above 20, and Star can raise its chosen score as high as 24. Applying Lance and the ordinary Intelligence ASI before Star legally produces Intelligence 22.

The original score rolls/ledger are not preserved, so the reconstructed starting scores cannot be independently proved. They are nevertheless internally coherent.

## HP

The sheet's **106 HP** is correct only if Daisy used the Wizard fixed average at every level:

- Level 1: 6 + 3 Constitution = 9.
- Levels 2–12: 11 × (4 + 3) = 77.
- Wizard total = 86.
- Giant = +20 maximum and current HP.
- Final maximum = 106.

A Constitution modifier increase changes maximum HP retroactively, so using +3 for all twelve levels is correct. If any earlier Wizard hit points were rolled, 106 cannot be confirmed without those rolls. The Markdown sheet appropriately calls it an assumption, but the quick-value table should continue to be read as conditional.

## Saves, skills, and Kenku/background choices

The numerical saves and skill bonuses check out.

- Constitution save +7: Constitution +3 and proficiency +4.
- Intelligence and Wisdom saves +10/+7: Wizard save proficiencies.
- Arcana and Investigation +10.
- Deception +5 and Sleight of Hand +7 are valid Volo Kenku Training choices.
- Worthless Husk grants Stealth and Survival; both +7 values are correct (local Steinhardt p. 124).
- Speed 30 feet and languages Common/Auran match Volo Kenku.
- Volo Kenku also cannot speak normally except through Mimicry; the short trait list is not the complete rule.

Anatomical Expert is calculated correctly under the adopted local version (Steinhardt p. 111):

- Normal Medicine: Wisdom +3 + proficiency +4 + Intelligence +6 = **+13**.
- Creature with a skeleton: Wisdom +3 + double proficiency +8 + Intelligence +6 = **+17**.

The prior campaign note granting advantage on Heathcrow checks is a campaign ruling, not a Kenku trait.

## Osteomancer and feat audit

### Correct

- Brittle Bone Armor: bonus action; 24 temporary HP; +4 AC at Wizard 12; slashing/piercing resistance while its temporary HP remain; one use per short or long rest; requires no worn armor or shield.
- Bone Puppetry: action, 60 feet, Strength save against DC 18, six uses per long rest.
- Skeletal Mastery: Alter Self at will with the restricted options; no concentration; boneless movement and limitations are summarized correctly.

The Mithral Plate Cloak has been ruled not to count as armor, so it does not block Brittle Bone Armor in this campaign.

### Correction: Osteomantic Adept is incomplete

The sheet says only that Daisy takes necrotic damage to cast an osteomancy spell one level higher. The adopted feat (Steinhardt p. 113) additionally says:

- The spell must be an osteomancy spell of 1st level or higher.
- Roll a number of d6 equal to half the spell's **original level**, rounded up, minimum one die.
- Daisy takes that much necrotic damage.
- That damage **cannot be reduced in any way**.

Examples:

- Empower a 1st- or 2nd-level spell: 1d6 self-damage.
- Empower a 3rd- or 4th-level spell: 2d6 self-damage.
- Empower a 5th- or 6th-level spell: 3d6 self-damage.

The Wisdom +1 choice is legal; the feat permits Intelligence, Wisdom, or Charisma +1, maximum 20.

## Spellbook and prepared spells

### Counts

The total of 31 non-cantrip spells is plausible:

- A Wizard normally has 28 level-up spells by level 12: six at level 1 plus two for each of eleven later Wizard levels.
- The three separately granted occult spells make 31.

However, the acquisition labels do not establish a fully legal history by themselves. A level-3 Wizard's ten normal level-up spells must include at least eight 1st-level spells, because 2nd-level slots do not arrive until Wizard 3. The sheet labels the pre-jump spellbook as four 1st-level and six 2nd-level spells. That can be resolved only if:

- several spells were copied or DM-granted before the jump, or
- some of the current “new leveling additions” are reassigned as Daisy's earlier 1st-level selections and some old 2nd-level entries are reassigned to later Wizard levels.

The final collection can be arranged into a legal level-12 progression, but the current “previous” versus “new” labels are not a reliable acquisition ledger.

### Bone Shield classification

The current sheet is correct to call Bone Shield off-list. In the adopted local Steinhardt edition, Bone Shield is a Druid/Ranger/Warlock spell, not a Wizard spell (printed p. 128). An older online playtest listed Wizard and should not override the local source.

Graveyard Shuffle is likewise Cleric/Druid only (printed p. 136). Daisy can prepare these only because of the Bone Wand's custom rule, and the DM should explicitly confirm that the wand allows off-list spells to be entered in the spellbook, prepared as Wizard spells, and cast using Intelligence.

### Costly components currently missing

A component pouch or arcane focus does not replace a material component that has a listed price or is consumed. The Bone Wand does not bypass those components unless the DM explicitly says it does.

| Spell | Required component | Current issue |
| --- | --- | --- |
| Dread Scarecrow | Femur flute worth 50 gp | Not listed in inventory |
| Graveyard Shuffle | Spinal bone and an opal worth at least 300 gp; opal consumed | Not listed; spell cannot be used as the stated emergency revival without it |
| Contingency | Statuette of Daisy worth at least 1,500 gp | Not listed; Contingency also ends if the statuette leaves Daisy's person |
| Bone Cocoon | Shrunk and gilded rib cage worth at least 50 gp | Not listed; relevant when preparing/casting it |
| Find Familiar | 10 gp of charcoal, incense, and herbs consumed in a brass brazier | Not listed; needed each casting |

Mine's 5,000 gp gems do not automatically satisfy “an opal” or a specially made statuette. A suitable gem/component must be identified or purchased, unless the DM permits a substitution.

### Prepared-list consequence

Until the components are obtained or waived, **Graveyard Shuffle and Contingency should not be treated as ready-to-use prepared options**, and Dread Scarecrow also needs its flute. The prepared-spell count remains legal, but the practical combat guide overstates access to these spells.

## Deck/card audit

### Published effects recorded accurately

| Card | Audit |
| --- | --- |
| Aberration | 90-foot telepathy is correct |
| Star | +2 Intelligence, maximum 24, is correct |
| Fates | Unused event erasure before Daisy dies is correct |
| Flames | A powerful devil is Daisy's enemy; “nothing apparent” does not mean no effect |
| Expert | Dexterity +2, maximum 22, is correct |
| Lance | All six scores +1, maximum 20, is correct |
| Giant | +20 maximum/current HP is correct; +5 inches is a valid 2d10 roll |
| Mine | Seven gems and seven ore chunks are valid rolls; 52,500 gp total is correct |
| Well | Learning three cantrips from any list is correct |

Guidance, Eldritch Blast, and Mind Sliver are valid choices if the DM allows their sourcebooks. The card does not define a casting ability, so Intelligence remains a necessary DM ruling. Their level-12 scaling on the sheet is correct.

### Tomb deadline missing

Tomb allows one component-free casting of True Resurrection **within one year of drawing the card**. It is not an indefinite unused resurrection. Record the in-world draw date and expiry date.

### Ring attunement needs firmer recording

Published Ring creates a DM-chosen rare-or-rarer ring. If the drawer has an available attunement slot, the card automatically attunes the drawer to it when it appears.

The Ring of Intellect is a custom ring version of Headband of Intellect. Its “set Intelligence to 19” effect correctly does nothing while Daisy's natural Intelligence is 22. But:

- the ring should be rare or rarer to satisfy the card;
- the headband-equivalent normally requires attunement; and
- if an attunement slot was available when drawn, the Ring card says Daisy was automatically attuned.

Only a further DM modification makes attunement wholly unresolved.

### Knight race detail missing

Published Knight gives a loyal 4th-level fighter of the **same race as the drawer**. Beelzebub should therefore be a Volo Kenku unless the DM changed this. The storing/summoning necklace and free-action deployment are entirely custom additions.

### Explicit DM modifications, not errors

| Card | Published result | Heathcrow result |
| --- | --- | --- |
| Key | Rare-or-rarer magic weapon with which Daisy is proficient | Custom Legendary Bone Wand |
| Tree | Base AC 15 + Dexterity while unarmored, plus fire vulnerability | Stackable +5 AC plus fire vulnerability |
| Jester | 10,000 XP or two extra draws | Exactly one milestone level |
| Sun | 50,000 XP and a random wondrous item | Party-wide jump to level 11, no item |
| Ring | DM-chosen rare-or-rarer ring | Custom Ring of Intellect |
| Knight | Same-race level-4 fighter | Fighter plus custom summoning necklace |
| Well | Three any-list cantrips; no casting ability specified | Intelligence casting ability |

Under published 2014 XP rules, a level-3 character receiving 60,000 total XP from Sun and Jester would finish at **level 9**, not level 12. Daisy is level 12 only because the DM replaced Sun with the party milestone to level 11 and replaced Jester with one additional level. `context.md` records both rulings, so level 12 is correct for Heathcrow.

## Armor Class

The calculations are correct under the recorded DM rulings:

- Cloak base: 15 + Dexterity 3 = 18.
- DM-modified Tree: +5 = 23.
- Brittle Bone Armor: +4 = 27 while active.

Published Tree would not add +5. It would set unarmored base AC to 15 + Dexterity, which duplicates the cloak's existing 18 rather than stacking with it. Under published Tree plus the cloak ruling, Daisy would be AC 18 normally and AC 22 with Brittle Bone Armor. Therefore 23/27 must remain clearly labeled as house-rule values.

Tree's fire vulnerability is correctly recorded. Fire resistance from Absorb Elements or the cold version of Fire Shield counteracts that vulnerability; in the ordinary case, having both produces approximately normal incoming fire damage rather than half damage.

## Final confirmed quick values

Subject to the DM rulings and assumptions stated above:

| Statistic | Confirmed value |
| --- | ---: |
| Level | Wizard 12, by DM milestone/card conversion |
| Proficiency | +4 |
| AC | 23, house rule |
| AC with Brittle Bone Armor | 27, house-rule stacking |
| Initiative | +3 |
| Speed | 30 ft. |
| HP | 106 only with fixed-average leveling |
| Temporary HP from Brittle Bone Armor | 24 |
| Spell save DC | 18 |
| Spell attack | +10 |
| Prepared spell limit | 18 |
| Wizard cantrips | 5 |
| Well cantrips | 3 |
| Spell slots | 4/3/3/3/2/1 |
| Passive Perception | 13 |
| Medicine | +13, or +17 for a creature with a skeleton |

## Recommended corrections to the working sheet

1. Add Osteomantic Adept's exact d6 self-damage formula and “cannot be reduced” clause.
2. Add Tomb's one-year deadline and record its in-world expiry.
3. Add or obtain the 50 gp femur flute, 300 gp consumable opal plus spinal bone, and 1,500 gp self-statuette before relying on Dread Scarecrow, Graveyard Shuffle, and Contingency.
4. Record whether the Ring of Intellect is rare or rarer and whether Daisy is currently attuned.
5. Record Beelzebub as Kenku or note the DM's race override.
6. Replace the “previous/new” spellbook split with a simple current list, or add a provenance note explaining copied/DM-granted/reassigned selections.
7. Preserve the 106 HP label as conditional until the old HP rolls or a fixed-HP DM ruling are confirmed.
8. Keep AC 23/27 and level 12 labeled as campaign rulings, because neither follows directly from the published card text.
