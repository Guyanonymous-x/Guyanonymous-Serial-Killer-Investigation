# Design: every rule and number (V1)

All of these are first guesses for the prototype and can be changed. Percentages are chances, rolled each time.

## Time

- One turn is one day. Day 1 is a Monday.
- During the day, each detective does one task. At night, the killer may act. In the morning, any body is found.

## The city

- **2,000 residents** in **6 districts** (Northgate, Old Town, Hillcrest, Harbor, Market, Riverside) and **55 places**.
- **Jobs:** each workplace has set jobs, shifts and staff numbers. Shifts are day, evening or night. Offices and schools on day shift work Monday to Friday; everyone else works 5 random days a week. Staff numbers at workplaces are 2.5 times the base list; bars and other hangouts keep their base numbers.
- **People without a workplace:** 16% students (18–23), 34% retired (64–86), 24% between jobs, stay-at-home parents or carers, 26% self-employed (day work, Monday to Friday).
- **Evening habits:** 25% have none, 45% have one place, 30% have two. Each habit is 1–2 fixed evenings a week, never on nights they work evening or night shifts. People over 64 stick to quieter places (church, library, community centre, park, café, diner, bowling, cinema).
- **Looks:** height is around 177 cm (±7) for men and 164 cm (±6) for women. Shoe size follows height. Hair: black 30%, brown 35%, blonde 20%, red 7%. Over-56s are grey 60% of the time.
- **Blood types:** O+ 37%, A+ 34%, B+ 9%, O− 7%, A− 6%, AB+ 3%, B− 2%, AB− 1%.
- **Cars:** 66% own one (30% for over-75s). Colours: white, black, silver and grey are common; blue and red less so; green, maroon, brown and yellow are rare.
- **Lives alone:** 33% (50% for over-64s, 15% for students).
- **Names:** every resident has a different full name.

## The killer

- One resident aged 25–55, never someone who works evening shifts.
- Lives alone 70% of the time. Has a car 60% of the time even if they didn't before.
- **Victim type:** one sex, plus one of: an age band (20–30, 28–40 or 40–60), a hair colour, or living alone. At least 60 residents must fit the type.
- **Hunting places:** two of their own evening places (bars, diners, gyms, laundromat, parks, cinema, bowling, library, café), each on two set nights. They hunt at one place at a time.
- To make the pattern findable, 7 people who fit the victim type are made regulars at each hunting place on the killer's nights.
- **Timing:** first gap between killings is 6 days, shrinking by 1 after each kill, down to 2. They only strike on a night they go to their current hunting place.
- **Time of death:** between about 23:00 and 03:00.
- **Victim choice:** someone of their type who is at the hunting place that evening (regular or evening staff). If there's no one, someone of their type who lives in that district.
- **Scene:** if the victim lives alone, 45% at their home; otherwise near the hunting place.
- **Signature:** the same item left at every scene (a paper crane, a chess pawn and so on). **Method:** the same each time. **Trophy:** an item taken from each victim.
- **Traces left per killing:** shoe print 60%, blood 45%, hair 45%, wound angle showing height 70%, witness who saw their sex 45%, witness who saw their car 40% (if they have one), a friend who remembers an over-friendly person 35%.
- **Gloves (no blood):** when heat is 40 or more, or 30% of the time after 3 kills.

### Heat (how close the killer feels you are)

| Event | Heat |
|---|---|
| Interviewed | +30 |
| Alibi checked | +10 |
| Asked for a blood sample | +15 |
| Spots a stakeout or a tail | +25 |
| Home searched | +40 |
| Press conference | +10 |
| Tailed on a night they don't hunt | +15 (40% of the time) |
| Each day | −5 |

- Heat 60+ at a killing: moves to the other hunting place afterwards (heat −15).
- Heat 80+: lies low for 4 days (once per case, heat −20).
- Spots surveillance: skips that night, tries again 2 days later, and moves if heat is 50+.

## Your department

| Detective | Forensics | People | Surveillance |
|---|---|---|---|
| Ruth Okafor | 3 | 1 | 2 |
| Sam Brandt | 1 | 3 | 2 |
| Lena Vasquez | 2 | 2 | 1 |
| Marco Hale | 1 | 2 | 3 |

**Skill chance** = 30% + 20% per level, so level 1 = 50%, level 2 = 70%, level 3 = 90%.

## Tasks

| Task | Skill | What it does |
|---|---|---|
| Examine crime scene | Forensics | Finds shoe print, blood (at 80% of the usual chance) and hair. Halved after the scene is more than 2 days old. Can repeat. |
| Attend autopsy | Forensics | Once per case. Gives cause and time of death. May give the attacker's height range (skill chance +10%). |
| Canvass witnesses & friends | People | Where the victim was last seen (skill chance +15%, max 95%), witness sightings, a friend's memory (at 80%). Repeats are at 60%. |
| Pull staff & regulars list | — | Always works. Lists everyone who works at or frequents a place, and on which days. |
| Interview a person | People | Reveals hair, possibly shoe size, evening habits and demeanour. The killer leaves out their hunting places; seems evasive 30% + 20% per People level. Innocent people seem nervous 12% of the time. |
| Check their alibis | People | Needs an interview first. See Alibis below. |
| Request a blood sample | People | Innocent people agree 85% of the time. The killer always refuses. |
| Night stakeout at a place | Surveillance | If the killer hunts there that night: caught 20% + 20% per level; otherwise 60% they spot you. Also notes who was there. |
| Tail a person tonight | Surveillance | Shows where they went. If it's the killer on a hunting night: caught 10% + 15% per level; otherwise 50% they spot you; otherwise you lose them. |
| Canvass a map area | People | See Area canvasses below. |
| Seek warrant & search home | Forensics | Needs case strength 3+ and nothing clearing them. The killer's home always has signature items; trophies are found at 90% (50% if heat is 70+), adjusted by skill. Searching an innocent home adds pressure. |

### Alibis

- Innocent person on night shift that night: **confirmed** by timesheet. This clears them.
- Innocent person who lives with others: **weak** (household confirms).
- Innocent person who lives alone: **unverified**.
- Killer who lives alone: **contradicted** 30% + 15% per People level (a neighbour saw or heard them go out), otherwise unverified.
- Killer who lives with others: **contradicted** 50% + 15% per level (partner admits they went out), otherwise weak.

### Area canvasses

- Draw a circle (radius up to 120 map units; the whole map is 900 × 600). It needs about **one detective-day per 60 homes** inside it, at least 1.
- The circle is split into equal slices, one per day. Each detective-day completes the next slice. Several detectives can work it on the same day. Progress is kept if you stop.
- Each slice can turn up, at full strength regardless of circle size:
  - Night sightings (sex, car colour) if a crime scene is in the slice (skill chance).
  - Doorbell-camera footage (car colour or a height range, 35%, once per case) if the killer's route from the scene to their home crosses the slice.
  - Neighbours noticing someone who comes home at 2–3am on the killer's nights (skill chance × 0.8) if the killer lives in the slice.
  - **Gossip** (65% per slice). If the killer lives in the slice, 45% of gossip is true and about them. Otherwise it's about a random resident: night-shift workers are said to come and go at all hours (true but misleading); others get a true harmless habit (50%) or a made-up suspicion (50%).
- A finished area can be canvassed again only after a new body is found.

### Press conference

- Every 3 days. Pressure −15, killer heat +10.
- 3 tips. 35% of the time, one of them is about the real killer.

## Evidence and court

**Case strength** for a person adds up:

| Evidence | Points |
|---|---|
| Sex matches a witness | 1 |
| Height within the known range | 1 |
| Car colour matches | 2 |
| Shoe size matches | 2 |
| Hair colour matches | 1 |
| Blood type matches | 2 |
| An alibi contradicted | 2 |
| A regular, on that weekday, at a place where a victim was last seen | 1 per place |
| Didn't mention a place they're known to frequent | 1 |
| Seemed evasive or nervous | 1 |
| Refused a blood sample | 1 |
| Signature items found at home | 3 |
| Each victim's belonging found at home | 2 |
| Caught in the act | Automatic conviction |

**Clears them:** any known trait that doesn't match, or a confirmed (timesheet) alibi.

- **Warrant:** strength 3+ and nothing clearing them.
- **Conviction:** strength 7+ and nothing clearing them.

## Public pressure

- Starts at 20. +2 every day. +12 for each new body.
- Searching an innocent home: +5. Acquitting the real killer: +20. Acquitting an innocent person: +25.
- Convicting an innocent person: −40 at first, then +40 when the next body appears.
- Warnings at 50, 75 and 90. **At 100 you're taken off the case.**
- In testing, a player who does nothing loses around day 23, after about 4 victims.
