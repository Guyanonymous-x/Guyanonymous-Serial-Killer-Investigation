# Design: every rule and number (V3)

V1 (`DESIGN.md`) and V2 (`DESIGN_V2.md`) rules still apply unless changed here. All numbers are first guesses and can be changed.

## 1. Panels (desktop)

- Every area is a panel. Drag it by its title bar, resize it from the bottom-right corner, **▁** collapses it to its title, **✕** closes it, and clicking a panel brings it to the front.
- Edges snap to a **20-pixel grid**.
- Case files, City map, Evidence wall and Timeline are separate panels. Timeline starts closed.
- **Panels ▾** shows or hides any panel. **Layouts…** saves the current layout under a name, uses or deletes saved layouts, downloads or copies a layout file, loads one from a file or pasted text, and resets to the default.
- The last layout is kept automatically in the browser. Police and killer layouts are separate.
- The default layout is fitted to the screen size. Screens 760 pixels wide or less (phones) keep the single-column layout with tabs.

## 2. Killer mode

### Wealth and money

| Wealth | Start money | Weekly pay (Mondays, if employed) | Notes |
|---|---|---|---|
| Indigent | 0 | 0 | Sleeps at a shelter; no car; hides things outside; can beg (4h, +2–8); police look at you a little sooner |
| Poor | 20 | 30 | |
| Middle | 80 | 80 | Can buy poison |
| Comfortable | 250 | 150 | Faster travel (taxi) |
| Wealthy | 1,000 | 350 | Always a car; +2 free hours a day; police need warrant strength 4 to search you |

- **Storage unit:** costs 10 a week unless you're comfortable or wealthy. If you can't pay, it's cleared and its contents go to the police.
- **Steal:** 2h, +10–40. 8% chance you're caught and cautioned; police then have your blood type.
- **Rob a victim** (tick "take valuables"): wallet or purse 5–40 × (1 + victim's wealth level); at their home 20–150 × (1 + wealth level), plus goods to sell. A bank card is taken 60% of the time.
- **Use a stolen card:** 1h, +30–120. The bank reports where it was used, and police can pull CCTV (detective's skill chance: your sex, height ±5 cm and hair).
- **Sell stolen goods:** 1h, +10–40. 40% chance a pawn-shop record reaches the police 3–6 days later (+3 evidence).

### Free time and travel

- Free hours as in V2. A police officer has 2 fewer hours on shift days, and rotating shifts.
- Worn out (tiredness 6+): 2 fewer hours a day.
- Tiredness rises by 3 per act and falls by 1 a day.
- **Travel** from your home to the place, there and back: about 1 hour per 150 map units on foot or by bus, 240 by taxi (comfortable or wealthy), 360 by car.

### Watching

| Action | Hours | Effect |
|---|---|---|
| Watch any place | 3 | Learn everyone who works or spends evenings there, and their days. Going twice makes you a regular on its records. |
| Walk a district's streets | 3 | Learn 25 residents; for 40% of them, whether they live alone. |
| Watch a person | 2 | Their routine and whether they live alone. 12% chance a neighbour notices, which creates an incident report. |

### Planning a night

- **Where:** at a place where they are tonight; on their way home from that place, or from an evening shift; or at their home (only if you know they live alone).
- **Hours needed** = travel + 3 + the means' time + 2 for high care + ½ per precaution, rounded up.

| Means | Cost | Hours to get | Shop record | Time to use | Effect on traces |
|---|---|---|---|---|---|
| Bare hands | free | – | – | 1 | hair ×1.3, blood ×0.6 |
| Something found at the scene | free | – | – | 1 | unpredictable (each trace ×0.6–1.6) |
| Something heavy from home | free | – | – | ½ | blood ×1.3; 50% chance of traces on your clothes |
| Cord | 5 | 1 | 30% | 1 | hair ×1.1 |
| Blade | 15 | 1 | 40% | ½ | blood ×1.6; 80% chance of traces on your clothes |
| Poison | 40 (middle wealth or better) | 3 | 70% | 2 | shoe ×0.5, hair ×0.5, blood ×0.2, sex sighting ×0.5 |
| Your car | free (needs a car) | – | – | ½ | car sighting ×2.5, shoe ×0.2, hair ×0.3; on someone's way home only |

- A shop record is 30% more likely if you pay by card and 40% less likely with cash. Middle wealth and above pay by card 70% of the time.
- When police check shop records for the means used, the buyers they find are mixed with 4–14 innocent buyers (1–4 for poison).

| Precaution | Cost | Effect |
|---|---|---|
| Gloves | 5 | Blood ×0.25; nothing you dispose of carries your traces |
| Mask | 10 | Sex sighting ×0.6 |
| Shoe covers | 8 | Shoe print ×0.15 |
| Change of clothes | 15 | Hair ×0.5; leaves a bag of clothes to deal with |

- Care: low ×1.4, normal ×1, high ×0.55. High care adds 10% to sex and car sightings. Being worn out multiplies all traces by 1.2.

### Being seen where you act

- At a place: 30% (if it isn't a park) plus 25% if you act at the place itself, or 10% if you act on the route home. Being seen puts you on that place's records for that night (card payment, CCTV or staff memory).

### After an act

- **Urge** falls by 70 × (0.3 + 0.4 × desire match + 0.3 × pattern match). For the next 2 days it doesn't rise.
- **Desires:** two, set from your background (sex, age decade, hair, living alone, or kind of place). After each act there's a 25% chance one shifts to your most common choice for that attribute (once you've made it twice).
- **Things:** a kept item, a bag of clothes (from a change of clothes, or from a means with traces), and a means that now carries traces.

### Dealing with things

| Way | Hours | Chance found, per day | For |
|---|---|---|---|
| A street bin | 1 | 4% | 10 days |
| The river | 2 | 1% | 30 days |
| Burning it | 2 | 0.5% | 30 days (household suspicion +6) |
| Burying it | 3 | 1.5% | 40 days |
| A bin across the city | 3 | 2% | 10 days |

- If something is found and it carries your traces (no gloves), the lab gives the police your blood type, or your shoe size if they already have that.
- **Plant** (2h): in someone's home, car or bin, optionally with an anonymous tip. 10% chance someone sees you. Items in a bin are found the next day; items in a home or car are found if that person is searched.
- **Leave at a later scene:** the police find the earlier victim's item there, which links the cases.
- **Send** (2h, or 4h posted from another district): to the newspaper or a victim's family. Public pressure +15. The postmark goes on record, and without gloves the lab gets a trace.

### Police officer (as a job)

- **At the station** panel: the suspect board (including whether you're on it), what the police know, and canteen talk about planned stakeouts.
- **Misplace evidence** (2h, on shift): removes one known trait. 15% chance of an internal affairs inquiry.
- **Point colleagues at someone** (1h, on shift): that person gets extra police attention for 7 days. 10% chance of an inquiry.
- **Internal affairs inquiry:** +3 evidence against you, you go on the suspect board, and a search warrant needs only strength 2.

### Your stance

- **Blood samples:** refuse (as in V2) or give one.
- **Interviews:** keep your habits to yourself (police may catch the lie) or be open about where you go.
- In killer mode the chance of seeming evasive is halved.

## 3. The computer police in killer mode

- They re-pull a place's list when a new case points to it again.
- **Geographic profiling** from 3 cases: the centre of the scenes, with a radius of the average distance (50–110 map units). They canvass that area, and re-centre it if the scenes drift.
- **Blood screening** once the blood type is known and public pressure is over 50: everyone in the profile area of the right sex is asked. Innocent people refuse 15% of the time.
- They check shop records for each case's means, and check bank-card use.
- **Suspect weighting** adds points for: profile-area residents matching known traits (+2), refusing screening (+4), buying the means (+3), pawned goods (+5), an anonymous tip (+2), internal affairs (+6), steering by a police-officer killer (+4), planted items found (+4), and being indigent (+1).
- **New evidence points:**

| Evidence | Points |
|---|---|
| Refused a blood screening | 1 |
| Bought the means shortly before a killing | 1 |
| Sold a victim's property | 3 |
| An object at home matches the victims' wounds | 3 |
| Clothing with traces from a victim | 2 |
| Internal affairs: evidence tampering | 3 |
| Named in an anonymous tip | 0 |

- **Conviction in killer mode** needs strength 7 or more, nothing clearing the person, **and at least one hard piece of evidence**: blood type, the signature items, a victim's belongings, the weapon, clothing with traces, pawned goods, fibres, a household statement, phone contact, or being caught.
- New police tasks, also available to the police player: **blood screening drive in a map area**, **check shop records for the means used**, **trace use of the victim's bank cards**.
- **Signs for you:** with public pressure over 50, a 30% chance each day of noticing more police around your district.

## 4. Other changes

- The press nickname in killer mode uses the district (or "Night") when you leave no signature.
- Case files show when no signature item was found, when an earlier victim's item was left at a scene, and when valuables were taken.
- A Central Police Station exists in every town.
