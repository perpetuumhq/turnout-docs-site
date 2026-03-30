# Journey 1: Owner Pre-Launch — Stitch Prompts

> 5 screens covering venue owner acquisition, pre-order, qualification, and onboarding.

---

## Screen 1.1 — turnout.so Landing Page

**Context:** Design the marketing landing page for Turnout, a venue demand operating system for India's go-out economy. Target audience is venue owners (bar owners, fitness studio operators, restaurant managers) who want to fill empty tables and slots. The page should feel warm, credible, and modern — not like a generic SaaS landing page. Think "premium tool built by people who understand nightlife and venues."

**Components (top to bottom):**

- **Sticky Nav Bar:** Left: "Turnout" logo text in Plus Jakarta Sans 800, color `#FF6B35`. Right: "See Samples" link and "Claim Your Spot" primary button
- **Hero Section (60% viewport):**
  - Headline: "Your venue deserves a landing page that works" in 48px Plus Jakarta Sans 800, color `#0F172A`
  - Subheadline: "Existing venue photos become Instagram ads. Leads go to WhatsApp. Every walk-in is attributed." in 16px Inter 400, color `#475569`
  - Primary CTA button: "Claim Your Spot" — `#FF6B35` background, white text, 14px 700, 12px radius
  - Secondary CTA: "See Sample Pages" — white bg, `#0F172A` text, 1px `#E2E8F0` border, 8px radius
  - Inline demo video placeholder (rounded 12px, 16:9 ratio) with play button overlay
- **Social Proof Row:** 3 venue cards side-by-side — each with venue photo placeholder (80x80, 8px radius), venue name in 14px bold, category badge (pill style, `#FFC4A3` bg), and a short quote in 13px italic `#64748B`
- **Feature Breakdown Section:** Header "How It Works" in 26px H2. 3 cards in a row:
  - Card 1: Camera icon + "Real Photos Only" title + "We use your actual venue photos, no stock imagery" body
  - Card 2: Sparkle icon + "AI Composition" title + "Smart landing pages that adapt to each customer" body
  - Card 3: Chat icon + "WhatsApp Concierge" title + "Leads convert in a single WhatsApp thread" body
  - Each card: white bg, 1px `#E2E8F0` border, 14px radius, 20px padding
- **Pricing Section:** Header "Simple Pricing". Two pricing cards side-by-side:
  - Card 1: "Monthly" badge, "Rs 4,999/mo", feature list (5 bullet points), secondary CTA
  - Card 2: "Annual" badge with "Save 35%" tag in `#059669`, "Rs 12,999/yr", feature list, primary CTA "Claim Your Spot"
- **FAQ Section:** 5 accordion items (collapsed by default): "How fast is setup?", "Do you use my photos?", "What if I'm not on Instagram?", "Can I cancel?", "Who has early access?"
- **Footer:** Dark navy `#0F172A` bg, white text. Turnout logo, copyright, "Designed for India's go-out economy"

**Style:** Follow design.md tokens exactly. 60% white / 25% navy / 10% orange ratio. Cards have 1px `#E2E8F0` border and 14px radius. All CTAs use `#FF6B35` with 12px radius. Body text in Inter 14px `#475569`.

**Platform:** Mobile-first, 375px width. Single column layout. Hero stacks vertically. Feature cards stack to 1-column. Pricing cards stack. Side padding 16px. Sticky CTA bar at bottom on mobile.

---

## Screen 1.2 — Pre-Order Form

**Context:** A clean, focused form page where venue owners submit their details to claim a pre-launch spot on Turnout. The page should feel quick and effortless — no more than 60 seconds to complete. Warm and professional, with trust signals.

**Components (top to bottom):**

- **Header Bar:** Turnout logo left, "Back to home" text link right
- **Progress Indicator:** Step 1 of 2, thin orange progress bar at top (50% filled, `#FF6B35`)
- **Hero Text:** "Claim your spot" in 32px H1 Plus Jakarta Sans 800. Subtext: "Takes 60 seconds. No payment required." in 16px Inter, `#64748B`
- **Form Card** (white bg, 14px radius, `#E2E8F0` border, 24px padding):
  - **Field 1:** "Venue name" label (13px Inter 600), text input (full-width, 12px radius, 14px 12px padding, 1px `#E2E8F0` border, focus: 2px `#FF6B35`)
  - **Field 2:** "Category" label, dropdown select with options: Restaurant, Cafe, Sports, Fitness, Wellness, Nightlife, Event Space
  - **Field 3:** "City" label, dropdown: Delhi, Bangalore, Mumbai
  - **Field 4:** "Owner email" label, email input with placeholder "you@venue.com"
  - **Field 5:** "Instagram handle" label (optional tag), text input with @ prefix
  - **Field 6:** "Phone (WhatsApp)" label, tel input with +91 prefix
  - All required fields marked with orange asterisk
- **Submit Button:** Full-width, "Submit Pre-Order" in primary CTA style (`#FF6B35`, white text, 12px radius, 14px 24px padding)
- **Trust Line:** Below button: Lock icon + "Your data is safe. We'll only contact you about Turnout." in 12px `#94A3B8`

**Style:** Minimal, focused. White page bg. Single centered card (max-width 480px on desktop). Orange accents only on CTA and focus states. All inputs follow form token specs from design.md.

**Platform:** Mobile 375px. Form card takes full width minus 16px padding each side. All inputs stack vertically with 16px gap between fields.

---

## Screen 1.3 — Journey Questions

**Context:** After submitting the pre-order form, venue owners answer 5-8 structured questions that help Turnout understand their venue and qualify them. This is a conversational, one-question-at-a-time flow — not a long boring form. Each question fills the screen. Think onboarding quiz, friendly and fast.

**Components:**

- **Progress Bar:** Top of screen, thin bar showing question X of 8, `#FF6B35` fill on `#F1F5F9` track
- **Question Card (full screen):**
  - Question number: "Question 3 of 8" in 12px Inter 500 uppercase, `#94A3B8`
  - Question text: e.g., "How would you describe your crowd on a Friday night?" in 26px H2 Plus Jakarta Sans 700, `#0F172A`
  - Answer options as large tappable pill buttons (full width, 16px padding, 12px radius, 1px `#E2E8F0` border). Selected state: `#FF6B35` border, `#FFF3ED` background, `#FF6B35` text
  - Example options: "Chill & conversational", "High energy & dancing", "Mixed — depends on the night", "Mostly regulars"
- **Navigation:** Bottom of screen — "Back" text link (left) and "Next" primary button (right, disabled until selection made)
- **Skip Option:** Small "Skip this question" link below options in 12px `#94A3B8`

**Style:** Clean single-card layout. One question visible at a time. Smooth transitions between questions (fade, slide-left). Pills have 44px minimum touch target.

**Platform:** Mobile 375px, full-screen cards. 16px side padding. Question text centered. Answer pills stack vertically with 12px gap.

---

## Screen 1.4 — Qualification Result

**Context:** After completing the journey questions, the owner sees their qualification score. This screen builds excitement and trust — it should feel like receiving an exclusive invite. If they qualify as "OG" (score >= 70), the celebration should be visible.

**Components (top to bottom):**

- **Celebration Animation Area:** Confetti or sparkle animation (subtle, 2s duration) for OG qualifiers
- **Score Display:**
  - Large circular score indicator: Score number (e.g., "87") in 48px JetBrains Mono 600, centered in a ring. Ring fill: `#FF6B35` for percentage, `#F1F5F9` for remainder
  - Label below ring: "Qualification Score" in 12px Inter 500 uppercase `#94A3B8`
- **Status Badge:** If OG (>=70): Large badge "You're a Turnout OG" in Plus Jakarta Sans 700, with star icon, `#FF6B35` text. If below: "Almost there" with encouragement copy
- **Breakdown Card** (white bg, 14px radius, 20px padding):
  - 4 score dimensions as horizontal bars:
    - "Content Readiness" — bar fill shows %, e.g., 80%
    - "Audience Fit" — e.g., 90%
    - "Category Demand" — e.g., 75%
    - "Location Score" — e.g., 85%
  - Each bar: `#FF6B35` fill on `#F1F5F9` track, 8px height, 4px radius
- **Next Steps Section:**
  - "What happens next" header in 18px H3
  - 3 numbered steps: "1. We'll schedule your content shoot", "2. Your AI-powered page gets built", "3. You go live and start filling tables"
- **CTA:** "Schedule Your Shoot" primary button (full-width on mobile)

**Style:** Celebratory but professional. Orange accents for score and badges. White background. Score ring is the visual centerpiece.

**Platform:** Mobile 375px. Everything stacks vertically. Score ring centered. 16px side padding.

---

## Screen 1.5 — OG Welcome + Content Shoot Scheduling

**Context:** The owner has qualified as an OG member. This screen welcomes them warmly and lets them schedule their venue content shoot. It should feel exclusive and exciting — like joining a private club.

**Components (top to bottom):**

- **Welcome Header:**
  - OG badge icon (small, inline) + "Welcome to Turnout, [Venue Name]" in 32px H1
  - "You're one of the first venues in [City]. Let's make your page unforgettable." in 16px body, `#475569`
- **OG Perks Card** (white bg, 14px radius, orange left border 4px `#FF6B35`, 24px padding):
  - "Your OG Benefits" header in 18px H3
  - 4 benefit items with check icons (`#059669`):
    - "Free professional content shoot"
    - "Priority page setup (live in 48 hours)"
    - "Dedicated account manager"
    - "Founding member pricing locked forever"
- **Shoot Scheduler Card** (white bg, 14px radius, 20px padding):
  - "Pick your shoot date" in 18px H3
  - Calendar date picker showing next 14 days. Available dates in `#0F172A`, unavailable grayed `#94A3B8`, selected date: `#FF6B35` bg circle with white text
  - Time slot selector below: 3-4 time pills ("10 AM", "2 PM", "5 PM") as selectable pills
  - Location confirmation: "[Venue Name], [Address]" with map pin icon, small "Change" link
- **CTA:** "Confirm Shoot Date" primary button (full-width), disabled until date+time selected
- **Help Line:** "Questions? Chat with us" with WhatsApp icon, `#25D366` text link

**Style:** Warm, exclusive feel. OG perks card has the orange left border accent. Calendar uses orange for selection states. Clean, uncluttered layout.

**Platform:** Mobile 375px, single column. Calendar is touch-optimized with 44px minimum day cell size. 16px side padding.
