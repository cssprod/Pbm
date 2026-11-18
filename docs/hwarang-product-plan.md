# Product Development Plan: The Flower Knights Return

*A phased plan to turn the kids ITF Taekwon-Do anime into a show that modern 6-10 year olds choose to watch, and that grows discipline and the ability to defend themselves physically, mentally and emotionally.*

- Owner and final approver: Randy
- Status: draft v1, 2026-11-18, for Randy's review
- Builds on: the production skills and `episode-producer` agent (`.claude/`, PR #1), the ITF lore library (`references/itf/`, PR #2), and `brand/brand.md`
- Timeline convention: "Week 1" is the week Randy approves this plan. Dates move with his decisions, not the other way round.

---

## 0. Decisions Randy needs to make first

These change the goal, so they are Randy's. Everything else in the plan can start without them, using the recommended option.

| # | Decision | Options | Recommendation |
|---|----------|---------|----------------|
| D1 | How the Hwarang idea fits the existing show | **Wrap:** keep the 24 Doors world and make the kids a modern Hwarang club. **Replace:** rebuild the show around a new Hwarang world. | **Decided 2026-11-18 by Randy: Wrap.** Keeps the pattern-a-door engine (which already maps to all 24 legends) and adds the Hwarang as the heart of the team. Less rework, stronger premise. |
| D2 | Show title | Keep *Tiger Belt: The 24 Doors*; or a Hwarang-led title such as *Flower Knights*, *The Flower Knights of the 24 Doors*, *Hwarang Rising* | Shortlist 3, run trademark and search checks (Phase 0), then concept-test with parents (Phase 2). Do not lock before checks. |
| D3 | Budgets | Per main episode, per short, per month (fields in `brand/brand.md` are still blank) | Set a pilot-only budget first; set season budgets after the pilot's real cost is known. |
| D4 | Instructor reviewer | A named ITF instructor (rank, school) who signs off technique and safety lessons | Required before any safety lesson is published. |
| D5 | Korean cultural advisor | A Korean or Korean-diaspora advisor (paid or volunteer) who reviews history, language and visuals | Strongly recommended before the pilot is locked. |
| D6 | Voices | AI voices, human voice actors, or a mix | Human or licensed voices for the four leads; AI for temp tracks and minor parts. Kids hear the difference, and it protects monetisation. |
| D7 | Release cadence | Starting target from `production-pipeline`: 1 main episode every 2 weeks, 3 shorts a week | Bank 4 finished episodes before launch, then hold the cadence you can keep for a year. |

---

## 1. Vision

### 1.1 The problem

Taekwon-Do's stories and lessons are wise, deep and emotionally mature. But to a modern kid, the way they are usually presented looks black-and-white and strict: lines, counting, silence, rules. Meanwhile kids' media competes for attention with fast, funny, colourful, music-driven shows and games. The lessons are not the problem. The packaging is.

### 1.2 The answer: bring back the Flower Knights

The **Hwarang** ("flower youth", "flowering knights") of the Silla kingdom were young people who trained in martial arts **and** in poetry, music, dance and good manners, and who travelled mountains and rivers to grow strong and wise (`references/itf/patterns.md`, Hwa-Rang). General Choi drew on their ideals, and the pattern **Hwa-Rang** is named after them. The Hwarang are the bridge we need: they make "strong" and "creative" the same thing.

**The premise in one line:** the world needs the Flower Knights again, and this time they are ordinary modern kids who discover that a kick, a drawing, a drumbeat and a kind word can all come from the same brave heart.

### 1.3 What we promise

| To kids | To parents |
|---------|-----------|
| An exciting anime adventure with friends, a funny tiger, magic doors, music and powers that grow as you level up. | A show that builds discipline, confidence, emotional skills and real safety skills, with nothing you would not want your child to copy. |
| "I can do that too": moves and songs to try at home. | Honest about AI use, Made for Kids, no data collected from children, reviewed by a real instructor. |

### 1.4 Why this can win against modern kids' shows

Design principles drawn from what holds 6-10 year olds (to be validated in Phase 2, treat as hypotheses):

1. **A team, not a lecture.** Kids love a crew where each member has a distinct power and personality. The Hwarang were a team; our club is a team.
2. **Levelling up you can see.** Belts, the Belt Tree, badges for arts, doors opened. Collecting and growing are core pleasures at this age.
3. **Music as power.** Music-driven, Korean-flavoured kids' media has shown huge appeal recently; Hwarang musicians give us an authentic, original reason to make music central. We must stay clearly original (see Section 9, risks).
4. **Funny every 30 seconds** (`storytelling`): Bori and Leo carry the comedy.
5. **Real-world payoff.** Every episode ends with something a kid can do: a move, a breath, a safety skill, a kind act.
6. **Fantasy grounded in true stories.** "This really happened" (or "this is a real legend") is a superpower that most fantasy shows do not have.

---

## 2. The framework: Three Shields and the Flower

Randy's goal is a child who can defend himself **physically, mentally and emotionally**. We make that explicit, visible and collectable.

| Shield | What it protects | Built from | Examples already in the library |
|--------|------------------|-----------|--------------------------------|
| **Body Shield** | Physical safety | Stances, distance, voice, escapes, falling, getting help | SD-01 Be the Boss of Your Space, SD-02 Confident Stance, SD-03 Power Voice, SD-04 Stop Hand, SD-13 to SD-20 escapes and falls |
| **Mind Shield** | Clear thinking under pressure | Spotting tricks and lies, online safety, choosing your thoughts, awareness | SD-11 Online Safety Shield, SD-21 Spot the Exits, SD-22 Buddy System, SD-23 Tricky People; Won-Hyo "your thoughts change your feelings" |
| **Heart Shield** | Emotional strength | Naming feelings, calming down, resilience after failure, empathy, standing up for others | SD-24 Calm Body Clear Mind, SD-08 Walk Away, SD-09 Words That Shield, SD-10 Upstander, SD-25 Making Peace |
| **The Flower** (the Hwarang gift) | The creative, compassionate, collaborative mind | Each kid's art, teamwork, kindness | Hwa-Rang pattern moral: "strength plus kindness and creativity" |

How it shows on screen:
- Each episode earns one Shield skill (the Safety Lesson) and shows one tenet beating the Gloom.
- A kid "Blooms" when a tenet, a pattern and their art come together: their belt knot glows, petals and light, and their art becomes a power that **builds, calms, heals or connects, never hurts**.
- The **Shield Board** in the dojang tracks the club's earned skills: a visible, collectable progress system that kids can copy at home on a printable chart (sold or given to parents, never collected from kids).

Episode formula update (extends the lesson rule in `storytelling`):
**one tenet + one pattern or belt meaning + one Shield skill + one art moment.**

Tie to the Student Oath (`tenets-and-oath.md`): "I shall never misuse Taekwon-Do" and "I shall build a more peaceful world" become the club's mission. The Flower Knights' job is peace.

---

## 3. Creative concept: the world and characters (series bible v2)

All lore comes from `references/itf/`. Anything not in the library is marked `[VERIFY]` and kept off screen until checked.

### 3.1 Where the Hwarang fit ("wrap", decided by Randy on 2026-11-18)

- **The Dojang (real world)** stays: a warm neighbourhood Taekwon-Do school.
- **The Great Clock and its 24 Doors** stay: each pattern opens its legend.
- **New: the Flower Knights Club.** In the pilot, Grandma Park tells the bedtime legend of the Hwarang. Kai, Hana and Leo decide to start their own club at the dojang: modern Flower Knights who train hard and make things.
- **New: Sol, a Hwarang guide from the legend world.** A fictional teenage Hwarang (not a historical person) who plays a bamboo flute and steps out of the Clock to guide the kids through the doors. Sol gives the Hwarang a presence in every episode long before the kids reach the Hwa-Rang pattern at red belt. Sol is cheerful, poetic, a bit old-fashioned about modern things (comedy: Sol versus a vending machine), and the kids teach Sol as much as Sol teaches them.
- **The season mystery:** one door on the Clock never glows. It is the Hwa-Rang door. Why can't Sol go home? The answer pays off when the kids reach red belt and earn it, by living the five Flower Promises together.

### 3.2 The Five Flower Promises

The Hwarang had five rules from the monk Won-Gwang (`patterns.md`, Hwa-Rang). We use the library's kid versions as the club's charter, recited alongside the Student Oath:

1. Love your home and the people in it. *(from "be loyal to your country")*
2. Respect your parents.
3. Be a true friend.
4. Never give up. *(from "never retreat in battle")*
5. Be gentle with every living thing; only use force when you truly must. *(from "never take a life without good reason")*

### 3.3 Cast v2

Keeps the existing cast (`series-bible`) and gives each kid a Flower (art), a Shield strength, and a flaw to grow out of.

| Character | Belt (S1) | Flower (art) | Shield strength | Flaw and growth |
|-----------|-----------|--------------|-----------------|-----------------|
| **Kai**, 8, hero | White | Rhythm: drums, beatboxing, the kihap as a beat | Body | Wants to be strong fast; learns patience and self-control |
| **Hana**, 9 | Yellow | Poetry and brush lettering (echoes young General Choi, who studied calligraphy with a Taekkyon master, `general-choi.md`) | Mind | Too careful; learns indomitable spirit |
| **Leo**, 7 | White | Drawing and comics; his sketches come alive in the legend world | Heart | Afraid to try; learns perseverance |
| **New member** (introduced ep 3 or 4), 8-9 | White | Dance or b-boying, or building and inventing (choose in Phase 1) | Body/Mind | Show-off who doesn't listen; learns courtesy |
| **Bori**, tiger cub spirit | n/a | Cheers everyone on, terrible singer | n/a | Grows as Kai grows |
| **Sol**, Hwarang guide (fictional) | n/a | Bamboo flute, poems about mountains | All | Homesick; learns that home is people |
| **Sabum Han**, 6th dan | n/a | Secretly paints | n/a | Knows more about the Clock than he says |
| **Grandma Park** | n/a | Storyteller | n/a | Her stories match the doors |
| **The Gloom** | n/a | Shadow fog | n/a | Whispers "give up", "you're not good enough", "just hit them"; shrinks when a tenet is used |

Diversity and gender: the historical Hwarang were young men of Silla. Our modern club is open to every kid (Hana is a founding member). The show still aims at boys 6-10 through its energy, humour and action.

### 3.4 Rules of the magic (v2, extends `series-bible`)

1. Doors open through focus, practice and a tenet, never through strength alone.
2. In a legend, kids can watch, help and learn; they never change real history.
3. The Gloom is beaten by tenets and creativity, never by hurting anyone.
4. Arts are powers that build, calm, heal or connect. Never a weapon.
5. A Bloom needs the team: no kid saves the day alone for long.
6. Every adventure brings one lesson home to Kai's real-world problem.

### 3.5 Silla thread (the Hwarang story across the whole series)

Several of the 24 patterns belong to Silla and connect directly to the Hwarang. This is our long arc:

| Pattern | Belt | Silla link (from `patterns.md`) | Role in the arc |
|---------|------|------------------------------|-----------------|
| Won-Hyo | 6th kup | Silla monk who shared his teaching with everyday people, singing and dancing in the streets | First trip to Silla; Sol's world |
| Hwa-Rang | 2nd kup | The Hwarang youth group | The locked door opens; the kids meet the original Flower Knights |
| Yoo-Sin | 3rd Dan | General Kim Yoo-Sin, who trained as a 17-year-old Hwarang; 668 AD, the year Korea was united | "Why do you train?" Owning mistakes |
| Moon-Moo | 4th Dan | King of Silla; the legend of the flute that calms ten thousand waves | Sol's flute and the power of music to bring peace |
| Tong-Il | 6th Dan | "Becoming one again" | Series finale: two halves become one, mirroring Chon-Ji |

**How we tell unification:** as three families of one people learning to become one family, not as conquest. Heroes from the other two kingdoms also have patterns (Kwang-Gae from Koguryo, Ge-Baek from Baekje), so no kingdom is ever the villain. On screen say "Korea's Three Kingdoms". (Note: the Three Kingdoms, Koguryo, Baekje and Silla, covered the whole Korean peninsula and beyond, not only present-day South Korea.)

Facts to verify before they appear on screen `[VERIFY]`:
- The Hwarang's founding date. The ITF definition says "early 7th century"; many histories date the group's formal organisation to the 6th century under King Jinheung. Quote the ITF definition for the pattern and keep other dates off screen until checked against `sources.md` S10/S12.
- Any claim that the Hwarang "won" the unification. Say "Hwarang like Kim Yoo-Sin helped unite Korea's Three Kingdoms" only after it is checked.
- Any details from the *Hwarang Segi* manuscript, whose authenticity is disputed `[VERIFY]`.

Always avoid: the story of the boy Hwarang Gwan-Chang dying in battle; battle deaths; Kim Yoo-Sin beheading his horse (`patterns.md`).

### 3.6 Tone

Exciting first, wise second, funny always. Anime energy at a gentle level. Real but kid-sized conflicts. Adults are wise and kind. Martial arts never settle a playground argument (`series-bible`). The Hwarang add beauty: mountains, flutes, petals, ink, music.

### 3.7 Recurring segments (v2)

1. Cold open hook (5-10 s)
2. Real-world problem
3. Practice, the door glows
4. The legend, with Sol
5. The Gloom moment and the Bloom
6. Back home: the lesson used
7. Bori's Fact (5 s)
8. **Sabum Han's Safety Lesson** with the Shield icon earned
9. **The Flower Promise** chant and sign-off: "Train with heart. Make something kind. See you behind the next door!" plus the bow

---

## 4. Season architecture

### 4.1 Reconciling the two season maps

The repo has two season maps: `itf-lore` (5 short seasons, 2 patterns each) and `references/itf/README.md` (Season 1 covers all colour belts). Recommendation: a middle path that lets the show grow with the viewer, keeps the Hwarang payoff as a big event, and gives each season a natural finale (a grading).

| Season | Belt journey | Patterns | Big idea | Finale |
|--------|--------------|----------|----------|--------|
| **S1: The Flower Knights Return** (10 eps) | White to Green | Chon-Ji, Dan-Gun, Do-San, Won-Hyo, plus General Choi origin and the Oath | Every Flower Knight starts as a seed | Green belt; the locked door is revealed |
| **S2: Roots and Sky** (10 eps) | Green to Blue to Red | Yul-Gok, Joong-Gun, Toi-Gye | Wisdom, courage, humility | Red belt; the Hwa-Rang door begins to glow |
| **S3: The Hwa-Rang Door** (8-10 eps) | Red to Black | Hwa-Rang, Choong-Moo | Strong and gentle; never give up | Black belt; Sol goes home, and stays a friend |
| **S4 onward: Black Belt Legends** | Dan patterns | Kwang-Gae to Tong-Il, with the Silla thread (Yoo-Sin, Moon-Moo) | Legends told and lived | Tong-Il series finale |

### 4.2 Season 1 episode slate (draft, for `episodes/backlog.md`)

Tenets and Safety Lessons follow the library's pairings (`patterns.json`, `self-defense-lessons.md`) where they exist.

| Ep | Working title | Pattern / theme | Tenet | Shield skill | Flower moment |
|----|---------------|-----------------|-------|--------------|---------------|
| 1 | The Seed and the Flower (pilot) | White belt + Chon-Ji; Grandma's Hwarang tale; Sol arrives | Courtesy | SD-01 Be the Boss of Your Space (Body) | Kai's first beat |
| 2 | The Bear Who Waited | Dan-Gun | Perseverance | SD-02 Confident Stance (Body) | Leo draws the 21-day counter |
| 3 | Five Flower Promises | Student Oath + the Hwarang rules; the club is founded | Integrity | SD-06 My Trusted Adults Team (Heart) | Hana writes the club charter |
| 4 | Yellow Belt Day | First grading; the new member joins | Self-Control | SD-03 Power Voice (Body) | Kai's kihap beat |
| 5 | The Boy Who Cleaned the Street | Do-San | Integrity | SD-04 Stop Hand (Body) | The club paints a mural |
| 6 | The Small Boy Who Wouldn't Give Up | General Choi origin | Indomitable Spirit | SD-08 Walk Away Like a Black Belt (Heart) | Hana's brush lettering |
| 7 | Words That Shield | A bullying story at school | Courtesy | SD-09 Words That Shield (Heart) | Leo's comic answers a bully |
| 8 | The Sweetest Water | Won-Hyo; first trip to Silla | Self-Control | SD-05 No, Go, Yell, Tell (Body) + SD-24 Calm Body (Heart) | Sol's flute |
| 9 | The Gloom Goes Online | Applying the Mind Shield to screens | Integrity | SD-11 Online Safety Shield (Mind) | The team makes a song |
| 10 | Green Belt Bloom (finale) | Green belt grading; the locked Hwa-Rang door | All five | Review of S1 Shields | First full-team Bloom |

Plus about 30 shorts for S1: "Legend in 45", Safety Lesson shorts, Bori's Facts, Pattern Challenges, and new **Flower shorts** (a 30-second art challenge: "draw a bear who waits", "make a kihap beat").

---

## 5. The phased plan

Each phase lists its goal, steps and tasks, the skill or file that owns the work, the deliverable, and the gate that must pass to move on. Phases 9 (safety) and 10 (measurement) run continuously alongside the others.

### Phase 0: Foundation and decisions (Weeks 1-2)

**Goal:** settle the decisions and set-up that everything else depends on.

1. Decisions
   - [ ] Randy decides D1-D7 (Section 0).
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
   - [ ] Update the skill with: Flower Knights Club, Sol, Cast v2, arts and Shields, the Bloom, Rules of the magic v2, recurring segments v2.
   - [ ] Design the new club member (dance or maker; pick one in a 3-option concept test in Phase 2).
   - [ ] Write character one-pagers: voice, catchphrase, what they want, what they fear, how they Bloom.
   - [ ] Define the Gloom's limits: spooky fog only, never horror (`child-safety-compliance`).
3. Story system (`storytelling`, `itf-lore`, `self-defense-lessons`)
   - [ ] Update the lesson rule to "tenet + pattern + Shield + art".
   - [ ] Tag every SD lesson with its Shield (Body, Mind, Heart).
   - [ ] Reconcile the season map (Section 4.1) in `itf-lore`.
   - [ ] Seed `episodes/backlog.md` with the S1 slate (Section 4.2) and `episodes/continuity.md`.
4. Season arc
   - [ ] Write the S1 arc document: Sol's homesickness, the locked door mystery, each kid's growth line, where each new skill is planted and paid off.
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
   - H1: kids find the art-powers exciting, not "soft". Signal: they ask to see a Bloom again or copy it.
   - H2: parents value the Three Shields framing. Signal: it is the top reason they would show the show.
   - H3: Sol is a favourite. Signal: kids mention Sol unprompted.
   - If H1 fails, lean the Bloom towards action and kihap; keep arts as the source, not the spectacle.

**Deliverables:** `analytics/comparables.md`, interview and survey notes, concept-test results, a one-page "what we learned" memo.
**Gate:** at least 2 of 3 hypotheses supported, or a revised concept that Randy approves.

### Phase 3: Look and sound development (Weeks 5-10)

**Goal:** a visual and audio identity that looks premium and stays consistent through AI generation.

1. Art direction (`art-direction`)
   - [ ] Style frames for: the dojang, the Great Clock, a Silla mountain and river scene, the Bloom effect.
   - [ ] Character model sheets for every lead (turnarounds, expressions, belt-knot details, Sol's Silla-inspired clothes reviewed by the cultural advisor).
   - [ ] Shield and Flower icon set; the Shield Board.
   - [ ] Colour script per belt colour; Silla palette (petals, ink, bamboo).
2. Generation tests (`video-generation`)
   - [ ] Test 2-3 image and video tools on the same 10-shot sequence. Score consistency, motion quality, lip-sync, cost per finished second, and commercial-use terms.
   - [ ] Build the reusable asset library: backgrounds, the door-opening sequence, the Bloom sequence, the bow, the Safety Lesson set (reuse cuts cost and keeps the look consistent).
3. Sound (`voice-and-music`)
   - [ ] Theme song: catchy, chantable, built around the kihap and a bamboo-flute hook. Licensed or composed for hire with full rights.
   - [ ] Musical signatures: each kid's art has a sound (Kai's beat, Sol's flute, Hana's brush swish, Leo's pencil scratch).
   - [ ] Voice casting for the leads (D6). Korean pronunciation guide from `terminology.md`, checked by the advisor.
   - [ ] Sound library: door, Bloom, Gloom whisper (soft, never a jump-scare), kihap.
4. Costing
   - [ ] Measure the real cost per finished minute and per short, and log it (`accounting`).

**Deliverables:** art bible, model sheets, tool decision, theme song, cast, cost per minute.
**Gate:** Randy approves the look and the theme; cost per minute fits the budget.

### Phase 4: Pilot (Weeks 9-14)

**Goal:** one finished main episode and 3 shorts that prove the show.

1. Run EP001 "The Seed and the Flower" through all 12 stages of `production-pipeline`: brief, outline, script, storyboard, generate, audio, edit, package, QA, approval.
2. Script gates
   - [ ] Script read for "a laugh every 30 seconds", Kai makes the winning choice, one tenet shown not preached.
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

### Phase 5: Pipeline scale-up and Season 1 production (Weeks 14-30)

**Goal:** produce Season 1 at a steady, affordable cadence without losing quality.

1. Batching (`production-pipeline` rule 6)
   - [ ] Write scripts in batches of 3-4; generate visuals for a batch together for consistency.
   - [ ] Lock reusable sequences (door, Bloom, Safety Lesson set, sign-off).
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
   - Cold-open styles; episode length (4 vs 6 minutes); Sol-led vs Kai-led legends; Bloom early vs late.
   - Shorts mix: Safety Lesson vs Legend vs Flower challenge.
3. Community without collecting kids' data:
   - "Train along" episodes and pattern challenges kids do with a grown-up at home.
   - Parent-facing challenges on TikTok and Instagram ("practise the Stop Hand with your child tonight").
4. School network (strongest channel):
   - The **Flower Knights Club kit** for dojangs (see Phase 8): schools use episodes in class, and families find the channel through their school.
   - Track outreach in `business/partners.md`; the agent drafts emails, Randy sends.
5. Cultural partners: Korean cultural centres, Korean-language schools, Children's Day (Korea, 5 May) and Gaecheonjeol (3 October) themed releases.
6. Feed learnings back: each month update the backlog and one skill with what worked.

### Phase 8: Business and products (Month 4 to Month 18)

**Goal:** revenue that covers production, from sources that fit a Made for Kids channel.

Made for Kids means no personalised ads, comments, merch shelf, notification bell, cards or end screens (`child-safety-compliance`). So ads are a base, not the plan (`business-strategy`).

| Stream | What | When | Notes |
|--------|------|------|-------|
| **Flower Knights Club kit for dojangs** | A monthly class programme: episode, printable pattern sheet, Safety Lesson guide for instructors, a Flower art challenge, Shield certificates | Pilot onward; paid from S1 | Strongest fit. Schools pay a licence or sponsor an episode (credit aimed at parents). |
| YouTube ads (YPP) | MFK ads | After YPP eligibility | Low revenue per view; keep authenticity high to stay eligible. |
| Printables for parents | Shield Board chart, belt-progress chart, colouring pages, the Five Flower Promises poster | From launch | Sold on a parent-facing site, never linked to kids from MFK videos. |
| Picture books | One per season ("The Bear Who Waited", "The Flower Knights") | After S1 | Strong gift market; reuses art. |
| Merch | Bori plush, Shield patches for belts, Flower Knights wristbands in belt colours, bamboo practice flute | After S1 traction | Sold via the parent site and partner schools. Product safety and toy-testing rules apply (Randy gets advice first). |
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
| Love | Average % viewed, returning viewers, rewatch of Blooms and Safety Lessons | YouTube Analytics | Over 50% viewed on main episodes (`business-strategy`); returning viewers growing month on month |
| Reach | Views from schools and parents, shorts-to-episode flow | Platform analytics, partner reports | 10 partner schools by end of S1 |
| Learning | Can a kid explain the lesson and show the Shield skill? | Parent and instructor surveys (adults), the test viewer via Randy | Most parents report their child repeated or practised the lesson |
| Character growth | Discipline, calm, confidence, kindness at home and in class | Instructor and parent surveys each season (adults only, anonymous, aggregate) | Positive change reported by most participating instructors |
| Business | Cost per episode, revenue per episode, Club kit subscribers | `finance/ledger.csv`, `business/unit-economics.md` | Revenue covers production by the end of year 2 |
| Trust | QA pass rate, compliance issues, complaints | QA reports, compliance log | Zero red-line failures published |

Weekly report to Randy: what was made, what it cost, what the numbers say, what needs a decision.

### Phase 11: Expansion (Year 2 and beyond)

- Seasons 2-4 following the season map; the Silla thread builds to the Hwa-Rang door and the Tong-Il finale.
- Live dojang events: a "Flower Knights Day" at partner schools, run by the schools.
- A longer special (20-30 minutes) for streaming licensing.
- Translations and dubs (Korean and Spanish are natural first choices), each checked by native speakers.
- A safe, no-data companion (printed activity books first; any app or game only after a separate COPPA review and Randy's decision).

---

## 6. Changes this plan implies for the repo

This document only adds the plan. If Randy approves it, these follow-up changes bring the skills in line (each as its own small PR):

| File | Change |
|------|--------|
| `.claude/skills/series-bible/SKILL.md` | Flower Knights Club, Sol, Cast v2, Rules v2, segments v2 |
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
| 14-30 | 5 Season 1 | EP001-EP004 banked, then a steady cadence |
| 16-20 | 6 Launch | Channels live with Randy's approval |
| 20+ | 7 Growth | Weekly reviews, school network |
| Month 4-18 | 8 Business | Club kit, printables, book, merch |
| Always | 9 Safety, 10 Measurement | Zero red-line failures; love and learning tracked |
| Year 2+ | 11 Expansion | Seasons 2-4, specials, dubs |

---

## 8. What "done" looks like for Season 1

- 10 main episodes and about 30 shorts published, all with QA pass and Randy's approval.
- A kid can name the five tenets, the Five Flower Promises, and show at least five Shield skills with a grown-up.
- Parents describe the show as "exciting and good for him", not "educational but boring".
- At least 10 dojangs use the Club kit.
- The real cost per episode is known and falling; revenue streams beyond ads have started.
- Randy's son still asks for the next door.

---

## 9. Risks and how we handle them

| Risk | Why it matters | Mitigation |
|------|----------------|------------|
| Seen as "AI slop" or repetitive | Hurts trust and YouTube monetisation | Original stories, human creative input on every script, premium look, reuse only deliberate sequences |
| Arts feel "soft" to boys | Loses the core audience | Blooms are action spectacles; arts are the source of power, shown with anime energy; test early (H1) |
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

*Next step after Randy's review: Phase 0. The `episode-producer` agent can start Phase 1 (bible v2 and `hwarang.md`) as soon as D1 is decided.*
