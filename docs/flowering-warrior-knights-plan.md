# Product Development Plan: The Flowering Warrior Knights

*A phased plan to turn the kids ITF Taekwon-Do anime into a show that modern 6-10 year olds choose to watch, and that grows discipline and the ability to defend themselves physically, mentally and emotionally.*

- Owner and final approver: Randy
- Status: draft v2, 2026-11-18. Reworked to Randy's new big idea (five boys, the ageless Grandmaster storyteller, and a belt-by-belt Season 1).
- Builds on: the production skills and `episode-producer` agent (`.claude/`, PR #1), the ITF lore library (`references/itf/`, PR #2), and `brand/brand.md`
- Timeline convention: "Week 1" is the week Randy approves this plan. Dates move with his decisions, not the other way round.

---

## 0. Decisions

### Decided by Randy (2026-11-18)

- **The frame:** five boys finish every training session by sitting around their ageless Grandmaster, who tells them the myths, legends and lore of the patterns, belts and Taekwon-Do. As each story begins, the boys imagine themselves as characters in it. This replaces the earlier "magic doors" idea; the imagined legend is now the adventure.
- **The cast:** all boys, each with an incredible, cool creative skill or hobby. Season 1 ages: 8, 6, 6, 5, and 3½ (the 8-year-old's little brother).
- **The club:** the boys eventually form **The Flowering Warrior Knights** in their real lives, to bring peace and justice to the world around them. Their good deeds ripple outward and slowly change the future for the better, until they "build a more peaceful world" (the last line of the Student Oath).
- **Season 1 structure:** belt by belt, ending at red belt. White belt has 4 episodes (the belt's meaning, Saju Jirugi, Saju Makgi, Chon-Ji); yellow, green, blue and red have 3 each (the belt's meaning, then its two patterns). That is **16 episodes**.

### Still open

| # | Decision | Options | Recommendation |
|---|----------|---------|----------------|
| D2 | Show title | Keep *Tiger Belt: The 24 Doors* (doors no longer feature); or *The Flowering Warrior Knights*; or a short form such as *Warrior Knights* | *The Flowering Warrior Knights* now matches the premise. Run the trademark and handle checks (Phase 0) before locking it. |
| D3 | Budgets | Per main episode, per short, per month (still blank in `brand/brand.md`) | Pilot-only budget first; season budget once the pilot's real cost is known. 16 episodes is a bigger season, so this matters more now. |
| D4 | Instructor reviewer | A named ITF instructor who signs off technique and safety lessons | Required before any safety lesson is published. |
| D5 | Korean cultural advisor | A Korean or Korean-diaspora advisor who reviews history, language, the Grandmaster's portrayal, and visuals | Strongly recommended, more so now that a Korean Grandmaster is the show's central adult. |
| D6 | Voices | AI voices, human voice actors, or a mix | Human or licensed voices for the Grandmaster and the five boys; AI for temp tracks. Ideally real child voice actors through an agency (with parental consent and proper contracts), never any real child's voice cloned or used without that. |
| D7 | Release cadence | Starting target: 1 main episode every 2 weeks, 3 shorts a week | Bank 4 finished episodes before launch. At that pace, 16 episodes take about 32 weeks to release. |
| D8 | The Grandmaster's secret | How he has "lived for an eternity" | Recommended: he was once a young Hwarang of Silla who made a promise to keep teaching until the world is at peace. Hinted at all season and revealed in the Hwa-Rang episode. He is never a real historical person. |
| D9 | When the club forms | Early (white belt) or late | Recommended: the Grandmaster plants the idea in episode 1, the boys play at being knights all season, and the club is founded for real in the Hwa-Rang episode (ep 15). The finale is their first mission. |
| D10 | A villain or not | No villain (real-life problems only), or a gentle shadow inside the stories | Recommended: keep a gentle shadow, "the Gloom", that appears only in the imagined stories and whispers "give up", "just hit them". Boys 6-10 love a foe to beat, and the tenets beat it. |

---

## 1. Vision

### 1.1 The problem

Taekwon-Do's stories and lessons are wise, deep and emotionally mature. But to a modern kid, the way they are usually presented looks black-and-white and strict: lines, counting, silence, rules. Kids' media competes with fast, funny, colourful, music-driven shows and games. The lessons are not the problem. The packaging is.

### 1.2 The answer: the Flowering Warrior Knights

The **Hwarang** ("flower youth", "flowering knights") of the Silla kingdom were young people who trained in martial arts **and** in poetry, music, dance and good manners, and who travelled mountains and rivers to grow strong and wise (`references/itf/patterns.md`, Hwa-Rang). General Choi drew on their ideals, and the pattern **Hwa-Rang** is named after them. They make "strong" and "creative" the same thing.

**The premise in one line:** after every class, five boys sit at the feet of a Grandmaster who has lived forever, and his stories turn them into the heroes of Korea's legends, until they decide to become flowering warrior knights in real life and start, one small good deed at a time, to build a more peaceful world.

### 1.3 Why this format works

- **The circle is a ritual.** Every episode opens the same way: the bow, sweaty and laughing, sitting down, "Grandmaster, tell us a story!" Rituals make a show feel like the viewer's own.
- **Imagination is the superpower kids already have.** Watching the boys imagine themselves as a bear, a king, an admiral or a monk is exactly what our viewers do in play. It invites them to do the same.
- **Each boy's art shapes his imagination.** The comic-artist boy imagines the legend as a comic; the dancer moves through it; the drummer gives it a beat. That gives every legend a fresh visual style and gives each boy a reason to shine.
- **Real life is where the win counts.** The story ends, the boys go home, and they use what they learned. The good deed sends out a ripple.
- **Grounded in true stories.** "This is a real legend" is something most fantasy shows cannot say.

### 1.4 What we promise

| To kids | To parents |
|---------|-----------|
| A crew of funny, talented boys, a mysterious Grandmaster, and epic legends where you get to be the hero. Moves and art to try at home. | A show that builds discipline, confidence, emotional skills and real safety skills, with nothing you would not want your child to copy. Honest about AI use, Made for Kids, no data collected from children, reviewed by a real instructor. |

### 1.5 Design principles (hypotheses to test in Phase 2)

1. **A team with distinct powers.** Kids love a crew where each member has a clear personality and skill.
2. **Levelling up you can see:** belts, the club's Ripple Map, skills earned.
3. **Music and art as power,** grounded in the Hwarang, never copied from any existing show.
4. **A laugh every 30 seconds** (`storytelling`): the 3½-year-old and the 5-year-old carry a lot of the comedy.
5. **A real-world payoff every episode:** a move, a breath, a safety skill, a kind act.

---

## 2. The framework: Three Shields and the Flower

Randy's goal is a child who can defend himself **physically, mentally and emotionally**. We make that explicit and collectable.

| Shield | What it protects | Built from | Lessons already in the library |
|--------|------------------|-----------|--------------------------------|
| **Body Shield** | Physical safety | Stances, distance, voice, escapes, falling, getting help | SD-01 to SD-05, SD-13 to SD-20 |
| **Mind Shield** | Clear thinking under pressure | Spotting tricks, online safety, choosing your thoughts, awareness | SD-11, SD-21, SD-22, SD-23; Won-Hyo's "your thoughts change your feelings" |
| **Heart Shield** | Emotional strength | Naming feelings, calming down, bouncing back, empathy, standing up for others | SD-06, SD-08, SD-09, SD-10, SD-24, SD-25 |
| **The Flower** | The creative, compassionate, collaborative mind | Each boy's art, teamwork, kindness | Hwa-Rang's moral: "strength plus kindness and creativity" |

Episode formula (extends the lesson rule in `storytelling`): **one tenet + one belt, pattern or fundamental + one Shield skill + one art moment + one real-world ripple.**

---

## 3. Creative concept: the world and characters (series bible v2)

All lore comes from `references/itf/`. Anything not in the library is marked `[VERIFY]` and kept off screen until checked.

### 3.1 The world

- **The Dojang (real world):** a warm neighbourhood Taekwon-Do school. Wooden floor, the tenets on the wall, and a small back garden with a stone basin of water where the Grandmaster tells his stories.
- **The Story Circle:** after every class the boys sit in a circle around the Grandmaster. He strikes a small brass bowl, and the story begins.
- **The Imagined Legend:** as he tells it, the dojang melts into the legend and each boy becomes a character in it. The imagined world is drawn in a painterly ink-and-colour style, shifting with whose imagination leads (comic panels, dance, rhythm), so viewers always know what is real and what is imagined.
- **The Ripple:** every episode ends with the boys doing something good in real life. In the garden basin a drop falls and a ripple spreads. Over the season the Grandmaster's old scroll, the **Ripple Map**, fills with light, showing small changes spreading into the future. Only the Grandmaster (and the viewer) sees the full map until the finale.

### 3.2 Rules of the story (v2)

1. The legend's facts come from `references/itf/`. The boys' imagination adds the fun (who plays whom, jokes, their art), never changes the real story's outcome or meaning.
2. Martial arts in the stories show discipline and protection, never revenge, and never settle a playground argument.
3. The Gloom (if kept, D10) appears only in the imagined stories and is beaten by tenets and teamwork, never by hurting anyone.
4. The win that counts is the real-life choice after the story.
5. Each boy's art builds, calms, heals or connects. Never a weapon.

### 3.3 Cast v2 (names are placeholders)

All five boys are fictional. Their names, looks, voices and details must not be based on any real child, including Randy's own family (CLAUDE.md rule 4).

| Character | Age (S1) | Creative skill (his Flower) | How he imagines the legends | Shield strength | Flaw and growth |
|-----------|----------|-----------------------------|----------------------------|-----------------|-----------------|
| **Kai**, the leader | 8 | Drums and beatboxing; turns every kihap into a beat | Wants to be the hero of every story; learns to give others the lead role | Body | Impatient, wants to be strong fast; learns patience and self-control |
| **Bo**, Kai's little brother | 3½ | Finger-painting, clay monsters, singing very loudly | Always picks the animal (the tiger, the turtle ship's dragon head) | Heart | Copies Kai in everything; learns that being small isn't being weak (General Choi's own lesson) |
| **Leo** | 6 | Drawing comics; the legend turns into comic panels when he leads | Plays the sidekick and the narrator | Mind | Afraid to try new things; learns perseverance |
| **Jun** | 6 | Breakdancing and rhyming; spins and freezes become moves | Plays the warriors and the dancers | Body | A show-off who doesn't listen; learns courtesy |
| **Theo** | 5 | Building and inventing: cardboard, tape, gadgets; designs the turtle ship | Plays the planners, inventors and kings | Mind | Gives up when things break; learns indomitable spirit |
| **The Grandmaster** | Unknown | Calligraphy, the bamboo flute | Narrates; sometimes appears in the legend as a mysterious old hermit | All | His secret (D8) |
| **The boys' families** | Adults | Warm, busy, funny | Never in the legend | | Parents are kind and wise; no jokes at their expense |

**The Grandmaster.** A legendary South Korean Grandmaster (in ITF terms a 9th-dan *Saseong*, `terminology.md`). Kind, funny, a little mischievous, endlessly patient. He says little in class and everything in stories. He has secretly lived for an eternity, and small clues show it: he hums a song nobody knows, he remembers things "from a long time ago" a little too clearly, the scroll in the back room is very old. He is **never** presented as General Choi or any real person, and the show never implies a real person was immortal. The cultural advisor reviews how he speaks, dresses and teaches so he is a real character, not a stereotype of the "wise old Asian master".

### 3.4 The Five Flower Promises

The club's charter, from the Hwarang's five rules given by the monk Won-Gwang, in the library's kid versions (`patterns.md`, Hwa-Rang), recited with the Student Oath:

1. Love your home and the people in it.
2. Respect your parents.
3. Be a true friend.
4. Never give up.
5. Be gentle with every living thing; only use force when you truly must.

### 3.5 The Silla thread

| Pattern | Belt | Link (from `patterns.md`) | Role |
|---------|------|---------------------------|------|
| Won-Hyo | Green (6th kup) | Silla monk who shared his teaching with everyday people, singing and dancing in the streets | First Silla story; the Grandmaster seems to know the place |
| Hwa-Rang | Red (2nd kup) | The Hwarang youth group | The club is founded; the Grandmaster's secret revealed |
| Yoo-Sin | 3rd Dan | Kim Yoo-Sin trained as a teenage Hwarang | Later seasons |
| Moon-Moo | 4th Dan | The flute that calms ten thousand waves | Later seasons; the Grandmaster's flute |
| Tong-Il | 6th Dan | "Becoming one again" | Series finale: the Ripple Map complete, a more peaceful world |

Unification is told as three families of one people becoming one family, never as conquest; heroes of the other kingdoms (Kwang-Gae of Koguryo, Ge-Baek of Baekje) are heroes too. On screen say "Korea's Three Kingdoms" (they covered the whole peninsula, not only present-day South Korea).

To verify before they appear on screen `[VERIFY]`: the Hwarang's founding date (ITF says "early 7th century"; many histories say the 6th century under King Jinheung); any claim about the Hwarang's role in unification; anything from the disputed *Hwarang Segi*. Always avoid: Gwan-Chang's death in battle, battle deaths, Kim Yoo-Sin beheading his horse.

### 3.6 Tone

Exciting first, wise second, funny always. Real but kid-sized problems (a lost game, a bully, a broken toy, a fight between brothers). Adults are wise and kind. The legends are epic but never gory.

### 3.7 Every episode (recurring segments v2)

1. **Cold open** (5-10 s): the end of class, a laugh or a mishap.
2. **The real-world problem:** one boy is stuck on something.
3. **The Story Circle:** "Grandmaster, tell us a story!" The bowl rings.
4. **The Imagined Legend:** the boys become its characters (about half the episode).
5. **The choice inside the story:** a tenet wins (and beats the Gloom, if kept).
6. **Back home:** the boy uses the lesson; the ripple spreads.
7. **Grandmaster's Fact** (5 s): one true fact or number about the belt or pattern.
8. **The Safety Lesson:** the Grandmaster (or an instructor at the dojang) teaches the Shield skill and the boys practise. See `self-defense-lessons`.
9. **Sign-off:** the Five Flower Promises or the Student Oath, the bow, and "Build a more peaceful world. See you after class!"

### 3.8 What the younger cast ages affect (flag)

The cast (3½ to 8) is younger than the audience (6-10). That works, with care:

- **Older viewers.** Kids usually watch characters their age or a bit older, so a cast this young can read as "a little-kid show" to 9-10 year olds. Mitigations: Kai (8) leads; the imagined legends cast the boys as kings, admirals and warriors, so the action looks grown-up; humour and pace are pitched at 8-10, not preschool; the boys age a year each season.
- **Bo (3½).** Great comic heart, but toddler humour skews young, so use it in small doses. He mostly joins the stories and the fun rather than doing techniques. Real 3-4 year olds train in "little tigers" style classes, so show him in a supervised, age-right way.
- **Safety copying.** Younger kids at home will copy Bo and Theo. Every move they do on screen must be safe for a 4-6 year old to copy, with a grown-up.
- **Belt pace.** Real students take years to reach red belt; the boys reach it in one season. Treat it as story time (montage and "months later" cards), and the Grandmaster can say "in a real dojang this takes a long time".
- **Voices.** Five child voices plus an older man is a big cast to voice. Budget for it (D6).
- **Real children.** Keep all five boys fully fictional (the 8-year-old with a 3½-year-old brother must not mirror any real family's names, looks or details).

---

## 4. Season architecture

### 4.1 Season map (replaces the two earlier maps in `itf-lore` and `references/itf/README.md`)

| Season | Belt journey | Episodes | Big idea | Finale |
|--------|--------------|----------|----------|--------|
| **S1: The Flowering Warrior Knights** | White to red (ends with Choong-Moo, red/black stripe) | 16 | From seeds to knights; the club is born | The club's first mission; the Ripple Map lights up |
| **S2** (boys a year older) | Black belt | About 10-12 | Black belt is a new beginning; the 1st Dan patterns (Kwang-Gae, Po-Eun, Ge-Baek) | Black belt grading |
| **S3 onward** | Dan patterns | | Black belt legends; the Silla thread (Yoo-Sin, Moon-Moo) | Tong-Il series finale: a more peaceful world |

### 4.2 Season 1 episode slate (draft, for `episodes/backlog.md`)

Tenets and Safety Lessons follow the library's pairings (`patterns.json`, `self-defense-lessons.md`) wherever they fit. Imagined roles are first ideas for the writers.

**White belt (4 episodes)**

| Ep | Working title | Subject | Tenet | Shield skill | Imagined roles and ripple |
|----|---------------|---------|-------|--------------|----------------------------|
| 1 | The Seed (pilot) | White belt meaning: innocence, a seed resting in the ground (`belts.md`) | Courtesy | SD-01 Be the Boss of Your Space (Body) | The boys imagine being seeds in snow; Bo refuses to stay a seed. The Grandmaster first mentions "flowering warrior knights". Ripple: Kai helps a new kid tie his belt. |
| 2 | Four Directions | Saju Jirugi (four-direction punch) `[VERIFY: name, meaning and any story; not yet in references]` | Self-Control | SD-21 Spot the Exits (Mind): look all four ways | A story of guarding the four directions (for example Korea's four guardian animals `[VERIFY]`). Ripple: Theo spots a safe exit at the park. |
| 3 | The Four Shields | Saju Makgi (four-direction block) `[VERIFY]` | Perseverance | SD-04 The Stop Hand (Body) | Blocking means protecting, not fighting. Ripple: Leo uses the Stop Hand and his words with a pushy kid. |
| 4 | Heaven and Earth | Chon-Ji; white belt grading | Courtesy | SD-03 The Power Voice (Body) | The boys imagine the first morning of the world: Jun dances the sky, Theo builds the earth. Ripple: the first kihap beat; yellow belts. |

**Yellow belt (3 episodes)**

| Ep | Working title | Subject | Tenet | Shield skill | Imagined roles and ripple |
|----|---------------|---------|-------|--------------|----------------------------|
| 5 | Roots | Yellow belt meaning: the earth where roots grow | Integrity | SD-07 If You Get Lost (Body/Mind) | Roots are the people who hold you up. Ripple: the boys thank the people who help them. |
| 6 | The Bear Who Waited | Dan-Gun | Perseverance | SD-02 The Confident Stance (Body) | Kai is the patient bear, Bo is the tiger who gives up after a day. Ripple: Kai sticks with a hard drum beat. |
| 7 | The Boy Who Cleaned the Street | Do-San | Integrity | SD-22 The Buddy System (Mind) | Leo's comic of the street getting cleaner. Ripple: the boys clean up the dojang's street. |

**Green belt (3 episodes)**

| Ep | Working title | Subject | Tenet | Shield skill | Imagined roles and ripple |
|----|---------------|---------|-------|--------------|----------------------------|
| 8 | Growing | Green belt meaning: the plant's growth | Perseverance | SD-24 Calm Body, Clear Mind (Heart) | A sprout pushing through rock. Ripple: Theo tries again when his invention breaks. |
| 9 | The Sweetest Water | Won-Hyo; first Silla story | Self-Control | SD-05 No, Go, Yell, Tell (Body) | Jun is Won-Hyo dancing in the streets. The Grandmaster seems to remember Silla. Ripple: Leo changes "I can't" to "I can't yet". |
| 10 | Prepare Ahead | Yul-Gok | Perseverance | SD-06 My Trusted Adults Team (Heart) | Theo is the scholar who plans ahead. Ripple: the boys make a plan for a scary first. |

**Blue belt (3 episodes)**

| Ep | Working title | Subject | Tenet | Shield skill | Imagined roles and ripple |
|----|---------------|---------|-------|--------------|----------------------------|
| 11 | Reaching for the Sky | Blue belt meaning: heaven, the tree grows tall | Indomitable Spirit | SD-11 Online Safety Shield (Mind) | The tall tree in a big blue sky. Ripple: a tricky message online, handled with a grown-up. |
| 12 | The Promise | Joong-Gun (high sensitivity: values only, never the assassination; `patterns.md`) | Indomitable Spirit | SD-14 Wrist Grab Escape (Body, light contact with a grown-up) | Keeping promises and dreaming of peace. Ripple: Kai keeps a promise to Bo. Needs extra script review. |
| 13 | The Scholar Who Listened | Toi-Gye | Courtesy | SD-08 Walk Away Like a Black Belt (Heart) | Great people listen and admit mistakes. Ripple: Jun says sorry. |

**Red belt (3 episodes)**

| Ep | Working title | Subject | Tenet | Shield skill | Imagined roles and ripple |
|----|---------------|---------|-------|--------------|----------------------------|
| 14 | Red Means Careful | Red belt meaning: danger, so stay in control | Self-Control | SD-09 Words That Shield (Heart) | A glowing ember that must be kept safe. Ripple: Kai doesn't hit back. |
| 15 | The Flowering Knights | Hwa-Rang; the club is founded (D9) | All five | SD-10 Stand Up for a Friend (Heart) | All five boys become young Hwarang. The Grandmaster's secret (D8). Ripple: The Flowering Warrior Knights are born and recite the Five Flower Promises. |
| 16 | Thirteen Little Ships (finale) | Choong-Moo | Indomitable Spirit | SD-25 Making Peace (Heart); SD-13 Falling Safely as a short | Theo builds the turtle ship, Kai is the admiral. The club's first mission brings two groups of kids together. The Ripple Map lights up. |

Plus about 45-50 shorts for S1 (about three per episode): "Legend in 45", Safety Lesson shorts, Grandmaster's Facts, Pattern Challenges, and **Art challenges** led by each boy ("draw the bear who waits with Leo", "make a kihap beat with Kai").

## 5. The phased plan

Each phase lists its goal, steps and tasks, the skill or file that owns the work, the deliverable, and the gate that must pass to move on. Phases 9 (safety) and 10 (measurement) run continuously alongside the others.

### Phase 0: Foundation and decisions (Weeks 1-2)

**Goal:** settle the decisions and set-up that everything else depends on.

1. Decisions
   - [ ] Randy decides D2-D10 (Section 0).
   - [ ] Record decisions in `brand/brand.md` and project memory.
2. People
   - [ ] Name the instructor reviewer (D4) and agree scope: technique, safety lessons, ITF accuracy.
   - [ ] Find a Korean cultural advisor (D5): local Korean community centre, Korean cultural institute, or a Korean ITF instructor.
   - [ ] Decide what Randy's son's role is: test viewer only, with feedback passed on by Randy in words. No images, voice, name or details ever enter the repo or any tool (CLAUDE.md rule 4).
3. Name and rights (`rights-and-licensing`)
   - [ ] Shortlist 3 titles (D2).
   - [ ] Trademark search (USPTO, and KIPO for Korea if launching there) and YouTube/TikTok/Instagram handle search for each.
   - [ ] Check for confusion with existing Hwarang titles (for example the 2016 Korean TV drama about the Hwarang) and with recent hit Korean-themed kids' properties. Our names, designs and music stay clearly original.
   - [ ] Confirm we use no ITF organisation logo or crest; design an original emblem.
4. Business set-up (`business-strategy`, `accounting`)
   - [ ] Set pilot budget (D3) and fill `brand/brand.md`.
   - [ ] Create `finance/ledger.csv` and log every cost from now on.
   - [ ] Decide on a business entity and separate bank account before contracts or revenue (Randy decides, with professional advice).
5. Repo housekeeping
   - [ ] Merge PR #1 (skills) and PR #2 (lore) to `main` so every session reads one source of truth.

**Deliverables:** decisions recorded, reviewer and advisor named, title shortlist with check results, budget set.
**Gate:** Randy approves the title shortlist and budget.

### Phase 1: World and story bible v2 (Weeks 2-5)

**Goal:** the Hwarang concept becomes canon the agent can write from.

1. Lore
   - [ ] Write `references/itf/hwarang.md`: Hwarang history and legends for kids, with sources, `[VERIFY]` flags, and an "avoid" list. Have the cultural advisor review it.
   - [ ] Add the Five Flower Promises and the Silla thread to the references.
2. Bible (`series-bible`)
   - [ ] Update the skill with: the Story Circle frame, the five boys and the Grandmaster, imagined roles, the Ripple and Ripple Map, The Flowering Warrior Knights, Rules of the story v2, recurring segments v2.
   - [ ] Write the Grandmaster's secret and the clue trail (D8), and get the cultural advisor's notes on his portrayal.
   - [ ] Add Saju Jirugi and Saju Makgi to `references/itf/terminology.md` with sources, plus any story for the four directions, before episodes 2-3 are written.
   - [ ] Write character one-pagers: voice, catchphrase, what they want, what they fear, how their art shapes their imagination.
   - [ ] If the Gloom is kept (D10), define its limits: spooky shadow only, inside stories only, never horror (`child-safety-compliance`).
3. Story system (`storytelling`, `itf-lore`, `self-defense-lessons`)
   - [ ] Update the lesson rule to "tenet + pattern + Shield + art".
   - [ ] Tag every SD lesson with its Shield (Body, Mind, Heart).
   - [ ] Reconcile the season map (Section 4.1) in `itf-lore`.
   - [ ] Seed `episodes/backlog.md` with the S1 slate (Section 4.2) and `episodes/continuity.md`.
4. Season arc
   - [ ] Write the S1 arc document: the Grandmaster's secret, the club's path to founding in ep 15, the Ripple Map, each boy's growth line, where each new skill is planted and paid off.
5. Brand (`brand-management`)
   - [ ] Update the promise and values: "strong, kind, creative".
   - [ ] Add petal, ink and bamboo-flute motifs to the colour and motif system, alongside the belt colours.

**Deliverables:** bible v2, `hwarang.md`, tagged lesson library, S1 arc and backlog.
**Gate:** Randy approves bible v2; the cultural advisor signs off `hwarang.md`.

### Phase 2: Audience research and validation (Weeks 3-7, in parallel with Phase 1)

**Goal:** check that the concept appeals to kids and convinces parents, without collecting any child's data.

1. Desk research (`analytics-and-growth`)
   - [ ] Comparables study: the top 15-20 shows, games and YouTube channels boys 6-10 watch now. For each: format, length, humour, music use, levelling systems, what parents say. Output `analytics/comparables.md`.
   - [ ] Martial-arts kids' content on YouTube and TikTok: what works, what is missing (most is live-action instruction, very little is story).
   - [ ] Search demand: what parents search ("taekwondo for kids at home", "teach kids self-defense", "how to help my child with anger").
2. Parent and instructor research (adults only)
   - [ ] Interview 5-10 ITF instructors: what keeps kids training, why they quit, which lessons they wish kids understood.
   - [ ] Parent survey (adults only, no child data) via partner schools and parent groups: what they want their kids to learn, what they block, what they pay for.
   - [ ] Concept test with parents: 3 title options, 3 key-art styles, 2 loglines, the Three Shields idea.
3. Kid appeal (through adults, observation only)
   - [ ] Randy shows his son concept art, a theme-song demo and an animatic, and reports reactions in words (what he laughed at, asked about, copied, wanted again). Nothing recorded or uploaded.
   - [ ] Partner schools may run an in-class viewing of the animatic under their own consent rules and send back aggregate notes ("most kids copied the kihap beat"). We receive no names, images or recordings.
4. Hypotheses and kill criteria (write them before testing)
   - H1: kids find the boys' arts and imagined legends exciting, not "soft". Signal: they ask to see a legend again or copy a boy's art or move.
   - H2: parents value the Three Shields framing. Signal: it is the top reason they would show the show.
   - H3: the Grandmaster and the Story Circle are a favourite. Signal: kids ask "what story is next?"
   - H4: 9-10 year olds still feel the show is for them despite the young cast (Section 3.8). Signal: parents of older kids report they watch willingly.
   - If H1 fails, lean the legends towards action and kihap; keep arts as the flavour, not the spectacle. If H4 fails, lean on Kai and the epic legend roles, and age the cast faster.

**Deliverables:** `analytics/comparables.md`, interview and survey notes, concept-test results, a one-page "what we learned" memo.
**Gate:** at least 2 of 3 hypotheses supported, or a revised concept that Randy approves.

### Phase 3: Look and sound development (Weeks 5-10)

**Goal:** a visual and audio identity that looks premium and stays consistent through AI generation.

1. Art direction (`art-direction`)
   - [ ] Style frames for: the dojang and garden, the Story Circle, the moment the dojang melts into a legend, the ink-and-colour legend style (one variant per boy's art), a Silla mountain scene, the Ripple Map.
   - [ ] Character model sheets for every lead (turnarounds, expressions, each boy at every belt colour, the Grandmaster in dobok and in his hermit form, reviewed by the cultural advisor).
   - [ ] Shield and Flower icon set; the Shield Board.
   - [ ] Colour script per belt colour; Silla palette (petals, ink, bamboo).
2. Generation tests (`video-generation`)
   - [ ] Test 2-3 image and video tools on the same 10-shot sequence. Score consistency, motion quality, lip-sync, cost per finished second, and commercial-use terms.
   - [ ] Build the reusable asset library: backgrounds, the Story Circle opening, the melt into the legend, the Ripple, the bow, the Safety Lesson set (reuse cuts cost and keeps the look consistent).
3. Sound (`voice-and-music`)
   - [ ] Theme song: catchy, chantable, built around the kihap and a bamboo-flute hook. Licensed or composed for hire with full rights.
   - [ ] Musical signatures: each kid's art has a sound (Kai's beat, Bo's off-key singing, Leo's pencil scratch, Jun's scratch-and-spin, Theo's tape-and-clank, the Grandmaster's flute and brass bowl).
   - [ ] Voice casting for the Grandmaster and the five boys (D6), with child actors only through proper agencies and parental consent. Korean pronunciation guide from `terminology.md`, checked by the advisor.
   - [ ] Sound library: the bowl ring, the melt, the ripple, the Gloom whisper (soft, never a jump-scare), kihap.
4. Costing
   - [ ] Measure the real cost per finished minute and per short, and log it (`accounting`).

**Deliverables:** art bible, model sheets, tool decision, theme song, cast, cost per minute.
**Gate:** Randy approves the look and the theme; cost per minute fits the budget.

### Phase 4: Pilot (Weeks 9-14)

**Goal:** one finished main episode and 3 shorts that prove the show.

1. Run EP001 "The Seed" through all 12 stages of `production-pipeline`: brief, outline, script, storyboard, generate, audio, edit, package, QA, approval.
2. Script gates
   - [ ] Script read for "a laugh every 30 seconds", a boy (not an adult) makes the winning choice, one tenet shown not preached.
   - [ ] Instructor sign-off on SD-01 and any technique on screen.
   - [ ] Cultural advisor review of Hwarang and Korean content.
3. Animatic test (before full generation, to save money)
   - [ ] Randy's son watches the animatic; Randy reports reactions.
   - [ ] One or two partner schools run a viewing and send aggregate notes.
   - [ ] Fix what lost attention (`analytics-and-growth`: anywhere a scene runs over about 40 seconds without change).
4. Final production and QA (`content-qa`, `child-safety-compliance`)
   - [ ] Full QA report: lore, technique, safety red lines, photosensitivity, captions, loudness.
   - [ ] Cut 3 shorts: a Legend in 45, the SD-01 Safety Lesson short, one Flower challenge.
5. Pilot review
   - [ ] Real cost of the pilot vs budget.
   - [ ] Lessons for the pipeline: what to template, what to reuse, what to batch.

**Deliverables:** EP001 master (16:9) and vertical cuts (9:16), 3 shorts, QA report, cost report.
**Gate:** Randy signs `approval.md`. The test viewer asks for more. Cost per episode is known. (Not published yet: see Phase 6.)

### Phase 5: Pipeline scale-up and Season 1 production (Weeks 14-46)

**Goal:** produce Season 1 at a steady, affordable cadence without losing quality.

1. Batching (`production-pipeline` rule 6)
   - [ ] Write scripts in batches of 3-4; generate visuals for a batch together for consistency.
   - [ ] Lock reusable sequences (Story Circle, melt, Ripple, Safety Lesson set, sign-off).
2. Automation (`ai-automation`)
   - [ ] Schedule the `episode-producer` agent to advance episodes and stop at human gates.
   - [ ] Cost guards: stop any job that would exceed the per-episode budget.
   - [ ] Run log (`logs/runs.md`) and weekly status summary for Randy.
3. Human creative input on every episode
   - [ ] Randy or a named writer approves each script and adds at least one original touch (a joke, a line, a beat). This protects quality and YouTube monetisation, which penalises mass-produced, repetitive content (`child-safety-compliance` section 2).
4. Production targets
   - [ ] Bank EP001-EP004 before launch.
   - [ ] Then 1 main episode every 2 weeks, 3 shorts a week (adjust after launch data).
5. Quality loop
   - [ ] After each episode: QA report, cost logged, continuity updated, one improvement to a skill or template.

**Deliverables:** S1 episodes and shorts on schedule, an automated but gated pipeline.
**Gate per episode:** QA pass plus Randy's written approval.

### Phase 6: Platform launch (Weeks 16-20)

**Goal:** a clean, compliant launch on YouTube, TikTok and Instagram.

1. Accounts (`social-media-management`, `child-safety-compliance`). Randy creates or approves every account; no account change without approval.
   - [ ] YouTube channel set to **Made for Kids**; every upload MFK.
   - [ ] TikTok and Instagram owned by Randy (adult), aimed at **parents**; strangers' DMs, duets and stitches limited.
   - [ ] Matching handles; channel art and bios on brand.
   - [ ] AI disclosure line in every description: "Animated with the help of AI tools; written and reviewed by people."
2. Launch package (`thumbnails-and-seo`)
   - [ ] Trailer (60-90 s) and a launch short.
   - [ ] Playlists: Season 1 episodes, Safety Lessons, Legends in 45, Flower challenges.
   - [ ] Honest titles and thumbnails that kids want and parents trust.
3. Launch calendar
   - [ ] Week 1: trailer, pilot, 3 shorts. Weeks 2-4: EP002-EP004 with shorts, then the regular cadence.
   - [ ] Parent-facing posts: "a 45-second safety lesson to practise with your kids"; "what the yellow belt really means".
4. Partner launch
   - [ ] 5-10 ITF schools share the pilot with their families (they post; we never ask kids to follow).
5. Approval
   - [ ] Every post prepared as private or draft; Randy flips it public (CLAUDE.md rule 1).

**Deliverables:** live channels, pilot and first episodes published with approval.
**Gate:** Randy's written approval for each public post.

### Phase 7: Growth (from launch, ongoing)

**Goal:** more returning viewers each month, driven by quality and by schools and parents, not by gaming the algorithm.

1. Weekly review (`analytics-and-growth`): retention curves, returning viewers, which segments lose kids, which shorts drive episode views.
2. Experiments (one at a time, written down first):
   - Cold-open styles; episode length (4 vs 6 minutes); which boy leads the imagined legend; legend length vs real-world length.
   - Shorts mix: Safety Lesson vs Legend vs Flower challenge.
3. Community without collecting kids' data:
   - "Train along" episodes and pattern challenges kids do with a grown-up at home.
   - Parent-facing challenges on TikTok and Instagram ("practise the Stop Hand with your child tonight").
4. School network (strongest channel):
   - The **Flowering Warrior Knights Club kit** for dojangs (see Phase 8): schools use episodes in class, and families find the channel through their school.
   - Track outreach in `business/partners.md`; the agent drafts emails, Randy sends.
5. Cultural partners: Korean cultural centres, Korean-language schools, Children's Day (Korea, 5 May) and Gaecheonjeol (3 October) themed releases.
6. Feed learnings back: each month update the backlog and one skill with what worked.

### Phase 8: Business and products (Month 4 to Month 18)

**Goal:** revenue that covers production, from sources that fit a Made for Kids channel.

Made for Kids means no personalised ads, comments, merch shelf, notification bell, cards or end screens (`child-safety-compliance`). So ads are a base, not the plan (`business-strategy`).

| Stream | What | When | Notes |
|--------|------|------|-------|
| **Flowering Warrior Knights Club kit for dojangs** | A monthly class programme: episode, a Story Circle guide for instructors, printable pattern sheet, Safety Lesson guide, an art challenge, Shield certificates, a class Ripple Map | Pilot onward; paid from S1 | Strongest fit. Schools pay a licence or sponsor an episode (credit aimed at parents). |
| YouTube ads (YPP) | MFK ads | After YPP eligibility | Low revenue per view; keep authenticity high to stay eligible. |
| Printables for parents | Shield Board chart, belt-progress chart, colouring pages, the Five Flower Promises poster | From launch | Sold on a parent-facing site, never linked to kids from MFK videos. |
| Picture books | One per season ("The Bear Who Waited", "The Flowering Warrior Knights") | After S1 | Strong gift market; reuses art. |
| Merch | Character plush (Bo and his clay monster), Shield patches for belts, Warrior Knights wristbands in belt colours, bamboo practice flute | After S1 traction | Sold via the parent site and partner schools. Product safety and toy-testing rules apply (Randy gets advice first). |
| Licensing | Kids' streaming platforms, schools, Taekwon-Do organisations | Once S1 exists | Do not take sides between ITF groups (`general-choi.md`). |
| Sponsors | Family brands, disclosed, aimed at parents | After launch | Platform paid-promotion disclosure every time. |
| Grants | Arts, cultural-heritage and educational media grants, including Korean cultural organisations | Apply in Phase 1-4 | Low cost, good fit. |

Tasks:
- [ ] Write `business/plan.md` and `business/unit-economics.md` from real pilot costs.
- [ ] Build the Club kit for 3 pilot schools, collect instructor feedback, then price it.
- [ ] Set up a simple parent-facing website (Randy decides, no child data collection).
- [ ] Quarterly review in `business/quarterly/`.

### Phase 9: Safety, compliance and trust (continuous)

Owner: `child-safety-compliance`, `content-qa`, `rights-and-licensing`.

- [ ] Every episode and short passes the red-line check: no graphic violence, no martial arts used to retaliate, no copyable dangerous stunts, no frightening body-safety content, no flashing lights or jump-scares, no off-platform calls to action.
- [ ] Every Safety Lesson has instructor sign-off and the standard disclaimer (practise with a grown-up; escape and get help first).
- [ ] No child data collected anywhere: no "comment your name", no contests needing kids' details.
- [ ] No real children's images, voices or details, including Randy's son, as input or output.
- [ ] Cultural review of every Korean history, language or costume element by the advisor.
- [ ] Apolitical always: no North/South politics, no taking sides between Taekwon-Do organisations, no present-day nation as a villain (`general-choi.md`).
- [ ] Quarterly check of YouTube, TikTok, Instagram, COPPA and AI-disclosure rules, logged in `brand/compliance-log.md`.
- [ ] Escalation: anything suggesting a child is at risk is hidden, recorded and sent to Randy at once.

### Phase 10: Measurement (continuous)

**Goal:** know whether the show is loved, and whether it actually helps kids.

| Layer | What we measure | How | Starting target (a hypothesis to revise) |
|-------|-----------------|-----|----------------------------------------|
| Love | Average % viewed, returning viewers, rewatch of legends and Safety Lessons | YouTube Analytics | Over 50% viewed on main episodes (`business-strategy`); returning viewers growing month on month |
| Reach | Views from schools and parents, shorts-to-episode flow | Platform analytics, partner reports | 10 partner schools by end of S1 |
| Learning | Can a kid explain the lesson and show the Shield skill? | Parent and instructor surveys (adults), the test viewer via Randy | Most parents report their child repeated or practised the lesson |
| Character growth | Discipline, calm, confidence, kindness at home and in class | Instructor and parent surveys each season (adults only, anonymous, aggregate) | Positive change reported by most participating instructors |
| Business | Cost per episode, revenue per episode, Club kit subscribers | `finance/ledger.csv`, `business/unit-economics.md` | Revenue covers production by the end of year 2 |
| Trust | QA pass rate, compliance issues, complaints | QA reports, compliance log | Zero red-line failures published |

Weekly report to Randy: what was made, what it cost, what the numbers say, what needs a decision.

### Phase 11: Expansion (Year 2 and beyond)

- Seasons 2-4 following the season map; the Silla thread builds to the Tong-Il finale and the finished Ripple Map.
- Live dojang events: a "Flowering Warrior Knights Day" at partner schools, run by the schools.
- A longer special (20-30 minutes) for streaming licensing.
- Translations and dubs (Korean and Spanish are natural first choices), each checked by native speakers.
- A safe, no-data companion (printed activity books first; any app or game only after a separate COPPA review and Randy's decision).

---

## 6. Changes this plan implies for the repo

This document only adds the plan. If Randy approves it, these follow-up changes bring the skills in line (each as its own small PR):

| File | Change |
|------|--------|
| `.claude/skills/series-bible/SKILL.md` | Story Circle frame, five boys and the Grandmaster, Ripple, the club, Rules v2, segments v2 |
| `.claude/skills/storytelling/SKILL.md` | Lesson rule "tenet + pattern + Shield + art"; brief template adds Shield and Flower lines |
| `.claude/skills/itf-lore/SKILL.md` | Reconciled season map (Section 4.1) |
| `.claude/skills/self-defense-lessons/SKILL.md`, `references/itf/self-defense-lessons.md` | Shield tag per lesson |
| `references/itf/hwarang.md` | New: Hwarang lore, sources, verify flags, avoid list |
| `brand/brand.md` | Title decision, promise "strong, kind, creative", Silla motifs, budgets, reviewer |
| `episodes/backlog.md`, `episodes/continuity.md` | S1 slate and starting continuity |
| `business/plan.md` | Built from Section 5, Phase 8 |
| `.claude/agents/episode-producer.md` | Show name and taste line updated after D2 |

---

## 7. Roadmap at a glance

| Weeks | Phase | Milestone |
|-------|-------|-----------|
| 1-2 | 0 Foundation | Decisions, reviewer, advisor, title shortlist, budget |
| 2-5 | 1 World and bible | Bible v2 and `hwarang.md` approved |
| 3-7 | 2 Research | Concept validated with parents, instructors and the test viewer |
| 5-10 | 3 Look and sound | Art bible, theme song, tools, cost per minute |
| 9-14 | 4 Pilot | EP001 and 3 shorts approved |
| 14-46 | 5 Season 1 | EP001-EP004 banked, then a steady cadence (16 episodes) |
| 16-20 | 6 Launch | Channels live with Randy's approval |
| 20+ | 7 Growth | Weekly reviews, school network |
| Month 4-18 | 8 Business | Club kit, printables, book, merch |
| Always | 9 Safety, 10 Measurement | Zero red-line failures; love and learning tracked |
| Year 2+ | 11 Expansion | Seasons 2-4, specials, dubs |

---

## 8. What "done" looks like for Season 1

- 16 main episodes (white to red) and about 45-50 shorts published, all with QA pass and Randy's approval.
- A kid can name the five tenets, the Five Flower Promises, and show at least five Shield skills with a grown-up.
- Parents describe the show as "exciting and good for him", not "educational but boring".
- At least 10 dojangs use the Club kit.
- The real cost per episode is known and falling; revenue streams beyond ads have started.
- Randy's son still asks for the next story.

---

## 9. Risks and how we handle them

| Risk | Why it matters | Mitigation |
|------|----------------|------------|
| Seen as "AI slop" or repetitive | Hurts trust and YouTube monetisation | Original stories, human creative input on every script, premium look, reuse only deliberate sequences |
| Arts feel "soft" to boys | Loses the core audience | The imagined legends are epic action; arts are cool skills, shown with anime energy; test early (H1) |
| Cast younger than the audience | 9-10 year olds may feel it's for little kids | Kai leads; epic imagined roles; humour pitched at 8-10; cast ages up each season; test (H4) |
| "Wise old master" stereotype | Disrespectful; dated | The Grandmaster is funny, specific and flawed; cultural advisor reviews him |
| Looks like a copy of a recent hit Korean-themed show | Legal and reputational | Original names, designs, songs; music is grounded in the Hwarang and the Manpasikjeok legend, not pop idols; rights check each design |
| Cultural inaccuracy or stereotyping | Disrespectful; loses Korean families and schools | Cultural advisor review; lore only from `references/itf/`; `[VERIFY]` until checked |
| Taekwon-Do politics | Alienates schools | "ITF-style" or "General Choi's Taekwon-Do"; Ko-Dang not Juche; never take sides |
| War stories in the patterns | Not for 6-10 | Tell values, not killing; unification as family coming together |
| Safety lesson misunderstood or misused | A child could get hurt | Instructor sign-off, escape-and-tell framing, practise with a grown-up, no strikes taught as answers |
| Character drift in AI video | Breaks the illusion | Model sheets, keyframe-first workflow, reusable assets, QA |
| Costs climb | Unsustainable | Pilot-first budgeting, cost guards, batching, log everything |
| Solo owner burnout | Show stalls | Automated pipeline with clear gates; bank episodes; a cadence Randy can keep for a year |
| Child privacy | Legal and moral | Collect nothing from kids; never use Randy's son's likeness or details; adults-only research |

---

*Next step after Randy's review: Phase 0. The `episode-producer` agent can start Phase 1 (bible v2 and `hwarang.md`) now that the frame is decided.*
