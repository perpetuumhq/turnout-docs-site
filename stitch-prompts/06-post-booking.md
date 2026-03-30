# Journey 6: Post-Booking + Owner Dashboard — Stitch Prompts

> 7 screens covering confirmation, reminders, check-in, rebooking, owner summaries, and the edit dashboard.

---

## Screen 6.1 — Booking Confirmation Email

**Context:** Design the transactional booking confirmation email that customers receive immediately after booking. It should look professional, mobile-optimized, and include all practical details. Think of it as a digital ticket + itinerary. The email renders in mobile mail apps primarily.

**Components (email layout, top to bottom):**

- **Email Header** (`#0F172A` bg, white text, 32px padding):
  - Turnout logo (small, `#FF6B35` text) left
  - "✓ Booking Confirmed" in 20px Plus Jakarta Sans 700, white, centered
- **Confirmation Banner** (`#059669` bg, white text, 24px padding, 12px radius):
  - Check circle icon + "You're all set for Padel Point!" in 18px 700
  - "Friday, March 28 at 6 PM" in 14px 400
- **Details Table** (white bg, 20px padding):
  - Row format — label left (13px `#64748B`), value right (14px 600 `#0F172A`):
    - "Date:" — "Friday, March 28, 2026"
    - "Time:" — "6:00 PM — 7:00 PM"
    - "Venue:" — "Padel Point, Indiranagar"
    - "Party size:" — "4 people"
    - "Booking ref:" — "TN20260328ABC123" (in JetBrains Mono)
    - "Total paid:" — "Rs 2,040 (Rs 510/person)"
  - Each row separated by 1px `#F1F5F9` divider
- **What to Bring Section** (`#F8FAFC` bg, 16px padding, 8px radius):
  - "What to bring:" in 14px 600
  - Checklist: "✓ Water bottle", "✓ Towel", "✓ Sports shoes", "Rackets provided by venue"
- **Venue Location Card:**
  - Static map placeholder (full-width, 160px height, 8px radius)
  - Address: "Padel Point, 3rd Cross, Indiranagar, Bangalore 560038" in 13px
  - "Get Directions" button (secondary style, map pin icon)
  - Phone: "Call venue: +91 98xxx xxxxx" (clickable)
- **Action Buttons Row** (3 buttons, evenly spaced):
  - "Add to Calendar" (outline button, calendar icon)
  - "Share on WhatsApp" (`#25D366` button, white text)
  - "Get Directions" (outline button, map icon)
- **Cancellation Policy:** "Free cancellation until 12h before your visit." in 12px `#64748B`
- **Email Footer** (`#F8FAFC` bg, 20px padding):
  - "Need to reschedule? Reply CHANGE. Questions? Reply HELP." in 13px `#475569`
  - "Sent by [Venue Name] via Turnout" in 11px `#94A3B8`

**Style:** Clean transactional email. Professional but warm. Use the orange sparingly (logo, occasional accent). Green for success/confirmation. Mobile-optimized (single column, large touch targets for buttons).

**Platform:** Email, 600px max-width (responsive). Single column. Large buttons (44px+ height). 20px side padding.

---

## Screen 6.2 — Reminder Messages (24h + 4h Before)

**Context:** Design two WhatsApp reminder messages: one sent 24 hours before the visit and one 4 hours before. They should be brief, practical, and category-aware.

### 6.2.1 — 24-Hour Reminder (WhatsApp)

**Components (WhatsApp message):**

- **Concierge Bubble:**
  - "Hey [Name]! Reminder: Padel Point tomorrow at 6 PM 🏸"
  - ""
  - "Quick prep:"
  - "• Wear comfortable sports shoes"
  - "• Bring water + towel"
  - "• Rackets provided"
  - ""
  - "📍 Directions: [link]"
  - ""
  - "Need to reschedule? Reply CHANGE"
- **Quick Reply Buttons:** "Thanks!", "CHANGE", "Get Directions"

### 6.2.2 — 4-Hour Reminder (WhatsApp)

**Components (WhatsApp message):**

- **Concierge Bubble:**
  - "Almost time! 🎾 Padel Point in 4 hours (6 PM)"
  - "See you there! Arrive 10 min early."
  - "📍 Tap for directions: [link]"
  - ""
  - "Running late? Reply LATE"
- **Quick Reply Buttons:** "On my way!", "LATE", "Directions"

**Style:** Brief, friendly, practical. Category-specific emoji (🏸 for padel). Action-oriented.

**Platform:** Mobile 375px WhatsApp mockup.

---

## Screen 6.3 — Check-in at Venue

**Context:** Design the venue check-in screen shown on the customer's phone when they arrive. They show a QR code to staff, or staff enters their booking ref manually. This is a simple, functional screen.

**Components:**

- **Header:** Turnout logo + "Check In" title
- **QR Code Display** (centered):
  - Large QR code (240x240px) on white bg with 24px padding, 14px radius border, subtle shadow
  - QR encodes booking ref "TN20260328ABC123"
  - Ref number displayed below: "TN20260328ABC123" in 16px JetBrains Mono 600
  - "Show this to staff" in 14px `#64748B`
- **Booking Summary** (below QR, compact):
  - Venue: "Padel Point" in 16px 600
  - "Friday, March 28 · 6 PM · 4 people"
  - "Court 2" in 14px `#64748B`
- **Alternative:** "Staff can also look up: TN20260328ABC" in 12px `#94A3B8`
- **Brightness Hint:** Sun icon + "Turn up screen brightness for easier scanning" in 11px `#94A3B8`
- **Post-Check-in State** (after scan):
  - QR area replaced with large green circle check (80px)
  - "Checked in! ✓" in 26px H2 `#059669`
  - "Enjoy your session!" in 16px `#475569`
  - "Court 2 · Starts in 8 minutes" in 14px `#64748B`

**Style:** Clean, functional. QR code is the hero element. Post-check-in state is celebratory green.

**Platform:** Mobile 375px. QR centered. Brightness at max hint useful for QR scanning.

---

## Screen 6.4 — Post-Visit Rebook Message

**Context:** WhatsApp message sent 4 hours after the customer's session, encouraging rebooking and pack upsell.

### 6.4.1 — Regular Persona Rebook

**Components (WhatsApp message):**

- **Concierge Bubble:**
  - "How was Padel Point? 🎾 Hope you had a blast!"
  - ""
  - "Most people who come once come back. Want to lock in next Friday at the same time?"
  - ""
  - "(Same crew, same spot!)"
- **Action Buttons (WhatsApp list):**
  - "Book Next Friday" (primary action)
  - "Show Me Packs" (secondary)
  - "Not now" (dismiss)
- **If "Show Me Packs" tapped:**
  - "Great choice! Our 10-visit pack:"
  - "• Rs 4,490 (Rs 449/visit — save 25%)"
  - "• Never worry about booking out"
  - "• Valid 3 months"
  - "Want to try it?"

### 6.4.2 — Beginner Persona Rebook

**Components (WhatsApp message):**

- **Concierge Bubble:**
  - "Hope that was fun! 🎾"
  - "Lot of beginners come back because it clicks on the 2nd try."
  - ""
  - "Want to try again next week? (No pressure — just an option!)"
- **Action Button:** "Book Again"

**Style:** Warm, celebratory. Not pushy. Pack upsell is secondary to simple rebooking. Beginner variant is extra low-pressure.

**Platform:** Mobile 375px WhatsApp.

---

## Screen 6.5 — Owner Weekly Summary (WhatsApp)

**Context:** Weekly WhatsApp message sent to venue owners every Monday morning with key metrics and one actionable insight. It should feel like a smart briefing, not a boring report.

### 6.5.1 — Metrics Summary

**Components (WhatsApp message):**

- **Concierge Bubble (formatted):**
  - "Hey [Owner]! Here's your week at Padel Point 📊"
  - ""
  - "**Bookings:** 24 total | +15% vs last week 📈"
  - "**Top Time:** Friday 6-7 PM (8 bookings)"
  - "**Top Source:** Instagram (45% of bookings)"
  - "**Revenue:** Rs 12,400 | +20% vs last week 🎉"
  - ""
  - "**Key Insight:** First-timers had 67% rebook rate (up from 54%). Your beginner experience is clicking!"
  - ""
  - "Want full analytics? Tap below"
- **Action Buttons:** "View Dashboard", "Got it, thanks"

### 6.5.2 — Action Items (sent 1h later)

**Components (WhatsApp message):**

- **Concierge Bubble:**
  - "**Quick wins this week:**"
  - ""
  - "1️⃣ **Content gap:** Missing photos of lounge area. Adding 3 photos could lift CTR by ~8%."
  - ""
  - "2️⃣ **Off-peak opportunity:** Wed-Thu evenings have 40% less demand. Try a 'Weekday special: 20% off' offer?"
  - ""
  - "3️⃣ **Testimonials:** 6 customers rated 5⭐ this week. Want to add quotes to your page?"
  - ""
  - "Let me know if you want help with any of these!"
- **Action Buttons:** "Upload Photos", "Enable Offer", "Collect Reviews"

**Style:** Metrics use bold + emoji for scannability. Action items are numbered and specific. Celebratory tone when growth positive.

**Platform:** Mobile 375px WhatsApp.

---

## Screen 6.6 — Owner Content Gap Request

**Context:** WhatsApp message requesting specific missing photos from the owner with estimated ROI.

**Components (WhatsApp message):**

- **Concierge Bubble:**
  - "Your page is strong, but 3 photos of the lounge area would help customers see the full vibe 📸"
  - ""
  - "**Missing:** Lounge seating + action shot of people playing + close-up of drinks/menu"
  - ""
  - "**Why:** Customers often ask 'What's the seating like?' — seeing it reduces booking anxiety."
  - ""
  - "**Estimated lift:** +8% CTR, +5% conversion (~12 more bookings/month)"
  - ""
  - "Send 3-5 photos (daytime + evening work best)"
- **Action Buttons:** "Upload Photos", "Send Photo Checklist", "Not now"

**Style:** Specific, data-driven, not generic. Estimated lift quantified. Clear ask (3-5 specific photos).

**Platform:** Mobile 375px WhatsApp.

---

## Screen 6.7 — Owner Page Edit Dashboard

**Context:** Design the owner's page editing dashboard — a split-view interface where they see a live phone preview on the left and editable fields on the right. On mobile, these stack (preview on top, form below, or toggle between views).

**Components:**

- **Top Bar:** Turnout logo left, "Edit Page" title center, "Preview" / "Edit" toggle pills right (mobile only)
- **Mobile View (375px — stacked):**
  - **Toggle Tabs:** "Preview" and "Edit" as two pills at top. Active: `#FF6B35` bg white text. Inactive: `#F1F5F9` bg `#475569` text
  - **Preview Mode:** Full-width phone mockup showing the venue's customer-facing page. Scrollable. Real-time updates.
  - **Edit Mode:** Form fields, stacked:
    - "Hero Image" — Current image thumbnail (120px height) + "Change" button + "Upload New" button
    - "Tagline" — Text input (full-width, 12px radius) with current tagline pre-filled
    - "Vibe Tags" — Chip/pill selector. Current tags shown as pills with ✕ delete. "+ Add tag" input
    - "Pricing" — Base price input field. Off-peak toggle + price. Group discount toggle + %
    - "Hours" — Open time picker + Close time picker
    - "Concierge Tone" — Radio: "Friendly", "Professional", "Energetic", "Calm"
    - "Testimonials" — List of current testimonials with edit/delete. "+ Add testimonial"
  - Each field: label (13px Inter 600), input (12px radius, `#E2E8F0` border, 14px padding)
- **Desktop View (1100px — side by side):**
  - Left 40%: Phone mockup preview (fixed, scrollable)
  - Right 60%: Edit form (scrollable)
  - Changes in right panel update left preview in real-time
- **Action Bar** (sticky bottom):
  - "Save Draft" secondary button
  - "Preview on Phone" secondary button (sends preview link to owner's phone)
  - "Publish Changes" primary button (`#FF6B35`)
- **Version Indicator:** "v1.2 · Last published 3 days ago" in 11px `#94A3B8` in top bar

**Style:** Dashboard aesthetic. Clean form layout. Preview is the visual anchor. Edit fields are well-organized. Publish button is the most prominent action. No visual clutter.

**Platform:** Mobile 375px (toggle between preview/edit). Desktop 1100px (split view). 16px padding on mobile, 32px on desktop.
