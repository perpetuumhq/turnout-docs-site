# Journey 4: Customer Page Experience — Stitch Prompts

> 5 core screens + 6 persona variant specifications for the consumer-facing booking flow.

---

## Screen 4.1 — Entry (Hero + Discovery)

**Context:** Design the primary customer-facing venue landing page for Turnout. This is the page a customer lands on after clicking an Instagram ad or WhatsApp link. It must capture attention in 3 seconds, build trust, and drive either a direct booking or WhatsApp conversation. The venue is a sports-social venue (pickleball/padel) in Bangalore, India. Target: young urban professionals (22-35) on mobile.

**Components (top to bottom):**

- **Hero Section (60% viewport, full-bleed):**
  - Background: Full-width venue photo (high quality, action shot of people playing). Dark gradient overlay from bottom (transparent to rgba(15,23,42,0.7))
  - Overlay content (bottom-aligned, left):
    - Venue name: "Padel Point" in 28px Plus Jakarta Sans 800, white text
    - Tagline: "Smash, laugh, repeat. Bangalore's favorite padel court." in 14px Inter 400, white with 80% opacity
  - Overlay badges (bottom-right): "Beginner-Friendly" pill (white bg, `#0F172A` text, 20px radius, 10px 14px padding)
- **Quick Info Bar** (sticky on scroll, white bg, 1px `#E2E8F0` bottom border, 12px padding):
  - 3 items in a row, evenly spaced:
    - Star icon + "4.2★ 87 reviews" in 13px JetBrains Mono 600 (tappable, `#0F172A`)
    - Pin icon + "Indiranagar" in 13px Inter 500 `#475569`
    - Clock icon + "Open till 10 PM" in 13px Inter 500 `#475569`
- **Category Badge Row:** Horizontal scroll of pill badges: "Court Booking", "Beginner-Friendly", "Group Fun", "Instagram-Worthy" — each `#F1F5F9` bg, `#475569` text, 20px radius
- **Vibe Tags:** "Casual • High-Energy • Social • Photo-Worthy" in 14px Inter, `#64748B`, centered, 16px vertical padding
- **Social Proof Section** (`#F8FAFC` bg, 16px padding, 12px radius):
  - "Popular on weekends" in 12px caption style
  - "43 people visited this week" with people icon, 14px 600
  - 3 overlapping avatar circles (28px each, 2px white border) + "+40 others"
- **Primary Offer Card** (white bg, 14px radius, orange left border 4px `#FF6B35`, 20px padding):
  - "First-timer special" in 12px caption uppercase `#FF6B35`
  - "Try padel for Rs 199" in 18px H3 Plus Jakarta Sans 700
  - "Usually Rs 599. No experience needed." in 13px `#64748B`
  - "Claim Offer" small button (`#FF6B35`, 8px radius)
- **Pricing Visibility:** "From Rs 199/person" in 16px Inter 600, `#0F172A`. "See all pricing →" link in `#4F8DFF`
- **Sticky Bottom CTA Bar** (fixed, 60px height, `#25D366` bg, 24px radius top corners):
  - WhatsApp icon (white) + "Book via WhatsApp" in 16px Inter 700, white
  - Full-width tappable area

**Style:** Hero-forward, trust-heavy. Orange accents on offers and CTAs. WhatsApp green for bottom CTA. White and `#F8FAFC` alternating sections. All text in Inter except venue name (Plus Jakarta Sans).

**Platform:** Mobile 375px. Hero is 60% viewport. Quick info bar becomes sticky after scrolling past hero. Bottom CTA always visible (fixed). 16px side padding on content sections.

---

## Screen 4.1 — Persona Variant: BEGINNER

**Context:** Same entry page but adapted for a first-timer who has never played padel. Increase reassurance, reduce anxiety, emphasize "no experience needed." Add beginner-specific trust signals.

**Modifications to base Screen 4.1:**

- Hero tagline changes to: "Never played? Perfect. Start here."
- Add prominent badge on hero: "Zero Experience Needed" (`#059669` bg, white text, pill)
- Vibe tags: replace "High-Energy" with "Beginner-Friendly"
- Social proof: Add "60% of visitors are first-timers" in 14px 600
- Insert "What to Expect" card after social proof:
  - Friendly icon + "Here's what happens when you show up:" in 16px 600
  - 3 short steps: "1. Gear provided (rackets + balls)", "2. 10-min intro from instructor", "3. Play and have fun!"
  - Each step: 13px Inter, `#475569`, numbered with orange `#FF6B35` numbers
- Testimonial card: Star rating 5/5 + "My first time and I was hooked! Instructor made it so easy." — Priya K. in 13px italic
- Offer card text: "First-time offer: Rs 199. Zero commitment. Try once and see."
- Sticky CTA text: "Chat with us — we'll help you start"

---

## Screen 4.1 — Persona Variant: GROUP ORGANIZER

**Context:** Same entry page but adapted for someone organizing a group outing (4+ friends). Emphasize group features, social fun, coordination tools.

**Modifications to base Screen 4.1:**

- Hero tagline: "Get your crew together. Courts are calling."
- Hero badge: "Great for Groups" (`#7C3AED` bg, white text)
- Add "Group Highlights" section after quick info:
  - 3 icons in a row: "Up to 20 people" + "Split payment" + "Invite friends via link"
  - Each: icon + 13px label, `#475569`
- Pricing: Show per-person with group discount: "Rs 510/person (15% group discount for 4+)"
- Social proof: "Most popular for Friday group sessions"
- Offer card: "Group deal: 4+ people save 15%. Invite your crew."
- Add "Invite Friends" button (secondary style) below offer card
- Sticky CTA: "Plan with friends on WhatsApp"

---

## Screen 4.1 — Persona Variant: SOLO

**Context:** Adapted for someone coming alone. Normalize solo attendance, emphasize meeting people and comfort.

**Modifications to base Screen 4.1:**

- Hero tagline: "Come solo. Leave with new friends."
- Hero badge: "Solo-Friendly" (`#36E4C7` bg, `#0F172A` text)
- Social proof: "40% of our visitors come solo"
- Insert "Solo Player Info" card:
  - "Open-play nights (Wed/Fri) rotate partners — you'll meet 8-10 people"
  - "No awkward intros. Just show up and play."
  - 13px Inter, `#475569`
- Testimonial: "Came alone, left with a WhatsApp group of 6 new padel buddies." — Vikram R.
- Sticky CTA: "Chat with us"

---

## Screen 4.1 — Persona Variant: PRICE-SENSITIVE

**Context:** Adapted for budget-conscious customer. Lead with value, show discounts prominently, emphasize transparency.

**Modifications to base Screen 4.1:**

- Hero tagline: "Great padel doesn't have to be expensive."
- Primary offer card moves UP to just below hero (high visual priority):
  - "Off-peak deal: Rs 239 (60% off)" in 18px H3, `#059669` text for savings
  - "Tue-Thu only. Student discount stacks: additional 15% off."
- Pricing section expanded:
  - Peak: "Rs 599/person (Fri-Sun)"
  - Off-peak: "Rs 239/person (Tue-Thu)" with "Best Value" badge in `#059669`
  - Pack: "10 visits = Rs 4,490 (Rs 449/visit, save 25%)"
- Remove premium/lifestyle imagery. Keep functional, value-forward
- Sticky CTA: "See today's deals on WhatsApp"

---

## Screen 4.2 — Single Input (Booking Picker)

**Context:** After the entry page, the customer picks their booking details. This is a focused single-purpose screen: choose date, time, and party size. It must be fast and frictionless. The UI adapts based on the venue's booking primitive (slots, reservations, or open registration).

**Components (top to bottom):**

- **Back Arrow + Step Indicator:** "← Back" left, "Step 1 of 3" right in 12px `#94A3B8`
- **Header:** "When do you want to play?" in 26px H2 Plus Jakarta Sans 700
- **Date Picker Section:**
  - Horizontal scrollable row of date cards (next 7 days):
    - Each: Day name ("Fri") in 11px `#94A3B8` + Date ("28") in 18px Plus Jakarta Sans 700 + Month ("Mar") in 11px `#94A3B8`
    - Card: 64px wide, 80px tall, 12px radius
    - Default: `#F8FAFC` bg, `#0F172A` text
    - Selected: `#FF6B35` bg, white text
    - Unavailable: `#F1F5F9` bg, `#94A3B8` text, strikethrough
- **Time Slot Grid:**
  - "Available times" label in 14px 600
  - Grid of time pills (3 columns):
    - Each: "6:00 PM" in 14px Inter 500, `#F1F5F9` bg, 8px radius, 12px 16px padding
    - Available: `#F1F5F9` bg, `#0F172A` text
    - Selected: `#FF6B35` bg, white text
    - Full: `#F1F5F9` bg, `#94A3B8` text, "FULL" small red label
    - Low availability: orange dot + "2 left" in 11px `#D97706`
  - Price shown per slot: "Rs 399" or "Rs 599" in 12px `#64748B` below each pill
- **Party Size Selector:**
  - "How many people?" label in 14px 600
  - Row of circle buttons: "1", "2", "3", "4", "5+" — each 48px circle
  - Default: `#F1F5F9` bg. Selected: `#FF6B35` bg, white text
  - Dynamic text below: "4 people × Rs 510 = Rs 2,040 (group discount applied)" in 13px `#475569`
- **Price Display** (sticky mini bar at bottom of content):
  - "Total: Rs 2,040" in 20px JetBrains Mono 600, `#0F172A`
  - "Rs 510/person (15% off)" in 13px `#059669`
- **CTA:** "Next" primary button (full-width, `#FF6B35`), disabled until all selections made

**Style:** Focused, minimal UI. Date cards are horizontal-scrollable. Time grid is compact. Party size buttons are large touch targets. Price updates dynamically.

**Platform:** Mobile 375px. Date row scrolls horizontally. Time grid is 3-column. 16px side padding.

---

## Screen 4.3 — Detail & Trust Building

**Context:** The customer has picked their slot. Before confirming, show them rich detail about what to expect, build trust with testimonials and credentials, and offer a WhatsApp escape hatch if they have questions. This page reduces anxiety and builds conviction.

**Components (top to bottom):**

- **Back + Step:** "← Back" + "Step 2 of 3"
- **Header:** "Here's what to expect" in 26px H2
- **Experience Card** (white bg, 14px radius, 20px padding):
  - Icon + "What happens when you arrive:" in 16px 600
  - Numbered list:
    - "1. Check in at reception (show your booking ref)"
    - "2. Gear provided — rackets, balls, shoes if needed"
    - "3. 10-min warm-up with instructor (for beginners)"
    - "4. 50 min of play time on your court"
  - Each: 14px Inter, `#475569`
- **Photo Gallery:** Horizontal scroll of 4 venue photos (140x140px each, 8px radius, 10px gap). Scroll indicator dots below.
- **Trust Block** (`#F8FAFC` bg, 12px radius, 20px padding):
  - 3-column grid:
    - Col 1: "4.2★" in 20px JetBrains Mono 600 + "87 reviews" in 11px `#64748B`
    - Col 2: Google icon + "4.2★ verified" in 11px
    - Col 3: Shield icon + "Verified by Turnout" in 11px
- **Testimonial Cards** (2 stacked):
  - Each: White bg, 12px radius, 16px padding. Quote in 14px italic `#475569`. Author: "— Priya K." in 13px 600 + star rating in `#FF6B35`
- **Safety & Logistics Card:**
  - "Good to know" in 14px 600
  - List items with icons: "Well-lit, busy area", "Parking available", "Beginner-friendly instructors", "All ages welcome"
  - Each: 13px `#475569`
- **WhatsApp Help Banner** (appears if user lingers >15s, `#E8F5E9` bg, 12px radius):
  - Chat icon + "Have questions? Chat with us on WhatsApp for instant help." in 14px
  - "Chat Now" small button (`#25D366`, white text, 8px radius)
- **CTA:** "Review Pricing & Book" primary button (full-width)

**Style:** Trust-focused. The trust block with 3 columns is a key credibility signal. Testimonials feel real and personal. Photo gallery adds visual richness. WhatsApp banner is help, not sales.

**Platform:** Mobile 375px. Gallery horizontal-scrolls. Trust block is 3-column grid. 16px side padding.

---

## Screen 4.4 — Reveal (Final Pricing)

**Context:** Final pricing confirmation screen before payment. Shows complete booking summary, optional add-ons, split payment toggle, and the total. Must be crystal clear — no hidden charges. This is the "moment of truth" before the customer commits.

**Components (top to bottom):**

- **Back + Step:** "← Back" + "Step 3 of 3"
- **Header:** "Here's your plan" in 26px H2
- **Booking Summary Card** (white bg, 14px radius, 20px padding, `#E2E8F0` border):
  - Venue name + category badge in one row: "Padel Point" 16px 600 + "Sports-Social" pill
  - Details grid (2 columns):
    - "Date:" — "Friday, March 28"
    - "Time:" — "6:00 PM"
    - "Duration:" — "60 minutes"
    - "Party size:" — "4 people"
  - Each row: label in 13px `#64748B`, value in 14px 600 `#0F172A`
  - Divider (`#F1F5F9`, 1px)
  - Price breakdown:
    - "Base price: Rs 599 × 4" — "Rs 2,396" (right-aligned)
    - "Group discount (15%):" — "−Rs 360" in `#059669`
    - Divider
    - "Total: Rs 2,036" in 20px JetBrains Mono 600
    - "Rs 509/person" in 14px `#059669`
  - Check icon + "No hidden charges" in 12px `#059669`
- **Add-ons Section:**
  - "Optional extras" in 14px 600
  - Toggle rows:
    - "Gear rental" — "+Rs 100/person" — toggle switch
    - "Water + energy drink" — "+Rs 75/person" — toggle
  - Price updates in real-time when toggled
- **Split Payment Toggle** (if party size > 1):
  - Card (`#F8FAFC` bg, 12px radius, 16px padding):
    - Left: Split icon + "Split payment — everyone pays their share" in 14px 600
    - Right: Toggle switch (on = `#FF6B35`)
    - Subtitle: "Payment links sent to your friends via WhatsApp" in 12px `#64748B`
- **Updated Total** (prominent):
  - "Total: Rs 2,036" in 24px JetBrains Mono 600, `#0F172A`
  - "Rs 509/person" in 16px `#059669`
- **CTA Buttons:**
  - Primary: "Book Now" (full-width, `#FF6B35`, 56px height for emphasis)
  - Secondary: "Reserve via WhatsApp" (`#25D366` bg, white text, full-width)

**Style:** Clean, transparent pricing. Summary card is well-organized with clear hierarchy. Discounts in green (`#059669`). Total is the largest number on screen. Two CTA options give flexibility.

**Platform:** Mobile 375px. Single column. Add-ons inline. 16px side padding. CTAs stack vertically with 12px gap.

---

## Screen 4.5 — Activation (Booking Confirmed)

**Context:** The customer has booked! This is the celebration screen. It confirms the booking, provides all practical info (what to bring, directions), and encourages sharing/referrals. It should feel rewarding and exciting.

**Components (top to bottom):**

- **Celebration Header:**
  - Large check circle icon (64px, `#059669` bg, white check, centered)
  - "You're all set!" in 32px H1 Plus Jakarta Sans 800, centered
  - "Booking ref: TN20260328ABC" in 14px JetBrains Mono, `#64748B`, centered
- **Confirmation Card** (white bg, 14px radius, 20px padding):
  - Venue name + date + time in compact format
  - "4 people · Court 2 · Rs 509/person"
  - Divider
  - "What to bring:" section with icons:
    - Water bottle icon + "Water bottle"
    - Towel icon + "Towel"
    - Shoe icon + "Sports shoes (rackets provided)"
  - "Arrive 10 min early for court orientation" in 13px `#D97706` (amber, attention)
- **Action Buttons (horizontal row):**
  - "Add to Calendar" small button (secondary style, calendar icon)
  - "Get Directions" small button (secondary, map icon)
  - "Call Venue" small button (secondary, phone icon)
- **Shareable Card Preview** (`#F8FAFC` bg, 14px radius, 20px padding):
  - Mini card preview (booking details as a screenshot-friendly visual)
  - "Share with your group:" label
  - Buttons row:
    - "Share on WhatsApp" (`#25D366` bg, white, full-width)
    - "Share on Instagram" (gradient bg, white)
    - "Copy Link" (secondary, link icon)
- **Referral Section** (if enabled, `#FFF3ED` bg, 14px radius, 20px padding):
  - Gift icon + "Invite friends, earn credit" in 16px 600
  - "Your friend books → You get Rs 100 credit" in 14px `#475569`
  - Referral link: "turnout.so/ref/ABC123" in JetBrains Mono 13px + copy button
  - "Copy Referral Link" small orange button
- **Next Steps Card:**
  - "What happens next:" in 14px 600
  - "24h before: You'll get a reminder" + clock icon
  - "4h before: Final check-in reminder" + bell icon
  - "See you there!" in 16px Plus Jakarta Sans 700, `#FF6B35`
- **CTA:** "Done" secondary button (closes page)

**Style:** Celebratory but informative. Green check for success. Share buttons are prominent. Referral section is warm (orange bg tint). Practical info is well-organized.

**Platform:** Mobile 375px. Stacks vertically. Share buttons can be 2-column grid. 16px side padding.
