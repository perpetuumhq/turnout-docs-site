# Journey 2: Owner Onboarding — Stitch Prompts

> 6 screens covering the owner onboarding experience from welcome through page creation.

---

## Screen 2.1 — Welcome + "We Already Know You"

**Context:** Design the first screen of the owner onboarding dashboard for Turnout, a venue demand operating system. The owner has just signed up and this screen shows them that Turnout has already analyzed their venue from public data (Instagram, Google, Zomato). It should feel magical — "we did our homework." The tone is warm, competent, and slightly impressive. Target: venue owner on mobile.

**Components (top to bottom):**

- **Top Bar:** "Turnout" logo text (`#FF6B35`, Plus Jakarta Sans 800) left. Owner avatar circle (40px, `#F1F5F9` bg with initials) right
- **Welcome Section:**
  - "Welcome, [Owner Name]" in 32px H1 Plus Jakarta Sans 800, `#0F172A`
  - "We already know a lot about [Venue Name]. Let's build your page." in 16px Inter, `#475569`
- **Venue Profile Card** (white bg, 14px radius, `#E2E8F0` border, 24px padding):
  - Venue photo placeholder (full-width, 200px height, 8px radius top corners)
  - Venue name in 18px H3 Plus Jakarta Sans 700
  - Category badge: e.g., "Bars & Pubs" pill (`#FFC4A3` bg, `#8F3510` text, 20px radius)
  - Location: map pin icon + "Indiranagar, Bangalore" in 13px `#64748B`
  - **Data Sources Row:** 3 small cards in a row:
    - Instagram icon + "2.4K followers" in 12px
    - Google icon + "4.2★ (87 reviews)" in 12px
    - Zomato icon + "3.8★" in 12px
  - Divider line (`#F1F5F9`)
  - **AI-Detected Tags:** "What we found:" label in 12px caption. Row of vibe tag pills: "Craft Beer", "Live Music", "Group-Friendly", "Date Night" — each in pill style (`#F1F5F9` bg, `#475569` text, 20px radius)
  - Edit link: "Something wrong? Edit details" in 12px `#4F8DFF`
- **CTA:** "Looks right — let's build your page" primary button (full-width, `#FF6B35`)
- **Secondary:** "I need to correct some info first" text link in 13px `#64748B`

**Style:** White bg. The venue card is the focal point. Use orange sparingly (CTA + logo only). Data sources use subtle gray backgrounds. Vibe tags are light and scannable.

**Platform:** Mobile 375px. Single column. Venue card full-width minus 16px padding. 16px side padding throughout.

---

## Screen 2.2 — The −1 Journey Page

**Context:** Before building the page, Turnout shows the owner what problems they're facing and how Turnout solves them. This is an empathy-driven "we understand you" screen. It's a sales-education moment disguised as onboarding. The tone should be relatable, not preachy.

**Components (top to bottom):**

- **Header:** "Venues like yours face these problems" in 26px H2, `#0F172A`
- **Problem Cards (3 stacked):** Each card (white bg, 14px radius, 20px padding, left border 4px):
  - **Card 1** (left border `#DC2626`): Red warning icon. "Empty slots on weekdays" title in 16px 600. "Tuesday-Thursday your courts/tables sit empty. You're paying rent but earning nothing." in 14px `#475569`
  - **Card 2** (left border `#D97706`): Amber icon. "Instagram posts don't convert" title. "You post content but can't track a single walk-in back to a post." body
  - **Card 3** (left border `#64748B`): Gray icon. "WhatsApp inquiries drop off" title. "Customers message but never book. No follow-up system." body
- **Transition Text:** "Here's how Turnout fixes this for [Category] venues:" in 18px H3, `#0F172A`, 32px top margin
- **Solution Cards (3 stacked):** Each card (white bg, 14px radius, 20px padding, left border 4px `#059669`):
  - Green check icon + solution title + description
  - Card 1: "AI-powered landing pages" — "We build pages from your real photos that adapt to each customer"
  - Card 2: "WhatsApp concierge" — "Every inquiry gets a smart, personalized response that converts"
  - Card 3: "Attribution tracking" — "Know exactly which ad caused which walk-in"
- **CTA:** "Let's build yours" primary button (full-width)

**Style:** Problem cards use warm reds/ambers for empathy (not alarm). Solution cards use success green. Strong visual contrast between problem and solution sections. Clean, readable.

**Platform:** Mobile 375px. All cards stack. 16px side padding. Cards have 12px vertical gap.

---

## Screen 2.3 — Template Selection

**Context:** The owner chooses a page template from 2-3 options. Turnout recommends one based on the venue's category and data. Each template preview should look like a real mini landing page. The recommended option should be clearly marked but not forced.

**Components (top to bottom):**

- **Header:** "Pick your page style" in 26px H2. "We recommend one based on your venue type." in 14px `#475569`
- **Template Cards (2-3, vertical stack on mobile):** Each card:
  - Template preview (phone mockup, 200px height, showing a miniature page layout with colored blocks representing hero, text, gallery, CTA)
  - Template name: e.g., "Sports-Social" in 16px 600
  - Description: "Energetic, group-focused. Highlights courts, slots, and group pricing." in 13px `#64748B`
  - "Best for: Fitness, Sports, Gaming" tag in 11px `#94A3B8`
  - If recommended: Orange badge "Recommended for you" (`#FFC4A3` bg, `#8F3510` text, pill shape) pinned to top-right corner
  - Selection state: Selected card has 2px `#FF6B35` border + `#FFF3ED` background tint
  - Tap anywhere on card to select
- **Compare Link:** "Compare templates side-by-side" in 13px `#4F8DFF` (optional, expands comparison)
- **CTA:** "Use this template" primary button (shows selected template name), full-width

**Style:** Template previews use abstract color blocks (not real content) to show layout structure. Recommended badge is prominent. Selected state is clear with orange border.

**Platform:** Mobile 375px. Cards stack vertically with 16px gap. Each card full-width minus padding.

---

## Screen 2.4 — Primitive Bundle Configuration

**Context:** The owner configures their booking/commercial primitives — what type of booking system they need (slots, reservations, tickets), pricing tiers, and add-ons. This should feel like a simple configurator, not an enterprise settings page. Think "choose your setup" wizard.

**Components (top to bottom):**

- **Header:** "Set up your booking system" in 26px H2. "We'll configure everything for [Category]." in 14px `#475569`
- **Booking Type Selector:** 3 large option cards (single select):
  - Card 1: Calendar icon + "Slot Booking" + "Customers pick a specific time slot (courts, classes, sessions)" — 14px body
  - Card 2: Table icon + "Reservation" + "Customers reserve a table or spot (restaurants, bars, cafes)"
  - Card 3: Ticket icon + "Open Registration" + "Customers sign up for events or open sessions"
  - Selected: 2px `#FF6B35` border, `#FFF3ED` bg tint, orange radio dot
- **Pricing Section** (appears after booking type selected):
  - "Base pricing" label. Price input: "Rs" prefix + number field (e.g., "599"). "/per person" suffix in `#64748B`
  - Toggle row: "Enable off-peak pricing" — toggle switch (off = `#E2E8F0`, on = `#FF6B35`). When on: secondary price input appears "Off-peak: Rs ___"
  - Toggle row: "Enable group discounts" — same toggle pattern. When on: "Discount for 4+ people: ___%" input
- **Add-ons Section:**
  - "Optional add-ons" header in 18px H3
  - Checklist items with toggle: "Gear rental (+Rs ___)", "Food/drinks package (+Rs ___)", "Instructor/host (+Rs ___)"
  - Each with price input that appears when toggled on
- **CTA:** "Save & Continue" primary button, full-width

**Style:** Clean form layout. Booking type cards are large and tappable (44px+ height). Toggles use orange for on-state. Price inputs are compact but readable.

**Platform:** Mobile 375px. Everything stacks. Toggle rows are full-width with label left and toggle right. 16px side padding.

---

## Screen 2.5 — Concierge Setup

**Context:** The owner configures their WhatsApp AI concierge — choosing personality, tone, and injecting venue-specific knowledge. This should feel like "training your AI assistant." Conversational and approachable, not technical.

**Components (top to bottom):**

- **Header:** "Train your concierge" in 26px H2. "This AI assistant will chat with customers on WhatsApp. Let's give it your venue's personality." in 14px `#475569`
- **Concierge Preview Card** (centered, `#F8FAFC` bg, 14px radius, 24px padding):
  - Chat bubble mockup: AI message "Hey! Looking to book a court at [Venue]? I can help you find the perfect time." in a WhatsApp-style green bubble (`#DCF8C6` bg, `#0F172A` text, 8px radius)
  - Label: "Preview of your concierge" in 11px `#94A3B8`
- **Tone Selector:** "Pick a personality" in 18px H3. 4 radio card options:
  - "Friendly & Warm" — "Like chatting with a knowledgeable friend" (default selected)
  - "Professional & Efficient" — "Quick, direct, gets to the point"
  - "Energetic & Fun" — "Enthusiastic, uses emojis, hype energy"
  - "Calm & Reassuring" — "Patient, great for beginners and first-timers"
  - Each: white card, 14px radius, 16px padding. Selected: `#FF6B35` border + radio dot
- **Knowledge Injection:**
  - "What should your concierge know?" in 18px H3
  - Text area (full-width, 120px height, 12px radius, placeholder: "e.g., We close early on Sundays. Our most popular slot is Friday 6 PM. We offer student discounts on weekdays.")
  - Helper: "The more context you give, the better your concierge performs." in 12px `#94A3B8`
- **FAQ Preload:** "Common questions your customers ask:" in 14px 600. 3 pre-filled editable text fields:
  - "What should I bring?"
  - "Is parking available?"
  - "Can beginners join?"
  - Each with edit icon and delete icon
  - "+ Add another question" link in `#4F8DFF`
- **CTA:** "Save Concierge Settings" primary button, full-width

**Style:** The chat preview bubble adds a WhatsApp feel. Radio cards are clean and tappable. Text areas have generous padding. Warm and non-technical throughout.

**Platform:** Mobile 375px. Single column. All elements stack. 16px side padding.

---

## Screen 2.6 — Final Review + Page Creation

**Context:** The owner reviews everything before their page gets generated. This is the "launch" moment — it should feel significant and exciting, with a clear summary of all their choices and a big launch CTA.

**Components (top to bottom):**

- **Header:** "Review & Launch" in 32px H1. "Everything looks great. Let's create your page." in 16px `#475569`
- **Summary Cards (stacked):** Each summarizes a previous step:
  - **Card 1 — Venue Info:** Venue photo thumbnail (60x60, 8px radius) + name + category badge + location. "Edit" link top-right in `#4F8DFF`
  - **Card 2 — Template:** Mini template preview (48px height) + template name. "Change" link
  - **Card 3 — Booking Setup:** Booking type icon + type name + base price "Rs 599/person". "Edit" link
  - **Card 4 — Concierge:** Chat icon + tone name (e.g., "Friendly & Warm") + "3 FAQs loaded". "Edit" link
  - Each card: white bg, 14px radius, 16px padding, 1px `#E2E8F0` border
- **Estimated Timeline:** Info card (`#F8FAFC` bg, 14px radius):
  - Clock icon + "Your page will be ready in ~2 hours" in 14px 600
  - "We'll send you a WhatsApp message when it's live." in 13px `#64748B`
- **Launch CTA:** Full-width, extra height (56px), "Create My Page" text in 16px 700, `#FF6B35` bg, white text, 12px radius. Slight glow effect: `box-shadow: 0 4px 20px rgba(255, 107, 53, 0.3)`
- **Fine Print:** "You can edit everything after launch." in 12px `#94A3B8`, centered below CTA

**Style:** Summary cards are clean and scannable. Each has the edit affordance. The launch CTA is the largest, most prominent button in the entire app — this is the moment. Orange glow adds excitement.

**Platform:** Mobile 375px. All cards stack with 12px gap. CTA is sticky-bottom on mobile (above safe area).
