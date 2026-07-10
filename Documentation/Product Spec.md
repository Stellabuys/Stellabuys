# Product Spec: RxStreak
### A Gamified Pharmacology Learning App for Nursing, Pharmacy & Pre-Health Students

**Category reference:** Competitive to [Epocrates: Drug Info & Pill ID](https://appmagic.rocks/iphone/epocrates-drug-info-and-pill-id/281935788)
**Strategic thesis:** "Duolingo for pharmacology" — a gamified, streak-driven quiz app that turns memorizing drug facts and spotting interactions into a daily habit and a shareable social artifact, targeting nursing/pharmacy/pre-med students where study content already goes viral organically on TikTok/IG/YouTube Shorts.

---

## 0. One-Line Pitch

RxStreak is Duolingo for drug knowledge: bite-sized daily quizzes, streaks, leagues, and a "Spot the Interaction" mini-game that turns pharmacology cramming into a game students actually want to post about.

---

## 1. Look & Feel / Brand Guidelines

### 1.1 Brand Personality
- **Energetic, not clinical.** The entire category (Epocrates, Lexicomp, Medscape) reads like a hospital intranet — grey, dense, textual. RxStreak should feel like a game first, a study tool second.
- **Confident and a little cheeky.** Borrow tone from Duolingo (playful mascot, push-notification guilt-trips) and Nurse-TikTok humor (self-aware about the absurdity of memorizing 200 beta-blockers) — never mock patient safety, but freely mock the *studying experience*.
- **Credible under the hood.** Playful skin, but every fact is pharmacist-reviewed and sourced. Brand trust is earned through a visible "Reviewed by PharmD" badge system, not a stiff tone.

### 1.2 Name & Mascot
- **App name:** RxStreak
- **Mascot:** "Dose" — a small pill-capsule character (half orange / half white capsule) with simple dot eyes, used in onboarding, streak-loss guilt notifications, and celebration animations. Deliberately simple/vector so it's cheap to animate and instantly recognizable as a sticker/GIF (built for Discord/iMessage sticker packs and TikTok overlays).

### 1.3 Color Palette

| Role | Name | Hex | Usage |
|---|---|---|---|
| Primary | **Capsule Orange** | `#FF6B35` | Primary CTA buttons, streak flame, logo |
| Primary Dark | **Deep Capsule** | `#D8491D` | Pressed states, dark-mode accents |
| Secondary | **Scrub Teal** | `#0FB5AE` | Secondary actions, correct-answer states, progress bars |
| Alert/Danger | **Interaction Red** | `#E63946` | "Contraindicated" flags in Spot-the-Interaction, streak-loss warning |
| Success | **Clear Green** | `#2EC4B6` | Correct answers, safe-combo flags |
| Warning | **Caution Amber** | `#FFB627` | "Use with caution" interaction tier |
| Neutral Dark | **Chart Ink** | `#1B1B2F` | Primary text, dark-mode background |
| Neutral Light | **Tablet White** | `#FAFAF7` | App background (light mode) |
| Neutral Mid | **Blister Grey** | `#C9C9D3` | Disabled states, dividers |

Rule of thumb: **orange = action/identity, teal = progress, red/amber/green = the interaction risk-meter system used consistently across every quiz, mini-game, and share card** so the visual language of "risk color" becomes instantly recognizable in social clips even with sound off.

### 1.4 Typography
- **Display / headers:** *Fredoka* or *Baloo 2* (rounded, friendly, high legibility at small sizes for social video overlays) — used for streak counts, score reveals, and app title.
- **Body / UI text:** *Inter* or *General Sans* — clean, highly legible at small sizes, used for quiz questions, drug monographs, settings.
- **Data/monospace accents:** *JetBrains Mono* for dosages, drug codes, and numeric stats (reinforces "clinical accuracy" against the otherwise playful UI).

### 1.5 Iconography & Illustration Style
- Flat, rounded, 2px-stroke line icons (consistent with Duolingo/Headspace-era mobile illustration trends) — no photorealistic pill imagery in the core UI (that's reserved for the actual pill-scan camera feature).
- Custom icon set for drug classes (a tiny capsule, syringe, inhaler, IV bag, patch) used as category tiles — designed to double as sticker-pack assets.
- Illustrations use a flat 3-color max palette (orange/teal/ink) to keep it cheap to produce at scale and consistent across marketing and product.

### 1.6 Motion & Sound
- Snappy, spring-based micro-animations (150–250ms) on every correct answer, streak increment, and level-up — this is the "dopamine layer" that makes screen-recordings satisfying to watch and share.
- A short, distinctive 2-note "ding" on correct answers and a signature "streak whoosh" sound — designed to be recognizable in a TikTok clip the way Duolingo's owl chime is.
- Confetti/capsule-burst animation on streak milestones (7/30/100/365 days) — the exact moment users are most likely to screen-record and post.

---

## 2. Core Functionality & Viral Highlights

### 2.1 Core Learning Loop (retention engine)
- **Daily Deck:** 5–10 bite-sized questions per day (multiple choice, drag-to-match, fill-in-the-blank) pulled from a spaced-repetition engine across drug classes, mechanisms, side effects, dosing, and nursing considerations.
- **Streaks:** Daily streak counter with streak-freeze items (earned or purchased) — the single highest-retention mechanic in Duolingo's playbook, ported directly.
- **Leagues:** Weekly leaderboard brackets (Bronze → Diamond) grouped by anonymous cohort, promoting/demoting users weekly — drives daily re-opens without needing push notifications alone.
- **XP & Mastery Tree:** Skill tree organized by drug class (cardiovascular, psych, antibiotics, pain management, etc.) with visual "mastery" fill states.

### 2.2 "Spot the Interaction" — the flagship mini-game (**primary viral feature**)
A fast-paced, timed game mode: two or three drugs/supplements flash on screen and the player has ~5 seconds to tag the combo **Green (safe) / Amber (caution) / Red (contraindicated)** before the timer runs out. Wrong or slow answers cost a life; streaks of correct answers build a combo multiplier.
- Ends in a **shareable Score Card** (see 3.5) styled like a Wordle/Spotify Wrapped result — colored emoji-style grid of your Green/Amber/Red calls plus your reaction-time score, copy-pasteable to social with zero login required to view.
- Weekly **"Beat the Community Score"** challenge deck — same 10 combos for everyone that week, so scores are directly comparable and competitive, driving organic "I got 9/10, bet you can't beat me" posts (identical mechanic to Wordle's daily-puzzle virality).
- Includes an opt-in **supplement/OTC/recreational track** (caffeine + pre-workout, melatonin + alcohol, Adderall + energy drinks) that clinical incumbents won't touch for liability reasons — this is the specific content most likely to break out of the nursing-student niche into general TikTok/college audiences.

### 2.3 Creator & Challenge Tools (**growth engine**)
- **Duel Links:** Any quiz or Spot-the-Interaction round can be packaged into a one-tap "Challenge a friend" link (iMessage/Instagram/TikTok share sheet) with no app-install requirement to view the challenger's score — classic Wordle/Poparazzi-style frictionless share loop.
- **Creator Mode:** Verified nurse/pharmacist/PharmD creators (the existing Nurse Blake / Nurse John / pharmacist-TikTok audience) get a dashboard to publish custom decks ("Sarah's ICU Med Deck"), branded score-card skins, and an affiliate code baked into the paywall — turns existing creator audiences into a distribution channel instead of competing for cold paid CPMs.
- **Duet-ready clip templates:** In-app "record my answer" mode auto-generates a vertical 15-second clip (question + countdown + reveal) formatted for direct TikTok/Reels upload — removes the biggest friction in organic UGC creation (screen-recording + editing).

### 2.4 Progression Tied to Real Credentials
- **Exam-mode decks** aligned to NCLEX-RN, NAPLEX, and USMLE Step pharm content — gives the "game" a legitimate high-stakes payoff (which drives conversion to paid) without breaking the core loop.
- **Certificates & shareable milestone badges** ("Top 1% this week in Cardiac Pharmacology") as LinkedIn/Instagram-story-ready image exports — taps professional-identity sharing, a different and higher-trust virality channel than meme content.

### 2.5 Monetization (context, not the focus of this spec)
- Freemium: 1 daily deck + limited lives free; **RxStreak Pro** subscription unlocks unlimited lives, full mastery tree, exam-mode decks, and streak-freeze inventory.
- Creator affiliate rev-share on Pro conversions attributed to a creator's decks/links.

---

## 3. Primary Screens

### 3.1 Onboarding — "Pick Your Track"
- Single question flow: *Nursing student / Pharmacy student / Pre-med / Just curious.*
- Placement quiz (5 questions) to seed initial mastery level — mirrors Duolingo's placement test, avoids a boring "start at zero" feel for advanced users.
- Ends on a streak-commitment screen ("How many days a week can you study?") that sets notification cadence — directly ported from habit-app best practice.

### 3.2 Home Dashboard
- Top: Streak flame counter + XP bar + league rank badge (always visible, always front-and-center — this is the retention anchor screen).
- Center: Today's Daily Deck card (large, single tappable CTA — "Start Today's Deck (6 min)").
- Below: Skill tree map (drug-class nodes, teal fill = mastered, grey = locked) — visually similar to Duolingo's path screen.
- Floating secondary CTA: **"Spot the Interaction" mini-game icon** (pulses if the daily community challenge hasn't been played yet) — kept visually distinct in Interaction Red/Amber/Green to reinforce it as the "fun/viral" mode vs. the "study" mode.

### 3.3 Quiz/Lesson Screen
- One question per screen, large tap targets, immediate color-coded feedback (green flash = correct, red shake = incorrect) with the 2-note sound cue.
- Progress dots at top (not a percentage bar) — gamifies "almost done" psychology.
- Post-lesson summary screen: XP earned, streak updated, mistakes reviewed, and a one-tap "Share my streak" button.

### 3.4 "Spot the Interaction" Mini-Game Screen
- Full-bleed card showing 2–3 drug/supplement names or icons; large color-coded tap zones (Green/Amber/Red) at the bottom third for thumb-reachability.
- Countdown ring animates around the card edge; combo multiplier ticks up in the corner.
- This screen is the one most designed **to be screen-recorded** — high motion, high color contrast, satisfying sound, short duration (60–90 seconds per round).

### 3.5 Score Card / Share Screen (post-game)
- Auto-generated result card: Wordle-style colored grid of Green/Amber/Red calls, final score, reaction-time stat, and the RxStreak logo/mascot.
- One-tap export presets for Instagram Story, TikTok video (auto-generates the 15-second clip template), and plain image copy for iMessage/Discord.
- "Challenge a friend" button generates the frictionless view-only link described in 2.3.

### 3.6 Leaderboard / League Screen
- Weekly bracket view (avatar, name/handle, XP this week) with promotion-zone (green) and demotion-zone (red) visually marked — same color grammar as the interaction risk-meter, reinforcing the brand's visual system.
- Countdown timer to league reset (drives end-of-week urgency and re-opens).

### 3.7 Profile / Trophy Case
- Streak history calendar (heatmap style, à la GitHub contributions graph), mastery tree completion %, and exportable milestone badges (LinkedIn/Instagram-story-ready) per section 2.4.
- Creator tab (if verified): deck performance stats, affiliate earnings, published challenge decks.

### 3.8 Creator Dashboard (secondary persona screen)
- Deck builder (question bank + custom drug combos for Spot-the-Interaction decks), branded score-card skin picker, affiliate link generator, and basic analytics (plays, shares, conversions).

---

## 4. Why This Wins on Social (Summary)

| Mechanic | Organic hook | Paid ad hook |
|---|---|---|
| Spot the Interaction score card | Wordle-style daily comparison posts | Visual, sound-on hook for 15-sec ad creative showing the countdown/reveal moment |
| Duel/Challenge links | Zero-install viewing = low-friction share loop | Retargeting via challenge-link clickers who haven't installed |
| Creator Mode | Existing nurse/pharmacist audiences distribute for you | Influencer-seeded UGC ads outperform studio-produced clinical ads |
| Streak/League milestones | Screenshot-worthy celebration animations | Use real in-app milestone clips as ad creative (proven Duolingo playbook) |
| Supplement/OTC interaction track | Taps college/biohacker audience outside core nursing niche | Broadens paid targeting beyond nursing students to general 18–30 wellness audience |
