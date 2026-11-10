# Design: every rule and number (V2)

V1's rules (in `DESIGN.md`) still apply unless changed here. Percentages are chances, rolled each time. All numbers are first guesses and can be changed.

## 1. Starting a case

| Setting | Choices |
|---|---|
| Play as | Police · Killer (computer police) · Two-player (one computer) |
| Population | 100 to 10,000, in steps of 100 (presets: village 100, town 500, city 2,000, large city 10,000) |
| Difficulty | Easy · Normal · Hard |
| Career roster | On or off (police side) |
| Case seed | Optional, to replay a case |

There is also a **tutorial case**: 1,500 people, Easy, 3 detectives, with 7 step-by-step tips.

## 2. The place scales with population

| Population | Districts |
|---|---|
| up to 300 | 1 |
| up to 1,000 | 2 |
| up to 3,000 | 4 |
| above 3,000 | 6 |

- **Places:** about 1 per 40 people (at least 8, at most 300). Small places use a selection of the named places. Large ones add generated pubs, cafés, shops, offices, works, schools, clinics, parks and so on.
- **Jobs:** about 48% of people work.
- **Names:** every resident has a different name. A middle initial is added if needed.
- **Hometown:** half the residents were born in the city; the rest come from one of 20 towns.

## 3. Difficulty

| | Easy | Normal | Hard |
|---|---|---|---|
| Public pressure per day | +1 | +2 | +3 |
| Killer's traces | ×1.15 | ×1 | ×0.85 |
| First gap between killings (police mode) | 7 days | 6 days | 5 days |
| Detectives' skills | +1 (to max 3 at start) | as listed | −1 (min 1) |
| Computer police (killer mode) | basic | uses phone records, background checks, finances, trait searches | also predicts stakeout nights more aggressively, works more suspects at once |

## 4. Your department

- **Force size:** about 1 detective per 500 people (at least 1, at most 20). A village gets a single sergeant.
- **Villages and small towns** (1,000 people or fewer): the county sends a forensics officer to each new scene (finds a shoe print 70%, blood 55%, hair 70%). Scenes stay fresh for 4 days instead of 2.
- **Skill levels** run from 1 to 4. **Chance of success** = 30% + 20% per level, at most 97%.
- **Getting better:** 5 successful uses of a skill raise it by one level, up to 4.
- **Fatigue:** +1 per working day, −2 per paperwork day. At 6, the detective works at one skill level lower. At 9, they take a day off (−3).
- **Squads** (5 or more detectives): put detectives in squads A, B or C and give a whole squad one order.
- **Standing orders:** a task carries on each day until you change it. "★ Newest case" always targets the latest body.
- **Budget:** starts at 40 + 10 per detective, plus 10 + 5 per detective every Monday.

| Spend | Cost | Effect |
|---|---|---|
| Profiler | 30 (once per case) | Report on the victim type, the offender's likely age range and the nights they strike |
| Temporary officer | 25 | One extra officer for 5 days (one skill at 2, the rest at 1) |
| Rush a lab result | 10 | Result arrives the next morning |

### Career roster

- Kept in the browser between cases. It starts with the four V1 detectives. New recruits start at level 1, with one skill at 2.
- **Burnout points:** 1 per 10 days of a case, plus 2 per failed charge. A detective retires at 6 points. There is also a 5% chance per case of retiring anyway.

## 5. Evidence

### The lab

- Blood traces and blood samples take 1–3 days (one more day above 5,000 people). Phone records take 2 days.

### Witnesses can be wrong

- **How often they're right:** ordinary witnesses 75%, a doorbell camera 85%, a friend's memory 90%, a message in phone records 80%, neighbours guessing a car 70%.
- **Confidence shown with each report:**

| | High | Medium | Low |
|---|---|---|---|
| When the witness is right | 50% | 35% | 15% |
| When the witness is wrong | 15% | 35% | 50% |

- The profile shows the value with the most weight (high = 3, medium = 2, low = 1) and lists every report.
- **Witness traits** (sex, car colour) and the age estimate count **+1** when they match. A mismatch counts **−1** but **doesn't clear** the person. Physical evidence (shoe, blood, hair, wound angle) still clears them.

### New tasks

| Task | Skill | What it does |
|---|---|---|
| Interview victim's friends, family & coworkers | People | Up to 1 relative (same surname), 2 friends (a shared evening place) and 2 coworkers; 2 people per day. May give where the victim was going (40%), a comment about an over-friendly person with the killer's sex and age range, a quarrel with someone (a red herring), or nothing useful. |
| Request phone records | People | 2 days. May show calls from the killer (25% of cases in police mode, 15% in killer mode), where the victim was going (60%), or a message about the killer's car (40%). |
| Background check | People | Hometown and years in the city, work history, an earlier name and an old record (both at skill chance for the killer), and people of a similar age (±6 years) from the same hometown. Innocent people: 12% have a minor old record and 4% were once questioned about a burglary. |
| Pull old incident reports near a place | People | Reports within a few streets. The killer has 3–5 earlier incidents near their home, work or evening places (sex right 80%; car mentioned 60% of the time and right 75%), mixed with unrelated ones (at least 6, more in big cities). |
| Interview a person's household | People | For the killer, it depends on the household's suspicion: under 40 they cover for them; 40–69 they admit a late night (breaks one alibi); 70 or more they describe late nights and hidden items, and say where things are hidden. |
| Check a person's finances | People | Shows a rented storage unit (the killer, if that's where things are; 10% of innocent people). |
| Search home / car / work locker / storage unit | Forensics | Each needs case strength 3+ and nothing clearing the person. Only the right place holds the killer's items. A car search may find fibres from a victim's clothing (60%). Searching an innocent person adds 5 pressure. |

### New evidence points

| Evidence | Points |
|---|---|
| Phoned a victim shortly before the death | 2 |
| Fibres from a victim's clothing in their car | 2 |
| Household member describes late nights and hidden items | 3 |
| Old record of similar behaviour | 1 |
| Age within the estimated range | 1 |
| Witness trait doesn't match | −1 |

## 6. The killer (police mode)

- **Origin file:** hometown, years in the city, an earlier name (sometimes), family background, school, past jobs, and an old police record of similar behaviour.
- **People from the past:** 1–2 residents from the same hometown within 3 years of the killer's age. Interviewed, they talk about someone they knew at school, sometimes by the old name, and say they may have seen that person at one of the killer's evening places.
- **Household suspicion:** +12 per killing, +8 when the press names the killer, +10 when police interview the killer, +8 per household interview, +10 when witness descriptions are released; −1 a day. At 85, the household member calls the tip line.
- **Where things are hidden:**

| Lives alone | Lives with others |
|---|---|
| home 35%, garage 20%, car 15%, storage unit 15%, outside 15% | car 30%, work locker 25% (if they have a job), storage unit 30%, outside 15% |

- **Hidden outside:** after 3 killings, there's a 3% chance each night that a dog walker finds the box. A partial print goes to the lab (3 days).

## 7. The press and the city

- **Press conference:** once every 3 days. You choose what to release: the signature, the cause of death, witness descriptions, or a public warning about who the victims have been.
  - Pressure drops by 15, plus 5 per item released. The killer's heat rises by 10, plus 5 per item.
  - Tips: 3, or 4 once the press has named the killer. Chance that one is about the real killer: 35%, plus 10% per item ever released, at most 75%.
  - **Releasing the signature:** copycat killings become possible (6% a night, at least 7 days apart). Each copycat is arrested 4–9 days later. Copycat scenes are kept out of the killer's profile, and examining the scene can reveal the item is slightly different.
  - **Releasing the warning:** 25% of people who fit the victim type stay home.
- **Press nickname:** after 2 linked cases, for example "The Paper Crane Killer". Public pressure then rises by 1 extra per day.
- **The city reacts:** each body adds 1 "fear" to its district, which fades by 0.1 a day. Each point of fear makes 10% of potential victims there stay home (at most 50%) and makes canvassing up to 30% more productive.
- **Neighbourhood patrols** form after 3 linked cases:
  - They're out in the district of the latest case on 30% of nights.
  - If the killer meant to strike there, they don't.
  - 15% of the time a patrol confronts an innocent person: public pressure +4.

## 8. Killer mode

### Free time

| Day | Free hours |
|---|---|
| Day off | 12 |
| Day-shift workday | 6 |
| Night-shift workday | 5 (can't act that night) |
| Evening-shift workday | 4 |

### Actions

| Action | Hours | Notes |
|---|---|---|
| Watch a place | 3 | Learn its regulars and staff, and their nights. Watching the same place twice makes you a regular on its records. |
| Watch a person | 2 | Their routine and whether they live alone. 12% chance a neighbour notices, which creates an incident report. |
| Plan tonight | 4 (6 with high care) | Person, place (or their home, if you know they live alone), care, keep something, leave a signature. |
| Be seen early | 2 | Tonight's alibi becomes "weak" instead of "unverified" or "contradicted". |
| Lie low | rest of day | Heat −10; household suspicion −5. |
| Move your things | 3 | Choose a new hiding place. Household suspicion +3. |
| Destroy what you kept | 3 | Permanent. |
| Write to the newspaper | 2 | Permanent. Public pressure +10; the postmark district goes on record. |
| Confide in someone | 1 | Permanent. Each Monday there's a 10% chance they call the tip line. |

### The night

- If the person isn't where you planned, nothing happens.
- A patrol in that district, a stakeout at the place, or a tail on you can stop the night: you may be caught, or you may notice and go home.
- **Care level** multiplies the traces left: low ×1.4, normal ×1, high ×0.55. High care adds 10% to the chance of a witness seeing your sex or car.
- **Urge:** starts at 20 and rises 7 a day (+2 if your pattern consistency is under 50%), to at most 120.
  - An act lowers urge by 70 × (0.35 + 0.65 × pattern fit).
  - **Pattern fit** compares the victim's sex, age decade, hair, living alone and type of place with your most common choices (once you have 2 or more acts).
  - At 100, the next free night happens on its own, with low care.
- **Household suspicion:** +12 per act. At 100 they turn you in, and the game ends.

### What you see

- News: a clinical one-line report of each body found, a headline, and the city's reaction.
- The press nickname, press conferences and patrols.
- **Signs** that the police are close: questions at your door, neighbours asked about you, a sample request, searches, a car following you, an unmarked car at a place, customer lists taken, detectives on your street, patrols nearby.

### The computer police

- Each day they work through: new scenes (autopsy, examine, canvass, the victim's circle, phone records), then the regulars lists for last-seen places, then suspects.
- **Suspects:** people on those lists on the right nights, plus people matching the known traits. They work the top 1–3 suspects in order: interview, alibis, background, blood sample, household, finances, then searches at strength 3+ and a charge at 7+.
- **Stakeouts and tails:** they stake out the most common last-seen place on matching nights, and tail the top suspect.
- **Press conferences** when public pressure is over 60.
- **Task force:** if public pressure reaches 100, a new task force takes over: every detective's skills go up by 1, and pressure resets to 50.

### End and score

- **The game ends** if you're convicted, caught in the act, or turned in.
- **Score** = (days free × 10 + quiet days × 5) × (1 + 0.3 × pattern consistency + 0.1 × each permanent risky choice).
  - **Risky choices:** using a signature, keeping things, writing to the newspaper, confiding in someone.
  - **Quiet day:** no signs of the police in the last 3 days.
  - **No points per victim.**
- The best score is kept on this computer.

## 9. Two-player (one computer)

- The killer player chooses a character privately.
- Each day: the killer's turn, a blank hand-over screen, the police turn, then the night resolves. Then another hand-over.
- **The police win** by a conviction or a catch in the act.
- **The killer wins** if public pressure reaches 100 and the police team is taken off the case.

## 10. Other

- **Save / Load:** 3 slots in the browser, plus a save file or copyable save text.
- **Timeline tab:** every event, oldest first, filtered by case or person.
- **Notes:** on cases and people. They show on the evidence wall.
- **Phones and tablets:** a single-column layout below 760 pixels wide.
