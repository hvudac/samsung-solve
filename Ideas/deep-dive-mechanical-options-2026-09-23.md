# Deep dive: the four options for a mechanical engineering team

Researched on 23 September 2026 for our team of three mechanical engineering students.
It covers the four options from `project-ideas.md`: X1 rubber-infill catcher, S6 beach
pellet separator, S1 mechanical hedgehog guard and P3 solo training partner for
wheelchair tennis. Every fact carries its source. Anything we could not confirm is marked
**unverified**, and our own estimates are marked as such. Competition dates are in
`../Resources/competition-brief-2026-09-23.md`.

## Verdict

The research changed the order. **S1 (mechanical hedgehog guard) is now the strongest
option.** X1 has a weak spot we did not know about. S6 is crowded. P3 depends on
interviews we have not done.

| Rank | Option | Verdict in one line |
| :---- | :---- | :---- |
| 1 | **S1 Mechanical hedgehog guard** | Peer-reviewed proof of the problem, a published test protocol we can use as our jury-proof measurement, and the mechanical route is open while brands chase cameras |
| 2 | **X1 Rubber-infill catcher** | A real Dutch legal pressure, but shoes carry only about 2.5% of the infill that escapes, and exit mats may not work. Worth it only as a measuring device or if we move to the bigger loss routes |
| 3 | **P3 Wheelchair tennis training partner** | Strong Dutch story, but cheap app-controlled ball machines already exist. Only worth it if players tell us ball collection or two-bounce feeding is their real problem |
| 4 | **S6 Beach pellet separator** | Crowded: at least two teams of mechanical engineering students have already built this, plus commercial machines. Drop unless we find a clear gap |

---

## S1. Mechanical hedgehog guard for robot mowers

### The problem, with evidence
- **No mower detects small hedgehogs.** Aalborg University tested 18 robot mowers with
  dead hedgehogs in 216 tests. None detected a hedgehog before touching it, "not even models
  with camera vision and ultrasonic sensors", and none detected dependent juveniles under
  200 g, which mostly passed underneath (Rasmussen et al., *Animals* 2021).
- **Height is what decides injury.** A follow-up with 19 models found only one mower, once,
  detected a carcass without touching it (Rasmussen et al., *Animals* 2024).
- **Hedgehogs freeze rather than flee.** In 100 tests with 50 live hedgehogs, only 1%
  curled up fully and 15% ran away; most stayed where they were (*Animals* 2024, behaviour
  study). So a guard cannot rely on the animal moving.
- **Injuries are serious.** In Germany, 370 hedgehogs injured by garden tools were recorded
  between June 2022 and September 2023, and 47% died (Leibniz-IZW).
- **The species is declining.** The IUCN moved the European hedgehog to Near Threatened on
  29 October 2024 (Hedgehog Street). Egelbescherming Nederland estimates the Dutch
  population fell about 75% over 50 years; the annual sighting count fell from about 13,000
  in 2024 to about 9,300 in 2025 (Nature Today). The sighting count is not a population
  estimate.

### Policy momentum
- **Wallonia** adopted a ban on robot mowers between 18:00 and 9:00 on 9 April 2026, with
  exceptions for sports fields and airports (Walloon environment department).
- **Germany:** Cologne since 1 October 2024 (dusk to dawn), Erlangen since February 2026
  (19:00 to 8:00), and several other cities and districts (city websites; the wider list is
  from a secondary source).
- **Netherlands:** no municipal ban as of April 2026 (NOS). A Tweede Kamer motion on
  hedgehog measures was reportedly adopted in June 2026 (**unverified**). Egelbescherming
  Nederland prefers education over bans: "just run the mowers during the day".

### What exists already
- **Safer features are known.** Pivoting blades, skid plates and front-wheel drive clearly
  reduced damage (Rasmussen 2021). Most mowers detect obstacles only by contact, through a
  floating body shell with magnet sensors.
- **Brands are going for cameras.** Husqvarna announced AI vision with infrared night vision
  for 2026, and Segway Navimow claims 95% hedgehog avoidance in its own tests, with an
  "Animal Friendly Mode" that also defaults to daytime mowing (company and trade sources).
- **A test standard is forming.** Aalborg and Oxford proposed a standard test: a small dummy
  (under 400 g, 7 cm high) and a large one (over 600 g, at least 10 cm high), 20 runs from
  each of three angles on a coconut mat, mower starting 3 m away (*Animals* 2024; Oxford,
  January 2024). In Germany, IZW and the crash-test firm CTS built heated dummies and are
  working towards a DIN standard (number **unverified**).
- **One retrofit failed.** A German aftermarket perforated guard for the Husqvarna 450X
  stopped the mower from docking (robomaeher.de).
- **Safety standard gap.** The mower safety standard (IEC 60335-2-107) tests with foot probes
  shaped like people, not animals. Probe forces and dimensions are **unverified** (paywalled).

### What would be new
A **low-force retrofit front skirt or guard** that reaches below 7 cm, still lets the mower
dock, and is **tested with the published dummy protocol**. Cameras are crowded; a tested
mechanical retrofit for the millions of contact-only mowers already in gardens is not. A
quick patent check found nothing specific, but a proper Espacenet search is still needed.

### The mechanical engineering work
- Skirt geometry and material (flexible PETG, TPU or rubber flaps) so a 7 cm, 180 to 400 g
  dummy is stopped or pushed aside before it reaches the blade disc.
- Force path: the skirt must transfer a very small contact force into the existing shell
  sensor, or trigger its own microswitch.
- Clearance: works on grass and slopes, does not snag, still docks.
- A test rig: the published dummy protocol, a force gauge, and paint on the dummy so any
  blade contact shows.

### Cheapest test (one weekend)
1. Borrow a basic contact-only mower.
2. Make dummies to the published size classes (sand-filled silicone or clay over a form).
3. Run the stock mower: how often does the small dummy pass underneath or get marked?
4. Measure the force needed to trigger the shell sensor, and the force a 180 g dummy on
   grass resists before sliding.
5. Fit a cardboard or PETG skirt and repeat three angles, 20 runs each. Check docking.

**Kill result:** the small dummy is still run over, it gets pushed ahead without triggering
a stop, the skirt snags or false-triggers on grass, or docking fails.

### Stakeholders
Egelbescherming Nederland and local hedgehog shelters (Stichting Egelopvang
Midden-Nederland), Dr Sophie Lund Rasmussen (Aalborg and Oxford), mower owners for a borrowed
machine, and possibly a mower dealer.

### Pitch hook
"No robot mower on the market can see a baby hedgehog. We made one stop for it, and proved
it on the scientists' own test."

---

## X1. Rubber-infill catcher for artificial pitches

### The problem, with evidence
- **How much escapes.** A Dutch systematic review estimates about 950 kg of infill escapes
  each pitch per year (range 570 to 2,280 kg), or about 1,778 kg including snow clearing
  (Kole et al., Open Universiteit, 2023).
- **Shoes are a small route.** By route: snow clearing 47%, brushing and maintenance 32%,
  grass verges 11%, runoff 7%, **players' shoes and clothing 2.5%, about 46 kg a year** (same
  review).
- **Per player** it is roughly 0.6 g on a dry pitch and 1.35 to 2.2 g on a wet one
  (Norwegian and Swedish studies, via Verschoor et al. 2021).
- **Exit mats may not work.** In the same review, players who crossed a walk-out mat still
  carried about as much granulate as those who did not, which "raises doubts about the
  effectiveness of a walk-out mat".
- **Scale.** The Netherlands has more than 1,800 artificial football pitches, about 90% with
  rubber (SBR) infill (KNVB), or about 2,200 football and 1,000 hockey pitches (BSNC 2024).
  EU-wide, infill is the largest single source of intentionally added microplastics, up to
  16,000 tonnes a year (ECHA).

### The Dutch pressure
- **EU ban from 2031.** The EU bans placing this infill on the market from 17 October 2031,
  and existing stock may still be used after that. There is no reporting duty for pitch
  owners (EU Regulation 2023/2055).
- **The real pressure is the Dutch duty of care for soil (zorgplicht).** The Raad van State
  ruled in October 2022 that rubber infill is only allowed with "adequate measures". Stichting
  InStrepitus has forced enforcement in Putten, Ermelo, Zwolle, Katwijk, Tilburg, Ede and
  other municipalities (Raad van State; Zembla).
- **The guidance already prescribes cleaning zones.** BSNC's 2024 guidance asks for exit
  zones at least 150 cm deep (two steps on a grate or mat), kickboards of at least 20 cm,
  drain filters and regular gully cleaning.
- **What it costs today.** Assen fitted kickboards and cleaning grates with catch trays on
  13 pitches for €160,000 (2020).

### What exists already
Boot scrapers with brushes (Manshanden, NL), football shoe cleaners (Sodex Sport), and
standard clean-walk grates. **None measure or weigh what they catch**, and none prove they
work. That gap is real.

### What would be new, and the honest catch
- The **measuring and proving** part is new: a station that tells a club or municipality
  how many grams it kept on the pitch is evidence for its duty of care.
- The catch: shoes are only 2.5% of losses, so a boot station alone cannot be pitched as
  the fix. Two ways to handle that:
  1. **Position it as the measuring instrument**, the thing that makes the problem visible
     and proves whether exit zones work, which the review doubts.
  2. **Pivot to the big routes:** a capture attachment for the maintenance brush (32%) or
     for snow clearing (47%). Much bigger impact and still mechanical, but we have **not
     researched** what turf-maintenance machines already recover.

### The mechanical engineering work
Brush and air-jet layout, separating granules from sand, grass and mud (sieve, then
drying), a catch tray on a load cell. Our own estimate: about 600 visits a week at 1 to 2 g
each is 0.6 to 1.2 kg a week, so a 5 kg load cell with about 1 g resolution is enough. Water
and mud in the catch are the bigger design problem.
- **Density note:** solid SBR is often quoted at about 1.1 to 1.2 g/cm³ (**unverified**). If
  so, it sinks in water, so flotation would separate out turf fibres, not the rubber.

### Cheapest test (one wet and one dry training)
Have 20 or more players each stand on a tray over a 0.5 mm sieve and brush their boots.
Dry the catch, sieve it and weigh it on a 0.1 g kitchen scale. Record grams of SBR per
player, the share that is rubber versus sand and dirt, and seconds per player. If the club
has a mat, compare players who crossed it with players who did not.

**Kill result:** well under 0.5 g of rubber per player, a catch that is mostly mud, players
unwilling to spend 5 seconds, or no better than the existing grate. **Pass result:**
consistently 1 to 2 g per player, mostly rubber. Both thresholds are our suggestion, not
from a study.

### Stakeholders
BSNC, KNVB Assist, Vereniging Sport en Gemeenten, Unie van Waterschappen, municipalities
under enforcement pressure (Assen, Zwolle, Katwijk, Tilburg), local clubs, Stichting
InStrepitus.

### Pitch hook
"Every Dutch municipality must prove it keeps rubber on the pitch. Nobody measures it. We
do."

---

## P3. Solo training partner for wheelchair tennis

### The Dutch context
- **The Netherlands dominates the sport.** Esther Vergeer (7 Paralympic golds, 21 Grand
  Slam singles titles), Diede de Groot (24 Grand Slam singles titles, Golden Slam 2021),
  Niels Vink (3 Paralympic golds, including Paris 2024 quad singles; Parasportsman of 2025).
  The elite train at the National Tennis Centre in Amstelveen, and KNLTB appointed Amanda
  Hopmans as national coach in December 2024.
- **The grassroots base is small and shrinking.** About 500 players in 2018, about 100 at
  ranked level, and "still falling" (Stichting BRNL blog). An older article gives 600 to 700
  players at about 32 clubs. There is no current KNLTB figure (**unverified**).
- **Known barriers:** few accessible lessons and facilities, regional programmes stopped, a
  sports chair costs about €3,000 (2018). **A lack of hitting partners as a barrier is
  unverified**, and it is the assumption this whole idea rests on.

### Rules and training
The ball may bounce twice, and the second bounce may land outside the court (ITF). Coaches
train the "mobility cycle": keep moving, push to the ball, hit, recover. About 80% of strokes
need less than 2.5 m of movement (Georgia Tech wheelchair tennis robot study). Players
already train with ordinary ball machines, and there are published wheelchair drills for
them.

### What exists already
- **Ball machines are cheap and smart now.** SIBOASI T2303M has app and remote control, 21
  programmable points and a random mode. Slinger Bag costs $749, Lobster Elite Two $1,599,
  Spinshot Player HS $2,179 with an app and random mode. Sportbot moves around the court.
  The autonomous Tennibot Rover ball collector costs $2,275.
- **Nothing is designed for wheelchair users.** We found no ball machine built for them.
- **Universities have been here.** A Wisconsin launcher for quad players (2016), Georgia
  Tech's "ESTHER" wheelchair tennis robot, a $169 ball-collecting robot at UC Berkeley. TU
  Delft (Van der Slikke, Bregman) measured wheelchair tennis movement with KNLTB in 2017.

### What would be new
Not app control or random placement, which already exist. What would be new: low cost
**plus** feed logic built for two bounces and the mobility cycle (timing set by how long the
chair takes to reach the ball and recover), **plus** ball collection and reloading that work
from the chair. If players say collection is the real pain, pivot to a collector that works
from a wheelchair.

### The mechanical engineering work
A two-wheel counter-rotating launcher (spin from different wheel speeds), a feed mechanism,
aim and oscillation, and a collector or hopper you can reach from a chair. Our own estimate:
a 100 mm wheel at about 20 m/s surface speed needs about 3,800 rpm, within a 12 V, roughly
200 W budget. The Georgia Tech study found about 8 m/s was enough for wheelchair feeds. Ball
data: 56.0 to 59.4 g and 6.54 to 6.86 cm across (ITF). Safety: nobody reaches into a running
launcher.

### Cheapest test (two weeks, no cost)
Interview three to five club players and two coaches: how do you train now, would you
practise alone, what stops you? Then a "Wizard of Oz" session: one of us feeds balls by hand
following patterns picked by a phone app (or we borrow a club machine), and we watch where it
breaks: placement, timing, reloading, collection.

**Kill result:** players already have enough partners or coach time; the real barrier is
transport, chair cost or court access; or an off-the-shelf machine for €700 to €2,000 works
fine for them.

### Stakeholders
KNLTB (national coach Amanda Hopmans), TU Delft Sports Engineering Institute, Uniek Sporten
(club finder), Gehandicaptensport Nederland, Fonds Gehandicaptensport, Stichting BRNL.

### Pitch hook
"The Netherlands produces the best wheelchair tennis players in the world, and fewer and
fewer people are starting the sport. We built the partner that is always available."

---

## S6. Beach pellet separator

### The problem, with evidence
- **The MSC Zoe container spill (January 2019)** included 22.5 tonnes of polystyrene
  pellets. More than 24 million were counted on the Wadden islands, and WUR/NIOZ found
  about 85% settled to the seafloor, because polystyrene sinks (Stichting De Noordzee;
  WUR/NIOZ).
- **Pellets are common on Dutch beaches.** They were found in 38% of De Noordzee's beach
  litter surveys (2018), and on most Zeeland beaches in a 2024 survey (NOS). Large litter is
  declining, but small plastics are not, and are "much harder to clean up" (De Noordzee,
  2026).
- **Big spills keep happening.** Galicia, Spain (December 2023): about 26 tonnes of PE
  pellets. Port of Tyne, UK (19 July 2026): about 25 tonnes, estimated at about a billion
  pellets, cleaned by volunteers with mesh bags and by council trommels and vacuums (trade
  and local news).
- **New EU law.** EU Regulation 2025/2365 on pellet losses has been in force since 16 December
  2025, with most obligations applying from 17 December 2027 (EU Council; Normachem).

### The physics
PE (0.88 to 0.97 g/cm³) and PP (0.90 to 0.92) float in fresh and sea water. PS (1.04 to
1.10), PVC and PET sink; seawater is about 1.025 and quartz sand 2.65 (Frontiers in Marine
Science; LibreTexts). Saturated salt brine (1.19 g/cm³) recovers about 94% of PE and PP and
would also float PS. Beach pellets in an Italian study were 80% PE and 20% PP. The share on
Dutch beaches that floats is **unverified**; plain water probably catches most, but would miss
a polystyrene spill like the MSC Zoe.

### What exists already (crowded)
- **Student teams have built this before.** Hoola One, a vacuum with seawater flotation, was
  built by 12 mechanical engineering students at Sherbrooke (prototype cost about $70,000).
  University of Southampton mechanical engineering students built a nurdle recovery unit that
  collected about 2 million pellets.
- **Commercial and charity kit exists.** The UK charity Nurdle uses hand trommels and a
  quad-towed vacuum developed with Kärcher. BeachTech Sweepy claims up to 95% removal on dry
  sand.
- **There is already a Dutch device.** Erik de Vries of De Bende van het Strand built a nurdle
  vacuum trailer, used at Scharendijke in March 2025.
- **The free method works.** Volunteers shake sand in a mesh bag in seawater, or skim a
  bucket.

### What would be new
A low-cost unit with no engine, for volunteers, in the gap between the free bucket and a
machine costing tens of thousands. It would handle wet sand and seaweed, add a brine stage
for polystyrene, and count pellets for citizen-science data. It is the weakest novelty of
the four.

### Cheapest test
Take a few 1 kg tideline samples at Scheveningen after a storm (ask Gemeente Den Haag and
Rijkswaterstaat whether a permit is needed first). Count pellets with a kitchen sieve and a
seawater bucket. Then spike clean sand with known PE, PP and PS pellets and compare recovery
and kg per minute for the bucket, a mesh bag and our rig.

**Kill result:** almost no pellets at Scheveningen, or our rig does not clearly beat the free
bucket or bag method on kg per minute.

### Stakeholders
Stichting De Noordzee (monitoring, Boskalis Beach Cleanup Tour), De Bende van het Strand,
Plastic Soup Foundation, TrashUre Hunt and Gemeente Den Haag, Rijkswaterstaat, WUR and NIOZ.

---

## What to do next

1. **This week:** make two hedgehog dummies and find someone with a robot mower (S1). Ask a
   local club whether we can brush boots after one training (X1). Both tests cost nothing.
2. **Before kick-off on 14 October:** send three messages to wheelchair tennis players or
   coaches (P3). Record every result in `../MEMORY.md` under Experiment log.
3. **By deliverable 1 on 21 October:** choose on the results.

## Sources

**S1 hedgehog guard**
- [Rasmussen et al. 2021, Animals: robot mower tests](https://pmc.ncbi.nlm.nih.gov/articles/PMC8143328/)
- [Rasmussen et al. 2024, Animals: standard test proposal](https://www.mdpi.com/2076-2615/14/1/122)
- [Animals 2024: hedgehog behaviour near mowers](https://www.mdpi.com/2076-2615/14/1/2)
- [Oxford: hedgehog safety test for robot mowers](https://www.ox.ac.uk/news/2024-01-16-researchers-develop-hedgehog-safety-test-robotic-lawnmowers)
- [Leibniz-IZW: hedgehogs injured by robot mowers](https://www.izw-berlin.de/en/press-release/new-research-into-hedgehogs-injured-by-robotic-lawn-mowers-discovers-a-significant-but-solvable-animal-welfare-and-conservation-problem.html)
- [Hedgehog Street: Near Threatened](https://www.hedgehogstreet.org/near-threatened/)
- [Egelbescherming Nederland](https://www.egelbescherming.nl/goed-nieuws-voor-de-egel-bescherming-komt-hoger-op-de-politieke-agenda/)
- [Nature Today: nachtelijk verbod op robotmaaiers?](https://www.naturetoday.com/nl/nl/nature-reports/message/?msg=35775)
- [Wallonie: rule of 9 April 2026](https://environnement.wallonie.be/actualite/robots-tondeuses-une-regle-wallonne-pour-mieux-proteger-les-herissons)
- [Stadt Koeln: night ban](https://www.stadt-koeln.de/politik-und-verwaltung/presse/mitteilungen/27055/index.html)
- [Erlangen: night ban](https://erlangen.de/aktuelles/naechtliches-verbot-fuer-maehroboter-7af869)
- [NOS: Nederland volgt nog niet](https://nos.nl/artikel/2609904-egels-in-wallonie-beschermd-tegen-robotmaaiers-nederland-volgt-nog-niet)
- [Husqvarna AI vision 2026](https://www.husqvarnagroup.com/en/press/husqvarna-group-reveals-ai-vision-technology-robotic-lawnmowers-2026-2397307)
- [Navimow hedgehog avoidance claim](https://roboticsandautomationnews.com/2026/05/12/navimow-responds-to-growing-hedgehogs-safety-concerns-with-ai-avoidance-technology/101404/)
- [Retrofit guard that broke docking](https://robomaeher.de/blog/igelschutz-apfelschutz-fuer-maehroboter-rasenroboter/)

**X1 infill catcher**
- [Kole et al. 2023: infill loss review](https://www.sciencedirect.com/science/article/pii/S0048969723048465)
- [Verschoor et al. 2021](https://link.springer.com/article/10.1186/s12302-021-00459-1)
- [ECHA: granules on pitches](https://echa.europa.eu/hot-topics/granules-mulches-on-pitches-playgrounds)
- [EU Regulation 2023/2055](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32023R2055)
- [KNVB dossier rubbergranulaat](https://www.knvb.nl/assist-bestuurders/accommodatie/velden/kunstgras/dossier-rubbergranulaat-kunstgras)
- [BSNC zorgplicht report 2024](https://www.bsnc.nl/wp-content/uploads/2025/01/2024-12-11-BSNC-Rapport-Zorgplicht_2024_def.pdf)
- [Raad van State ruling](https://www.raadvanstate.nl/@133436/gebruik-rubbergranulaat-kunstgrasvelden/)
- [Zembla: gemeenten moeten optreden](https://www.bnnvara.nl/zembla/artikelen/meer-gemeenten-moeten-optreden-tegen-milieuvervuilende-rubberkorrels-op-kunstgras)
- [Assen: measures on 13 pitches](https://www.assenstad.nl/assen/8698-assen-neemt-maatregelen-tegen-verspreiding-rubberkorrels-kunstgrasvelden)
- [Manshanden boot scrapers](https://www.manshanden.nl/matten-voetvegers.html)

**P3 wheelchair tennis**
- [ITF guide to wheelchair tennis](https://www.itftennis.com/en/news-and-media/articles/a-guide-to-wheelchair-tennis/)
- [KNLTB: Amanda Hopmans bondscoach](https://www.knltb.nl/nieuws/2024/12/amanda-hopmans-nieuwe-bondscoach-rolstoeltennis/)
- [Stichting BRNL blog on player numbers](https://jortverhage.com/bevorderen-rolstoeltennis/)
- [Georgia Tech wheelchair tennis robot](https://core-robotics-lab.github.io/Wheelchair-Tennis-Robot/assets/paper.pdf)
- [SIBOASI T2303M](https://www.siboasiballmachine.com/siboasi-tennis-ball-practicing-machine-t2303m-product/)
- [Ball machine prices overview](https://www.tennibot.com/blog/best-tennis-ball-machines/)
- [TU Delft measures wheelchair tennis movement](https://supportmagazine.nl/nieuws/tu-delft-meet-bewegingen-rolstoeltennissers-tijdens-wereldkampioenschap)
- [Uniek Sporten: rolstoeltennis](https://www.unieksporten.nl/sport/rolstoeltennis)

**S6 pellet separator**
- [De Noordzee: miljoenen plastic korrels](https://www.noordzee.nl/hoe-miljoenen-plastic-korrels-wijzen-op-een-groot-probleem/)
- [WUR/NIOZ on MSC Zoe pellets](https://edepot.wur.nl/543191)
- [NOS: Zeeuwse stranden meest vervuild](https://nos.nl/artikel/2514651-zeeuwse-stranden-meest-vervuild-van-nederland)
- [EU Council: pellet regulation](https://www.consilium.europa.eu/en/press/press-releases/2025/09/22/plastic-pellets-council-signs-off-regulation-to-reduce-pollution-from-microplastics/)
- [Polymer densities, Frontiers in Marine Science](https://www.frontiersin.org/journals/marine-science/articles/10.3389/fmars.2021.760649/full)
- [Hoola One](https://www.surfertoday.com/environment/hoola-one-the-beach-microplastic-vacuum-cleaner)
- [Southampton students' nurdle recovery unit](https://www.osrl.com/media/news/from-concept-to-cleanup-university-of-southampton-students-develop-advanced-nurdle-recovery-equipment/)
- [Dutch nurdle vacuum, Hart van Nederland](https://www.hartvannederland.nl/milieu-gezondheid/natuur/artikelen/speciale-stofzuiger-stranden-redden-plastic-vervuiling)
- [Port of Tyne spill, July 2026](https://envirotecmagazine.com/2026/07/24/major-nurdle-clean-up-launched-after-tyne-vessel-collision/)
