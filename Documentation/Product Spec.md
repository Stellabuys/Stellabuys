# Product Spec: Mom's Med Box
### Caregiver-Mode Medication Management for the Adult Child Managing a Parent's Meds Remotely

**Category reference:** Adjacent to pill-reminder apps (Medisafe, MyTherapy) and elder-tech monitoring (CareZone, Lively) — but built for the *caregiver*, not the patient.
**Strategic thesis:** Every existing medication app is designed around the person taking the pills. None are designed around the adult child 200 miles away, quietly panicking about whether Mom took her blood pressure medication today. "Sandwich generation" / caregiver-burden content is one of the most reliably overperforming genres on TikTok and Instagram (millions of views on "things no one tells you about caring for aging parents," "POV: you're the default parent to your parent") — and zero apps in the medication category are built to *be* that story, let alone let people share it. Mom's Med Box turns an invisible, exhausting logistics problem into a visible, shareable act of love.

---

## 0. One-Line Pitch

Mom's Med Box is the medication app for the person doing the worrying, not just the person doing the swallowing — real-time adherence visibility, a family "care circle" so siblings stop double-texting each other, and a weekly recap built to be screenshotted and shared by an entire generation quietly carrying this alone.

---

## 1. Look & Feel / Brand Guidelines

### 1.1 Brand Personality
- **Warm, not clinical.** The competitive set (Medisafe, CareZone, hospital portals) looks like medical software. Mom's Med Box should feel like a family photo album that happens to be extremely competent — warmth first, utility second, but the utility has to be flawless because the stakes are real.
- **Calm authority, not alarmist.** Caregivers are already anxious. The app's job is to be the steadiest voice in the room — clear status, no red-alert theater unless something is actually wrong.
- **Emotionally honest.** Copy should acknowledge the guilt, distance, and mental load directly ("You checked. She's okay.") rather than pretending this is a fun productivity app. This honesty is also what makes the content shareable — it names a feeling millions of people have never seen named by a brand.
- **Multi-generational by design.** One product, two very different users: the 35–55-year-old adult child (the buyer, the sharer) and the 65–85-year-old parent (who may only ever see a large-button, low-friction "simple mode"). Every design decision gets made twice.

### 1.2 Name & Icon
- **App name:** Mom's Med Box (marketing/App Store name stays warm and specific — product itself is gender-neutral, works as "Dad's Med Box," "Grandpa's Med Box" via a one-time relationship label at onboarding).
- **App icon / mark:** A simple rounded pillbox silhouette with a small heart notch cut into the lid — reads at 40px, doubles as a favicon and a "we made it" sticker for the weekly share card. No mascot character; the emotional register here is sincerity, not cuteness, and a cartoon mascot would undercut the trust the brand needs to earn.

### 1.3 Color Palette

| Role | Name | Hex | Usage |
|---|---|---|---|
| Primary | **Terracotta** | `#C96F4A` | Primary CTAs, logo, "all good today" state |
| Primary Dark | **Baked Clay** | `#9C5236` | Pressed states, dark-mode accents |
| Secondary | **Sage** | `#7C9885` | Secondary actions, calm/neutral status, navigation |
| Warm Neutral | **Linen** | `#F6EFE7` | App background (light mode) — evokes home, not hospital |
| Alert (used sparingly) | **Ember** | `#D64545` | Missed-dose escalation, only after grace window expires |
| Caution | **Honey** | `#E3A857` | "Not yet taken today" — gentle, not alarming |
| Confirmed | **Moss** | `#4C7A5E` | "Taken" checkmarks, adherence streak fill |
| Ink | **Walnut** | `#3A2E28` | Primary text, dark-mode background |
| Divider/Disabled | **Oat** | `#DDD3C7` | Borders, disabled states |

Rule of thumb: **terracotta = brand and action, sage = calm system state, honey → ember is the only two-stage urgency ramp in the entire app.** Reserving red for one specific, rare, real event (a genuinely missed dose past the grace window) is what keeps the app trustworthy instead of anxiety-inducing — and makes the rare red moment mean something on screen recordings.

### 1.4 Typography
- **Display / headers:** *Fraunces* or *Lora* (a warm, slightly editorial serif) for the caregiver-facing app's headlines and the weekly recap card — signals "this is a life thing," not "this is a SaaS dashboard."
- **Body / UI text:** *Inter* or *Public Sans* for all functional UI — settings, medication lists, logs.
- **Parent-facing "Simple Mode":** One weight, one size floor of 22pt minimum, *Atkinson Hyperlegible* (a typeface specifically designed for low-vision readability) — this is a non-negotiable accessibility choice, not a style preference.

### 1.5 Iconography & Illustration Style
- Soft, rounded, hand-drawn-feel line icons (think a warmer version of Headspace) rather than sharp clinical glyphs — pill bottles, calendars, and phones are drawn slightly imperfect/organic.
- No stock photography of elderly people looking sad or confused (the entire category does this, and it's part of why the category feels bleak). Illustration only, warm and specific, never stock.
- A single recurring visual motif — a small sun/checkmark hybrid — used for "all taken today," so the *feeling* of relief has one consistent visual signature across notifications, widgets, and share cards.

### 1.6 Motion & Sound
- Notifications and status changes use slow, gentle easing (300–400ms) — deliberately *not* snappy/gamified, because a bouncy dopamine-loop animation on "did Mom take her pills" reads as tone-deaf.
- A single soft chime (not a buzz or alarm tone) for "confirmed taken" notifications; escalation alerts use a distinct, slightly more urgent but still non-jarring tone — never a siren.
- The weekly recap card animates in like a photo developing/fading in — reinforces the "this is a keepsake, not a stat," which is what makes people want to save and post it.

---

## 2. Core Functionality & Viral Highlights

### 2.1 Remote Adherence Dashboard (the core utility)
- Real-time "Taken / Not Yet / Missed" status per medication, per day, visible to the adult child from anywhere — no more calling to ask "did you take your pills today?"
- Confirmation via any of three methods (parent picks what's realistic for them): one-tap "I took it" button in Simple Mode, a smart pill-organizer add-on (Bluetooth-connected), or a photo-of-the-empty-slot check-in.
- Grace-window logic: a "not yet" only escalates to a caregiver alert after a configurable buffer (e.g., 2 hours past scheduled time) — this is what keeps the app calm instead of anxious.

### 2.2 Family Care Circle (**the category-defining feature**)
- Every parent profile supports multiple caregivers (siblings, a home health aide, a spouse) with shared visibility and an activity log — so "did anyone check on Mom" stops being a group-text guessing game.
- Task assignment: "Sarah has Tuesday refill pickups, Mike has weekend check-ins" — turns invisible mental load into a visible, dividable list, which is precisely the pain point the caregiver-content genre is built on.
- A private family activity feed ("Mike confirmed Mom's evening meds," "Sarah added a new prescription") replaces the fragmented text-thread status updates every caregiving family currently improvises.

### 2.3 Weekly Recap Card (**primary viral/share mechanic**)
- Every Sunday, a single auto-generated card: adherence rate, a small warm illustration, and one human-readable line ("Mom took 20 of 21 doses this week — and you were there for all of it, from 600 miles away.")
- Designed explicitly to be screenshotted and posted — same mechanic family as a Spotify Wrapped or a Peloton milestone card, but pointed at an audience (caregivers) that currently has *no* branded artifact to represent an enormous, unacknowledged effort. This is content people will post captioned "no one prepared me for this" — the exact genre already proven to overperform.
- Optional "tag a sibling" share variant that gently credits whoever helped that week — a soft, non-guilt-trippy way to surface care-sharing on social, which doubles as organic acquisition (the tagged sibling is the next install).

### 2.4 "Are You Okay?" Check-In & Escalation Chain
- A daily, low-friction wellness check-in (a single tap, a photo, or a short voice note) separate from medication logging — because the real anxiety isn't just pills, it's "is she okay today."
- If a check-in *and* a medication dose are both missed past the grace window, the app escalates automatically down a pre-set contact chain (try Mom's phone → try neighbor/backup contact → notify all caregivers) — this is the feature that converts free users into paying subscribers, because it directly answers the 2am worry.
- Integrates with existing medical alert/fall-detection hardware (Apple Watch fall detection, Life Alert-style devices) as a data source rather than trying to replace it.

### 2.5 Caregiver Community & "Invisible Labor" Content Hub
- An in-app (and social-native) space where caregivers post their own recap cards, swap practical tips, and see they're not alone — seeded with the exact relatable, validating tone that performs in the caregiver-content genre organically (posts like "things I wish someone told me before I became my parent's caregiver").
- Creator partnerships with existing caregiver-content creators (a fast-growing, underserved niche compared to the crowded parenting/fitness creator markets) to seed authentic UGC using real (anonymized/composited) recap cards — the same distribution logic as nurse-TikTok for a clinical app, but for an audience with even less existing branded content speaking to them.

### 2.6 Simple Mode (parent-facing)
- A radically reduced interface for the parent: today's medications as large tappable cards, one button per dose ("I took my morning pills"), no settings, no navigation menu, optional voice confirmation for very low-dexterity users.
- Designed to be handed to a parent with zero onboarding friction — the adult child sets it up remotely, the parent just taps.

### 2.7 Monetization (context, not the focus of this spec)
- Freemium: one parent profile, medication tracking, and manual check-ins free.
- **Care Circle Plus** subscription unlocks: unlimited care-circle members, automated escalation chain, smart-dispenser hardware integration, and pharmacy refill sync — priced and positioned as "less than one missed-dose ER visit," which is the actual comparison caregivers make.

---

## 3. Primary Screens

### 3.1 Onboarding — "Who Are You Caring For?"
- First question sets the relationship label (Mom / Dad / Grandma / a name) that personalizes all copy throughout the app — this single input is what makes every subsequent screen feel personal instead of generic.
- Quick medication import: photograph pill bottles to auto-populate the medication list (OCR on label text) rather than manual data entry — removes the single biggest setup-friction point in the category.
- Ends by inviting other care-circle members via text/email link — turns onboarding itself into the first viral loop (each parent profile naturally invites 1–3 more installs).

### 3.2 Home Dashboard (adult-child view)
- Top: today's status in one glance — a warm sun/checkmark icon if everything's confirmed, a soft honey-colored "not yet" if a dose window hasn't closed, ember only if something is genuinely overdue.
- Center: today's medication list with per-dose taken/not-yet status and timestamps.
- Below: Care Circle activity strip (small avatars of who else checked in today) — reinforces that the caregiver isn't carrying this alone.
- Persistent, low-key "Check in on Mom" button separate from medication tracking — the wellness check-in lives at the same altitude as medication status, not buried in a menu.

### 3.3 Medication Management Screen
- Full list of active medications with dose times, refill countdown, and prescribing doctor — editable by any care-circle member, with a change log so no one silently alters Mom's dosing without the family knowing.
- Refill alerts tied to pharmacy-fill data where available (pharmacy API integration) or manual countdown otherwise, surfaced a week ahead of running out.

### 3.4 Care Circle Screen
- Visual roster of everyone with access, their assigned responsibilities (refills, weekday check-ins, weekend check-ins), and a shared activity log.
- One-tap task handoff ("Can you take Tuesday?") — designed to replace the exhausting group-text negotiation that currently happens in every multi-sibling caregiving family.

### 3.5 Weekly Recap / Share Screen
- The auto-generated Sunday card described in 2.3: adherence stat, warm illustration, one human sentence, care-circle credit line.
- One-tap export presets for Instagram Story, a plain image for texting to siblings, and a "tag someone" variant — this screen is the one explicitly designed to leave the app and be seen by people who've never heard of it.

### 3.6 "Are You Okay?" Check-In & Escalation Screen
- The parent's Simple Mode surfaces one very large, friendly button per day.
- The adult child's view shows check-in status alongside medication status and lets them configure the escalation chain (who gets called, in what order, after what delay) — a calm, clearly laid-out settings screen for what is, emotionally, the highest-stakes feature in the product.

### 3.7 Simple Mode (parent device home screen)
- Today's medications as 2–3 giant cards, each with a single tap target and a large checkmark on confirmation.
- No tab bar, no settings icon, no notifications badge clutter — the entire screen is designed to be usable by someone who has never used a smartphone app confidently in their life.

### 3.8 Caregiver Community Screen
- A scrollable feed of (opt-in, shareable) recap cards and short tips from other caregivers, plus a simple "you're not alone" resource hub (links to caregiver support groups, respite care info, and the app's own blog/creator content).
- Doubles as a soft in-app retention loop and an off-app content pipeline for organic social distribution.

---

## 4. Why This Wins on Social (Summary)

| Mechanic | Organic hook | Paid ad hook |
|---|---|---|
| Weekly Recap Card | Wrapped-style shareable artifact for a huge audience with zero existing branded content to represent their effort | Real (anonymized) recap cards as testimonial-style ad creative — "no one made anything for this" as the hook line |
| "Invisible labor made visible" copy/tone | Directly names the exact feeling driving the overperforming caregiver-content genre, giving people language and a visual to post | Ad copy borrowed straight from top-performing organic caregiver posts, pointed at a real product instead of just a vent |
| Family Care Circle tag-a-sibling share | Every install is a built-in invite loop to 1–3 more caregivers in the same family | Sibling-tag flow doubles as a low-CAC referral channel |
| Caregiver-creator partnerships | An underserved creator niche (vs. saturated parenting/fitness) means outsized reach per creator dollar | UGC-style ads from real caregiver creators outperform studio-produced elder-care ads, same as nurse-TikTok for clinical content |
| "Are You Okay?" escalation feature | Word-of-mouth from the single most emotionally resonant use case in the product (peace of mind at 2am) | Direct-response ad angle: "What if today's the day she doesn't answer the phone?" |
