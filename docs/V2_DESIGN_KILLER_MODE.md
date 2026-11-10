# V2 design: playing the killer, and other improvements (draft for review)

**Status:** built in V2 (10 November 2026). The rules as built, with all numbers, are in `DESIGN_V2.md`.

Part A (sections 1–17) covers killer mode. Part B (section 18) covers the other V2 improvements. Section 19 has the open questions and your answers. Those answers override earlier proposals.

- Items marked **Decided** are your decisions.
- Items marked **Proposed** are Claude's ideas. None of them is final until you approve it.
- Methods are kept deliberately abstract (a "care level", not real-world techniques).

---

## 1. Decided

- **Two sides.** The player can play the police (as in V1) or the killer.
- **Same world.** Killer mode uses V1's city, people, places, routines and evidence rules.
- **How acts are shown:** one short report line, written clinically, then the aftermath: news, the city's reaction and the investigation. The tone is clinical, not emotional and not vulgar. Nothing graphic is ever shown.
- **Killer mode is endless and scored.** It ends when the killer is convicted.
- **Opponent:** the computer plays the police. There is also a two-player mode on one computer: one person plays the killer, the other plays the police.
- **Also in V2 (your additions):** the killer's origin story, earlier acts leading up to the case, a press nickname, the killer's household, where they hide things and keep souvenirs, and choices that can't be undone. Proposed details are in sections 11–16.
- **Also in V2 (other improvements):** all 13 ideas from the suggestion list. See section 18.

---

## 2. Starting a game (Proposed)

- A start screen with three choices: **Police**, **Killer**, **Two-player**.
- In Killer mode, the player picks from 3 generated candidates, or takes a random one. Each candidate has a job, shifts, home, household, car, looks and usual evening places. These shape the game: a night-shift worker has different free nights than an office worker, and a person who lives with family has weaker alibis for late nights out.
- There is no forced victim type. Whatever pattern the player makes is the pattern the police try to find.

---

## 3. The daily turn (Proposed)

The killer still has a life. Work and usual habits happen automatically. Skipping them is possible, but it gets noticed.

On free evenings and days off, the player picks actions:

| Action | What it does | Risk |
|---|---|---|
| **Live normally** | Go to work and your usual places. | None. Builds a normal routine and alibis. |
| **Scout a place** | Learn who goes there and on which nights. Slower than the police's records pull. | Being seen there often gets you onto that place's list of regulars. |
| **Observe a person** | Learn their routine, and whether they live alone. | Small chance someone notices you. |
| **Act** | Choose a person, a place and a night from what you've scouted, and a **care level**. The result is one report line. | Leaves traces; see section 4. |
| **Lie low** | Stay home, keep to routine. | Lowers your heat slowly. |
| **Clear out your home** | Get rid of kept items. | Takes a free evening. Can be seen. |
| **Build an alibi** | Arrange to be seen somewhere earlier that evening. | Helps one night. Can be checked and broken. |

---

## 4. Choices that leave traces (Proposed)

V1's trace rules stay, but now the player's choices change the odds:

- **Familiar place vs new place.** Familiar is easier, but builds a pattern the police can link through place lists.
- **Care level (low / normal / high).** Higher care leaves fewer traces (shoe print, blood, hair), but takes longer, so there's more chance of a witness or a car sighting.
- **Signature (yes / no).** Leaving it raises the score but links every case.
- **Keepsake (yes / no).** Raises the score, but becomes evidence if your home is searched.
- **Your car.** Using it is faster, but cars get seen (V1's car sightings and doorbell cameras).

---

## 5. Meters (Proposed)

- **Urge** rises each day and resets after an act. If it gets very high, you're forced into a low-care act on the next free night.
- **Heat** (hidden in V1) is not shown as a number. You only see signs a resident would notice:
  - news stories, and what the police have released
  - detectives canvassing your street or workplace
  - a detective asking you questions, or asking for a sample
  - an unmarked car near your home (a tail or stakeout)
  - your usual places getting quieter

---

## 6. The aftermath (Proposed)

After each act:

1. **One clinical report line,** e.g. "Morning, day 14: the body of Maria Chen, 34, nurse, was found near The Anchor."
2. **News:** a short, factual headline and what the police are saying.
3. **The city reacts:** fewer people go out at night in that district and at that kind of place, which makes the next act harder. Police presence in that district goes up.
4. **The investigation:** the police assign detectives (shown as signs, see section 5).

All text stays clinical, factual and non-graphic.

---

## 7. The computer police (Proposed)

The computer runs the same four detectives with the same tasks as V1, using a simple priority list:

1. New body: examine the scene, attend the autopsy, canvass witnesses.
2. Pull staff and regulars lists for the places where victims were last seen.
3. Look for people who show up on more than one list, and match known traits against public records.
4. Interview and check alibis for the top suspects.
5. Stakeout the predicted place and night, or tail the top suspect.
6. Seek a warrant at case strength 3+. Charge at 7+ (V1's court rules).

**Difficulty levels** would change the detectives' skills and how well the computer cross-references lists.

---

## 8. Scoring (Proposed)

- Points for each day free.
- Bonus points for days with low heat (staying unnoticed).
- **No points per victim.** The score is about evasion, not harm.
- The game ends at conviction. An arrest followed by acquittal continues, with heat at maximum.
- Best scores are kept on this computer.

---

## 9. Two-player mode (Proposed)

- **Killer's turn:** the killer player picks actions while the other player looks away.
- **Pass-the-device screen:** a blank "Hand over to the other player" screen between turns, so neither side sees the other's information.
- **Police turn:** the police player uses V1's screens. They see only what the police know.
- Night resolves, the morning report appears, and the turns repeat.

---

## 10. What gets reused and what's new

| Reused from V1 | New for V2 |
|---|---|
| City, people, routines, map | Start screen and mode choice |
| Evidence and trace rules | Killer's daily actions and care choices |
| Court and case strength | Urge meter and visible signs of heat |
| Police tasks | Computer police decision-making |
| Evidence wall, case files | Aftermath and city reaction |
| | Scoring and local best scores |
| | Two-player turns and pass-the-device screen |

The biggest new piece of work is the **computer police**.

---

## 11. Origin story (Decided: include. Details Proposed)

- Every killer gets a generated background, written as a plain case file, not a glorified story:
  - where they were born and grew up
  - schools, and any school incidents
  - earlier towns and addresses
  - past jobs, and why they left
  - family situation, then and now
  - any earlier contact with police (complaints, minor charges, dropped cases)
- **Police mode:** it's hidden and found in pieces through records, such as an old address, a past employer or an old complaint. Each piece links to the present case.
- **Killer mode:** you read it at the start. It shapes the character's habits and weaknesses, for example how fast urge rises, which kinds of places feel familiar, and how they react to pressure.

## 12. Earlier acts, the lead-up (Decided: include. Details Proposed)

- Before day 1, the city already holds small, unsolved incidents tied to the killer, for example a prowler report, break-ins, a complaint from a neighbour, or someone reported for following a person home. They sit near the killer's home, workplace or usual places.
- They're mixed in with unrelated incidents, so not every one is relevant.
- New police task: **Pull cold-case files** for a district or place. These files are often the first link to a suspect.
- In killer mode, the lead-up is part of the origin file. Old witnesses can still recognise you.

## 13. Press nickname (Decided: include. Details Proposed)

- After the 2nd or 3rd linked case, the newspaper names the killer after the signature or the district (e.g. "The Harbor Crane Killer").
- Effects: public pressure rises faster, and more tips come in (mostly useless).
- In killer mode, the nickname appears in the headlines you read.

## 14. Household (Decided: include. Details Proposed)

V1 already gives everyone a household (alone, partner, family, roommates). In V2 those people matter:

| Household | Effect |
|---|---|
| Lives alone | Most freedom, weakest alibis, no one notices late nights. |
| Roommate | Gives a weak alibi; may notice late nights or a locked room. |
| Partner | Gives a stronger alibi; slowly notices patterns; may confront you or call the police. |
| Family with children | Strongest everyday alibi; least freedom; most people who might notice. |

- People at home have a **suspicion** level of their own, raised by late nights, hidden items and news reports that seem familiar.
- In police mode, household members can be interviewed, and they may become witnesses or tipsters.

## 15. Hiding places and souvenirs (Decided: include. Details Proposed)

- Keeping a souvenir is always optional and always adds risk.
- The killer chooses where to keep things. Each place is found a different way:

| Hiding place | How it can be found |
|---|---|
| Inside the home | Home search warrant |
| Garage or shed | Home search warrant |
| Car | Vehicle search (a separate warrant) |
| Work locker | Workplace warrant |
| Rented storage unit | New police task: check financial records (it shows the rent payments), then a warrant |
| Somewhere outside (park, waterfront) | Found by chance, by a groundskeeper or a dog walker |

- People at home may come across items kept in the home.
- The killer can move or destroy items. That uses a free evening and can be seen.

## 16. Choices that can't be undone (Decided: include. Details Proposed)

**Killer side**
- **Which killer you play.** Fixed for the whole game.
- **The signature.** Once used, changing it makes the cases harder to link, but the press and the police notice the change.
- **Destroying evidence.** It's gone for good, including anything you might later want as leverage.
- **Moving house.** Leaves a paper trail (leases, utility records, a forwarding address).
- **Confiding in someone.** That person now knows, permanently.
- **Contacting the press.** It can't be taken back, and it carries clues (handwriting, wording, where it was posted).

**Police side**
- **Releasing details to the press.** Once public, they're public. Copycats become possible.
- **Searching a home.** The suspect knows they're being watched from then on.
- **Charging someone.** As in V1, the court decides, and a failed case can't simply be retried.

## 17. Two-player note

In two-player mode, the permanent choices above apply to both players. The pass-the-device screen means neither side sees the other's choices.

---

## 18. Other V2 improvements (Decided: include all. Details Proposed)

| # | Improvement | Proposed details |
|---|---|---|
| 1 | **Save and load** | Save the case in the browser, with several save slots. Also save to a file you can keep or move to another computer. |
| 2 | **City size choice** | Any population from a village of 100 to a city of 10,000, chosen when starting a case (see answer 11). |
| 3 | **Tutorial case** | A short, easy case that walks through each task step by step. |
| 4 | **Difficulty settings** | Easy / Normal / Hard: killer care, pressure speed, detective skill. Separate settings for the computer police in killer mode. |
| 5 | **Lab delays** | Blood, fibre and sample results take 1–4 days. A faster lab costs budget. |
| 6 | **Unreliable witnesses** | Some sightings are wrong (wrong car colour, wrong height). Each sighting shows a confidence level. |
| 7 | **Richer victims' lives** | Friends, family and coworkers you can interview, plus phone records and diaries as new kinds of clue. |
| 8 | **Running a department** | Detective fatigue, an overtime budget, and specialists you can bring in (a profiler, a forensic lab, extra officers). |
| 9 | **The media** | You choose which details to release. Releasing more brings better tips, but the killer reads the news, and copycats become possible. |
| 10 | **More kinds of killer** | Different patterns and habits, a messier first act, a killer who changes victim type, and a killer who travels between districts. |
| 11 | **Case timeline** | A day-by-day view of every event, sighting and alibi, side by side. |
| 12 | **Player notes** | Your own notes on any person, place or case. They also appear on the evidence wall. |
| 13 | **Phones and tablets** | A layout that works on small screens. |

---

## 19. Open questions and your answers (10 November 2026)

Where an answer differs from an earlier "Proposed" item, the answer wins.

| # | Question | Your answer |
|---|---|---|
| 1 | Should the player pick their killer from 3 candidates, or always get a random one? | **All three ways:** pick from 3 candidates, take a random one, or build your own (choose job, household, car and so on). |
| 2 | Free choice of victims, or must the player stick to a type once one forms? | **Pull, not lock.** Straying from your type is allowed, but it raises urge. |
| 3 | Keep the urge meter? | **Yes.** An act outside your pattern lowers urge much less than one that fits it. |
| 4 | How many actions per free evening (1 or 2)? | **Time-based.** Each action costs hours from the killer's daily free time. |
| 5 | Should the computer police have difficulty levels? | **Yes:** Easy / Normal / Hard. |
| 6 | Scoring formula: are points per day free plus a low-heat bonus right? | **All three:** points per day free, a bonus for low-heat days, plus **pattern points** (staying true to your pattern) and **risk points** (permanent risky choices, such as keeping a signature). Still no points per victim. |
| 7 | Should the city react (people staying home, more police)? | **Yes, in both modes.** Also: after killings, people become more watchful at night (more witnesses), and **vigilante groups** may search for the killer too. |
| 8 | Should Police mode in V2 stay as in V1, apart from the improvements in section 18? | **Yes.** |
| 9 | How much of the origin story should the police be able to uncover? | **Whatever can be found from records, from people who know the killer now, and from people in the killer's past who knew them, if they're still alive and around.** Some may not even know the killer's real name (earlier names or aliases). |
| 10 | Should the partner or family be able to turn the killer in, ending the game? | **Yes,** if their suspicion gets too high. |
| 11 | Should a large city (10,000) be in V2? | **Yes, if it runs smoothly.** Population becomes a setting chosen when starting a new game, from a **small village of 100** up to a **city of 10,000**. |
| 12 | In which order should the V2 pieces be built? | **All at once,** as one V2 release. |

### Later additions

- **Police force size follows city size** (your decision). *Proposed details:* about 1 detective per 500 residents, with at least 1 and at most 20. A village of 100 has a single officer who covers everything. A city of 10,000 has 20 detectives, enough that you'd assign them as squads rather than one at a time.
- **Handling big forces and small villages** (your decisions):
  - **Squads and standing orders:** detectives can be grouped into squads and given lasting orders (for example "examine every new scene" or "keep canvassing Area 3") that continue until changed.
  - **County help for villages:** in small places, the county lends a forensics officer for each new body.
  - **Slower stale scenes in villages:** scenes take longer to go stale where the force is tiny.
- **Career roster** (your decision): detectives carry over between cases, gain skill in what they do (*proposed:* 5 successful uses of a skill raises it by one step, up to a maximum), and can retire or burn out. *Proposed:* burnout comes from long cases and failed charges, and retired detectives are replaced by new recruits at level 1.
