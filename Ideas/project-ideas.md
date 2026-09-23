# Project ideas

Drafted 23 September 2026 for a team of three with an engineering and robotics
background. Dates and rules come from `../Resources/competition-brief-2026-09-23.md`.
Nothing here has been tested yet: every problem size is either sourced or marked as an
assumption, and each idea ends with the cheapest experiment that would tell us whether
it holds up.

## How to read this

The competition runs about eleven weeks from kick-off to final, with three deliverables in
between, and the previous winner was a working hardware prototype (a blind-spot helmet).
So each idea is judged on five things:

- **Theme fit**: does it answer the organiser's question in plain words?
- **Demo on 9 December**: can we show it working on stage, live, in under a minute?
- **Buildable by three students in eleven weeks** with no budget before the prize.
- **Crowdedness**: how easily can a juror say "that already exists"?
- **Cheapest test**: how fast can we find out if it is a bad idea?

## Summary

| # | Idea | Theme | Demo | Buildable | Crowded | Cheapest test |
| :---- | :---- | :---- | :---- | :---- | :---- | :---- |
| S1 | Hedgehog-safe robot mowers | Sustainability (animal protection) | Strong | Medium | Low to medium | One evening |
| S2 | Old phones as nature sensors | Sustainability (circular + nature) | Medium | High | Medium | One night |
| S3 | Litter map from your bike ride | Sustainability (waste, plastic) | Medium | Medium | Medium | One ride |
| P1 | Referee whistle to wrist for deaf players | Sport (inclusion) | Strong | High | Low | One evening |
| P2 | Heading counter for youth football | Sport (safety) | Medium | Medium | Medium | One training |
| P3 | Solo training partner for wheelchair tennis | Sport (access) | Strong | Low | Medium | Two hours of calls |

The grades are our judgement, not measurements. Re-grade after each test.

## Sustainability & Tech

### S1. Hedgehog-safe robot mowers

- **Problem.** Hedgehogs are active at night and roll up instead of fleeing, and robot
  mowers increasingly run at night. Wallonia banned robot mowers between 18:00 and 9:00
  in 2025 to protect them; the Netherlands has no such rule (NOS, 10 April 2026).
  Stichting Egelopvang Midden-Nederland took in about 900 hedgehogs in 2025 and reports
  cut wounds on the back and head (same article). How many of those are mower injuries is
  **not established**: a Danish researcher noted wounds can also come from other garden
  tools or dogs (Egelwerkgroep, Aalborg University study).
- **Idea.** A small retrofit module (camera plus a cheap thermal sensor) that spots a
  hedgehog-sized warm body in front of a mower and stops it, or an add-on that enforces a
  night lock on mowers that support scheduling through an app.
- **Why us.** Sensor fusion and a moving robot is robotics-team work, and a small rover
  stopping in front of a hedgehog dummy on stage is a memorable demo.
- **Cheapest test (one evening).** A hot-water bottle in a brown sock in the grass at dusk.
  Point a phone camera and, if one of us has it, a cheap thermal sensor at it from 50 cm
  and 1 m. Does a pretrained detector or a simple temperature threshold find it without
  firing on leaves? Plus 30 minutes reading the published results of the Aalborg study and
  checking whether current mowers already claim animal detection.
- **Risks.** Mower makers may already ship detection (check first). Retrofitting a closed
  mower is hard, so the realistic prototype might be our own rover, which is a weaker
  claim than "works on your mower".

### S2. Old phones as nature sensors

- **Problem.** Working smartphones end up in drawers, while bird and bat counts in parks
  and schoolyards depend on volunteers counting by hand now and then. How many phones sit
  unused in Dutch homes is an **assumption** to source.
- **Idea.** An app plus a weatherproof, solar-fed enclosure that turns an old Android
  phone into an always-on sound monitor. It recognises bird calls on the device and posts
  daily species counts to a shared map for a school, park or municipality.
- **Why it fits Samsung.** Samsung ran a Galaxy Upcycling programme to give old phones a
  second life, and critics said it was scaled back (iFixit, Android Police). A student
  team showing the idea working in the field is a direct answer to that.
- **Cheapest test (one night).** One old phone, an existing bird-recognition app (BirdNET
  has one), on a balcony or in a garden overnight. Measure battery used per hour and count
  how many detections look plausible.
- **Risks.** Continuous bird monitoring on a Raspberry Pi (BirdNET-Pi) already exists, so
  our case rests on "the hardware is already in your drawer". Android background limits,
  heat and rain can kill it.

### S3. Litter map from your bike ride

- **Problem.** Cleanup groups and municipalities do not know where litter piles up until
  someone reports it by hand.
- **Idea.** A phone on the handlebar films the road edge, an on-device model spots litter,
  and every find is logged with GPS into a heat map. Riders earn points, cleanup groups get
  a map. Bridges both themes: movement and waste.
- **Cheapest test (one ride).** Film one 20-minute ride through Delft or Den Haag, run an
  off-the-shelf litter detector (trained on the public TACO litter dataset) on the frames,
  and count hits and false alarms by hand.
- **Risks.** Motion blur. Filming the street catches faces and number plates, so frames
  must be processed on the phone and thrown away (GDPR). Apps where people photograph
  litter by hand already exist. Whether a municipality would use the map is unknown: one
  email to a local cleanup group answers it.

## Sport & Tech

### P1. Referee whistle to wrist for deaf players

- **Problem.** Deaf and hard-of-hearing players in mixed amateur teams miss the whistle and
  keep playing. How often this causes problems is an **assumption**: it needs deaf players
  or a deaf sports club to confirm it.
- **Idea.** A phone on the sideline (or the referee's watch) detects the whistle and makes a
  band on each deaf player's wrist vibrate within a fraction of a second, with different
  patterns for stop, goal and end of half.
- **Why us.** Audio detection, low-latency wireless and haptics: small, buildable and very
  demonstrable. It answers "more accessible" and "more inclusion" directly.
- **Cheapest test (one evening).** A phone app that listens for a whistle and buzzes a
  paired watch or a second phone. Measure delay and false triggers with crowd noise played
  from a speaker. The same week, message one deaf sports club and ask whether this is a
  real problem for them.
- **Risks.** Sports rules on wearing anything on the wrist during matches (to verify per
  sport, football is strict on jewellery). Several whistles on neighbouring pitches.

### P2. Heading counter for youth football

- **Problem.** Repeated heading is linked to later brain disease in former professional
  players (University of Glasgow FIELD study, 2019), and England and Scotland limit heading
  in youth training. Whether Dutch clubs have such limits is **not checked**.
- **Idea.** A light sensor in a headband or cap clip counts headers per player per session
  so a coach can keep to a limit.
- **Cheapest test (one training).** Tape a phone or watch to a headband, head 20 balls, then
  jog and jump for five minutes. Do headers stand out clearly in the accelerometer data?
- **Risks.** Commercial head-impact sensors exist, though aimed at professionals. Must never
  be presented as a medical device.

### P3. Solo training partner for wheelchair tennis

- **Problem.** Wheelchair players need a partner or coach to feed balls, which limits how
  often they can train. An **assumption** to check with players.
- **Idea.** A low-cost ball feeder, steered from a phone, that adapts placement to the
  player's chair movement and logs sessions.
- **Cheapest test (two hours).** Call two wheelchair tennis clubs and ask how players train
  alone today, and price existing tennis ball machines.
- **Risks.** Ball machines already exist, so the "adapted" part has to be real. The most
  mechanical build of the six, and the hardest to finish in eleven weeks.

## Recommendation

**Lead with S1, hedgehog-safe robot mowers, with P1 as the backup**, provided the
30-minute check does not show that mower makers already solved it. Reasons: animal
protection is named in the theme, there is a live Benelux policy story (Wallonia's ban,
the Netherlands not following), our robotics background shows, and the stage demo is
unforgettable. P1 is the backup because it is the smallest build and the least crowded,
but it lives or dies on whether deaf players say the problem is real.

Plan until deliverable 1:

1. **Before 1 October:** register the team on Soapbox and read what the form asks for.
2. **Before 14 October (kick-off):** run the S1 and P1 cheapest tests, one evening each,
   and write the results into `../MEMORY.md`.
3. **By 21 October (deliverable 1):** pick one, record why in Key Decisions, drop the rest.

This recommendation does not yet account for the two teammates' skills and interests.
If either of them brings a strong sport, biology or design background, re-rank before
testing.

## Sources

- [Samsung Solve for Tomorrow NL](https://www.samsung.com/nl/explore/brand/solve-for-tomorrow/)
- [Soapbox challenge page](https://soapbox.nl/challenges/challenge-yHRcBY86HvIM/)
- [Samsung Newsroom NL, launch 2026](https://news.samsung.com/nl/samsung-electronics-benelux-opent-jacht-op-de-beste-studenten-ideeen-voor-solve-for-tomorrow-2026)
- [NOS: Egels in Wallonie beschermd tegen robotmaaiers, Nederland volgt nog niet](https://nos.nl/artikel/2609904-egels-in-wallonie-beschermd-tegen-robotmaaiers-nederland-volgt-nog-niet)
- [VRT NWS: Wallonie verbiedt robotmaaiers tussen 18 uur en 9 uur](https://www.vrt.be/vrtnws/nl/2025/07/03/wallonie-robotmaaiers-egels/)
- [Egelwerkgroep: onderzoek naar robotmaaiers en egels](https://www.egelwerkgroep.com/post/nieuw-onderzoek-naar-robotmaaiers-en-egels)
- [iFixit on Galaxy Upcycling](https://www.ifixit.com/News/50450/samsung-galaxy-upcycling-unlocked-smartphone-smarthome-project)
