# Journey 3: Owner Testing & Approval — Stitch Prompts

> 6 screens covering customer mode preview, feedback, approval, and shareable artifacts.

---

## Screen 3.1 — Customer Mode Toggle

**Context:** Design a dashboard screen for venue owners on Turnout where they can switch into "Customer Mode" to preview their page exactly as customers see it. The toggle should be prominent and the concept immediately clear. This is the owner's control center before going live.

**Components (top to bottom):**

- **Dashboard Nav:** Turnout logo left, venue name center in 14px 600, owner avatar right (40px circle)
- **Page Status Banner** (`#FFF3ED` bg, 12px radius, 16px padding):
  - Status dot (8px circle, `#D97706` amber for "draft" or `#059669` green for "live") + "Your page is in draft" in 14px 600
  - "Last updated 2 hours ago" in 12px `#94A3B8`
- **Customer Mode Card** (white bg, 14px radius, `#E2E8F0` border, 24px padding, centered):
  - Phone mockup illustration (abstract, showing a mini page preview — hero + cards + CTA)
  - "Experience Your Page" in 18px H3 Plus Jakarta Sans 700, centered
  - "See your page exactly as customers see it. Test the booking flow, check the copy, and flag anything." in 14px Inter, `#475569`, centered
  - Primary CTA: "Enter Customer Mode" button, full-width, `#FF6B35`
  - Info text below: "Analytics are paused in customer mode. No real bookings will be created." in 12px `#94A3B8`
- **Quick Stats Row** (3 mini metric cards, horizontal scroll on mobile):
  - "Page views: —" (dash for pre-launch)
  - "Bookings: —"
  - "Concierge chats: —"
  - Each: `#F8FAFC` bg, 12px radius, 16px padding, metric in 20px JetBrains Mono 600, label in 11px `#94A3B8`
- **Secondary Actions:**
  - "View Analytics" link (disabled/grayed for pre-launch)
  - "Edit Page" link in `#4F8DFF`

**Style:** Dashboard feel — clean, organized, metric-forward. The Customer Mode card is the centerpiece. Stats are placeholder (dashes) pre-launch but show the layout.

**Platform:** Mobile 375px. Stats row horizontal-scrolls. Main card centered. 16px side padding.

---

## Screen 3.2 — Full Customer Journey Simulation

**Context:** The owner is now IN customer mode, viewing their page exactly as a customer would see it. This is essentially Screen 4.1 (the customer entry page) but with a thin "Customer Mode" banner at the top. The banner should be minimal so the preview feels authentic.

**Components:**

- **Customer Mode Banner** (fixed top, 40px height, `#0F172A` bg):
  - Left: Eye icon + "CUSTOMER MODE" in 10px Inter 700 uppercase, white text, 1.5px tracking
  - Right: "Exit" button (small, white border, 4px radius, 8px 12px padding)
- **Below banner:** Render the full Screen 4.1 (Entry) — hero image, quick info bar, vibe tags, social proof, pricing, CTA. (See `04-customer-experience.md` Screen 4.1 for full component spec)
- **Floating Feedback FAB** (bottom-right, 56px circle):
  - Orange circle (`#FF6B35`) with pencil/notepad icon (white)
  - Subtle shadow: `0 4px 12px rgba(255, 107, 53, 0.3)`
  - Positioned 16px from right edge, 80px from bottom (above sticky CTA)

**Style:** The customer mode banner is dark and thin — just enough to remind the owner this is a preview. Everything below is pixel-perfect customer experience. The feedback FAB floats and is always accessible.

**Platform:** Mobile 375px. Banner is fixed. Page scrolls underneath. FAB is position:fixed.

---

## Screen 3.3 — Inline Feedback Overlay

**Context:** When the owner taps the feedback FAB, a bottom sheet slides up with section-by-section feedback options. Each section of their page can be rated or flagged. This should feel quick and lightweight — tap, flag, move on.

**Components:**

- **Bottom Sheet** (slides up from bottom, white bg, 16px radius top corners, shadow-xl):
  - **Handle bar** at top center (40px wide, 4px height, `#E2E8F0`, 2px radius)
  - **Header:** "Flag sections for review" in 18px H3, 20px bottom margin
  - **Section List** (scrollable within sheet):
    - Each row: Section name (14px 600) + section thumbnail (40x40, 4px radius, `#F8FAFC` bg) + chevron right icon
    - Sections: "Hero Image", "Pricing", "Concierge Sample", "Testimonials", "Call-to-Action", "Photo Gallery", "Trust Block"
    - Tapping a row expands inline or opens a sub-view
  - **Expanded Feedback (per section):**
    - Section name + small screenshot
    - Radio pills (horizontal): "Looks great", "Change copy", "Change image", "Add more info", "Remove"
    - Each pill: `#F1F5F9` bg, 12px `#475569` text, 20px radius. Selected: `#FF6B35` bg, white text
    - Optional textarea: "Tell us more (optional)" — 80px height, 12px radius
    - "Submit Flag" small button (`#FF6B35`, 8px radius)
  - **Concierge Rating** (separate section at bottom of list):
    - "Rate the concierge" label
    - 5 star icons (tappable, `#FF6B35` when filled, `#E2E8F0` when empty)
    - Optional textarea: "What could improve?"

**Style:** Bottom sheet pattern (iOS/Android standard). Clean section list. Radio pills are compact and scannable. Sheet can be swiped down to dismiss.

**Platform:** Mobile 375px. Bottom sheet takes ~70% of viewport. Sections scroll within.

---

## Screen 3.4 — Approval + Edit Requests

**Context:** After exiting customer mode, the owner sees a summary of their feedback and chooses how to proceed — go live immediately, wait for changes, or review again. This is the decision gate before launch.

**Components (top to bottom):**

- **Header:** "Ready to go live?" in 26px H2. "You flagged [N] sections. Here's the plan:" in 14px `#475569`
- **Feedback Summary Card** (white bg, 14px radius, 20px padding):
  - List of flagged items, each with:
    - Section name in 14px 600
    - Feedback type badge (e.g., "Change copy" in orange pill, "Change image" in blue pill)
    - Status: "Pending" in 12px `#D97706`
  - If no flags: Green card with check icon "No issues found! Your page looks great."
  - Timeline note: "Changes take 2-4 hours to process" in 12px `#94A3B8`
- **Approval Options** (3 radio cards, single select):
  - Card 1 (recommended): Radio + "Go live now" title in 14px 600 + "Don't wait for changes — publish immediately" in 13px `#64748B`. If selected: `#FF6B35` border
  - Card 2: Radio + "Wait for changes, then go live" + "We'll process feedback and auto-publish when ready"
  - Card 3: Radio + "I need to review again" + "Keep in draft. I'll test again later"
- **CTA:** "Approve" primary button (full-width). Text updates based on selection: "Go Live Now" / "Approve & Wait" / "Save as Draft"

**Style:** Clean decision layout. Summary card is compact. Radio cards are large and tappable. The selected option and CTA should feel decisive.

**Platform:** Mobile 375px. Cards stack. 16px padding. CTA sticky-bottom.

---

## Screen 3.5 — Shareable Artifact Generation

**Context:** The owner's page is live (or approved). Turnout generates promotional assets they can share — Instagram posts, stories, WhatsApp cards, QR codes. This screen should feel like a gift — "here are your marketing materials, ready to go."

**Components (top to bottom):**

- **Celebration Header:**
  - Rocket icon + "Your page is live!" in 32px H1, `#0F172A`
  - "Here's how to promote it." in 16px `#475569`
- **OG Badge Card** (if qualified, `#FFF3ED` bg, 14px radius, 20px padding):
  - "Turnout OG" badge preview (centered, 120x120px square with star + "Turnout OG" text)
  - "Add this to your Instagram bio or website" in 13px `#64748B`
  - Download buttons row: "PNG" "SVG" "IG Story Size" — each small pill button (secondary style)
- **Promotional Cards (3 stacked):**
  - **Card 1 — Instagram Feed Post:**
    - Preview: 1080x1350 mockup (scaled to fit, showing venue photo + branding overlay)
    - "Instagram Feed Post" label + "1080 × 1350px" in 12px `#94A3B8`
    - Buttons: "Download PNG" primary small + "Post to Instagram" secondary small
  - **Card 2 — Instagram Story:**
    - Preview: 1080x1920 mockup (tall, showing story template)
    - "Instagram Story" label + "1080 × 1920px"
    - Buttons: "Download" + "Send to Stories"
  - **Card 3 — WhatsApp Share Card:**
    - Preview: 540x960 mockup (WA optimized)
    - "WhatsApp Card" label
    - Buttons: "Download" + "Share via WhatsApp" (green `#25D366` button)
- **Page Link Section:**
  - QR code (centered, 160x160px, `#0F172A` dots on white)
  - Short URL: "turnout.so/[venue-slug]" in 16px JetBrains Mono, with copy icon button
  - "Download QR" small button

**Style:** Celebratory and generous. Each promo card shows a real-looking preview. Download buttons are prominent. QR code is clean and scannable.

**Platform:** Mobile 375px. All cards stack. Previews scale proportionally. 16px side padding.

---

## Screen 3.6 — Share Screen

**Context:** The final onboarding screen guides the owner to share their page through specific channels. This is the first step toward getting real customers. The screen should feel actionable and urgent (in a positive way) — "start sharing now."

**Components (top to bottom):**

- **Header:** "Share your page and start getting customers" in 26px H2
- **Share Option Cards (3 large cards, stacked):**
  - **Card 1 — Instagram Stories** (white bg, 14px radius, 20px padding):
    - Left: Instagram icon (gradient) + "Share on Instagram Stories" in 16px 600
    - Right: Chevron icon
    - Subtitle: "Reach your followers instantly" in 13px `#64748B`
    - Full card is tappable
  - **Card 2 — WhatsApp Broadcast** (white bg, same styling):
    - Left: WhatsApp icon (`#25D366`) + "Send via WhatsApp" in 16px 600
    - Subtitle: "Share with your regulars and contacts"
  - **Card 3 — Copy Link** (white bg, same styling):
    - Left: Link icon + "Copy Page Link" in 16px 600
    - Right: Instead of chevron, show "Copy" button (small, `#FF6B35`)
    - Below: URL display "turnout.so/[venue-slug]" in 13px JetBrains Mono `#64748B`
    - QR code mini (80x80) right-aligned
- **Tip Card** (`#F8FAFC` bg, 12px radius, 16px padding):
  - Lightbulb icon + "Tip: Share to your IG Stories, main feed, and WhatsApp broadcast list for maximum reach." in 13px `#475569`
- **CTA:** "Go to Dashboard" secondary button (outline style). This completes onboarding.

**Style:** Large, tappable share cards. Each platform icon uses its brand color. Clean and action-oriented. The tip card adds a coaching touch.

**Platform:** Mobile 375px. Cards stack with 12px gap. 16px side padding.
