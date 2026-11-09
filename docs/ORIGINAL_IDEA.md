# The original idea

*Dave's idea, held for about 20 years, as he described it in November 2026 (lightly tidied):*

It is not a first-person game, and not especially about graphics. It isn't a traditional text game either. It's closer to a management or incremental game.

**You are the police.**

A city of at least a few thousand, up to a few hundred thousand, people is created. The game keeps track of each individual: qualities about them, their job, and where they are through the day and night (going to work on work days, for example).

The serial killer is given characteristics: what makes people targets (if anything), what situations prompt the act, their pattern and methods, and their beginnings (the first acts).

The police's job is to use a skill or search out evidence each turn, narrowing down who the killer is by investigating and piecing things together.

People have names. Victims are people with richly detailed backgrounds, lives and behaviours, and all of those details are used to identify the killer's patterns.

# Design decisions so far

| Question | Decision |
|---|---|
| Who is the player? | The whole police department, not one detective. |
| Does the killer react to the police? | Yes. They adapt when the police get close. |
| How does a case end? | An arrest, then a court case. You need enough evidence to convict. |
| First step | A small playable prototype in the browser. |
| City size | Started at 500 people. Raised to 2,000 for V1. |
| Map | A city map showing places, bodies, where victims were last seen, and the homes of people of interest. You can draw an area and canvass it. |
| People of interest | Marked wherever they appear (lists, search results, the log). |
| Connections | An evidence wall with strings joining victims, people, places and facts, like a detective's corkboard. |
| Surveillance | Possible on places (stakeouts) and on people (tailing). |
| Neighbourhood gossip | Included in area canvasses: a mix of true and false. |
| Tailing odds | The best surveillance detective catches the killer about 55% of the time on a hunting night. |
| Area canvass size | Bigger areas take more days (about one detective-day per 60 homes). Progress is kept if stopped, detectives can share the work, and a finished canvass is as thorough as a small one. |
| Name | Guyanonymous' Serial Killer Investigation (for now). |

# Ideas from the first discussion, not yet built

- More kinds of victim type, and a messier "first kill" stage.
- Richer victims' lives: friends, family and coworkers to interview, diaries, phone records.
- Larger cities (tens or hundreds of thousands of people), filling in detail only when a person becomes relevant.
- A city-size choice when starting a new case.
