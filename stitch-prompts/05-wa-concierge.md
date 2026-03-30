# Journey 5: WhatsApp Concierge UI — Stitch Prompts

> 8 flows covering WhatsApp conversation interfaces and message templates.
> Note: These are WhatsApp-style chat UIs. Generate as mobile screens showing chat interfaces.

---

## Flow 5.1 — Entry Messages (Chat Screen)

**Context:** Design a WhatsApp-style chat screen showing the first message from Turnout's AI concierge to a customer. The customer has just tapped "Book via WhatsApp" from a venue landing page. The concierge should feel human, warm, and helpful — not like a bot. Show the phone's WhatsApp interface realistically.

**Components:**

- **WhatsApp Chrome:** Status bar (time, battery, signal), WhatsApp green header bar (`#075E54`), venue name + "Turnout Concierge" subtitle + verified badge, back arrow, call/video/menu icons
- **Chat Area** (WhatsApp wallpaper bg, light tan `#ECE5DD`):
  - **System Message:** "Messages are end-to-end encrypted" center pill (small, gray)
  - **Concierge Message Bubble** (white bg `#FFFFFF`, rounded, tail on left):
    - "Hi! 👋 I see you're interested in Padel Point. Great choice!"
    - New line: "Quick question — is this your first time playing?"
    - Timestamp: "6:42 PM" small right-aligned, `#94A3B8`
  - **Quick Reply Buttons** (below bubble, WhatsApp-style):
    - "Yes, first time!" (bordered pill, `#075E54` text)
    - "No, I've played before" (bordered pill)
    - "Just browsing" (bordered pill)
- **Input Bar** (bottom): Text field "Type a message" + emoji icon + camera icon + mic icon

**Style:** Pixel-perfect WhatsApp UI. Use WhatsApp's actual color scheme for chrome (`#075E54` header, `#ECE5DD` wallpaper, white/green bubbles). Concierge messages are white (incoming), customer messages will be green `#DCF8C6`.

**Platform:** Mobile 375px. Full WhatsApp interface mockup.

---

## Flow 5.1 — Persona Variants (6 Entry Messages)

Generate these as a **multi-screen set** — same WhatsApp chrome, different first messages:

| Persona | First Message |
|---------|--------------|
| **Beginner** | "Hi! 👋 I see you're interested in Padel Point. Great choice! Quick question — is this your first time playing?" |
| **Regular** | "Hey! Glad to see you back 😊 Looking to book Friday? I remember you like Court 2 in the evening." |
| **Group Organizer** | "Hey! 🏸 Planning something fun for your crew? I can help you book a court and sort out payment for everyone." |
| **Solo** | "Hi! 👋 Want to play some padel solo? I can help you find a slot where you'll meet other players or play at your own pace." |
| **Corporate** | "Hi! 👋 Planning a team event at Padel Point? I can help arrange bulk booking, invoicing, and any custom setup you need." |
| **Price-Sensitive** | "Hey! 👋 Interested in Padel Point? Let me tell you about our off-peak deals and what actually fits your budget." |

---

## Flow 5.2 — Price Hesitation Chat

**Context:** A multi-message WhatsApp conversation where the concierge addresses price concerns with a tiered offer ladder. Show a realistic back-and-forth conversation.

**Components (WhatsApp chat, 5-6 messages):**

1. **Concierge (white bubble):** "I totally get it — let me show you options:" then bullet list: "• First-time offer: Rs 199 (instead of 599)" / "• No commitment — try once and see if you love it" / "Sound better?"
2. **Customer (green bubble `#DCF8C6`):** "Yeah, Rs 199 works"
3. **Concierge:** "Perfect! 🎉 When would you like to try?" then "(Friday, Saturday, or next week?)"
4. **Customer:** "Friday evening"
5. **Concierge:** "Friday 6 PM is available! Rs 199 for your first session." then "Rackets provided. Just bring water + comfortable shoes." then "Ready to lock it in?"
6. **Customer:** "Yes!"
7. **Concierge:** "🎉 Booking confirmed!" then structured message card:

- **Inline Confirmation Card** (within chat, slightly different bg `#F0F4F8`, rounded):
  - "📅 Friday, March 28 at 6 PM"
  - "🏸 Court 2, Padel Point"
  - "👤 1 person"
  - "💰 Rs 199 (first-timer special)"
  - "Ref: TN20260328XYZ"

**Style:** Realistic WhatsApp conversation flow. Timestamp on each message. Read receipts (blue ticks) on customer messages. Typing indicator between messages.

**Platform:** Mobile 375px WhatsApp mockup.

---

## Flow 5.4 — Group Coordination Chat

**Context:** WhatsApp conversation where the concierge helps a group organizer coordinate a booking for 4 friends, including a shareable invite card.

**Components (WhatsApp chat, 6+ messages):**

1. **Concierge:** "So you're thinking Friday with 4 people? I can make this super easy:" then numbered list: "1. You pick the time" / "2. I send invite links to your friends" / "3. They confirm + pay their share" / "4. You're all set!"
2. **Customer:** "Friday 6 PM works"
3. **Concierge:** "Great! Here's an invite card to send your group:" then a **shareable card** (special message format):

- **Invite Card** (in-chat card, `#F8FAFC` bg, rounded 12px, orange top accent bar 3px `#FF6B35`):
  - "🏸 Shreya invited you to Padel Point"
  - "Friday 6 PM · 4 people"
  - "Rs 510/person (group discount applied)"
  - "Tap to confirm + pay → [link]"
  - "Powered by Turnout" small footer text

4. **Customer:** "Sent! Everyone's in"
5. **Concierge:** Final confirmation card (structured):
  - "🎉 Booking locked!"
  - "📅 Friday, March 28 at 6 PM"
  - "👥 4 people confirmed"
  - "💰 Rs 510/person (Rs 2,040 total)"
  - "📍 Court 2, Padel Point"
  - "Rackets provided. Bring water."
  - "See you Friday! 🎾"

**Style:** WhatsApp realistic. The invite card should look like a special rich message (similar to WhatsApp's payment/event cards). Orange accent on the invite card ties to Turnout brand.

**Platform:** Mobile 375px.

---

## Flow 5.5 — Slot Selection Chat

**Context:** The concierge simplifies slot selection by presenting time options as a readable text list instead of a confusing grid.

**Components (WhatsApp chat):**

1. **Concierge:** "Picking a time can be confusing! Let me make it easy. What day are you thinking?"
2. **Customer:** "This Saturday"
3. **Concierge:** Formatted slot message:

```
Saturday, March 29:

Morning:
• 7-8 AM (Rs 399, 4 spots) ✓
• 8-9 AM (Rs 399, FULL) ✗

Afternoon:
• 2-3 PM (Rs 499, 2 spots) ✓
• 3-4 PM (Rs 499, FULL) ✗

Evening:
• 5-6 PM (Rs 599, 3 spots) ✓
• 6-7 PM (Rs 599, 1 spot left) ⚡

Which time works?
```

4. **Customer:** "5-6 PM"
5. **Concierge:** "Perfect! 5-6 PM Saturday. Rs 599. Ready to confirm?"

**Style:** Clean text formatting in WhatsApp. Use emoji indicators for status (✓ available, ✗ full, ⚡ almost full). Monospaced feel for the slot grid.

**Platform:** Mobile 375px WhatsApp.

---

## Flow 5.6 — Safety/Trust Chat

**Context:** Customer asks about safety. The concierge responds with specific, honest details — not deflection.

**Components (WhatsApp chat):**

1. **Customer:** "Is it safe to come alone? Especially as a woman?"
2. **Concierge:** Detailed safety response: "Totally fair question. Here's the real answer:" then bold sections:
  - "**Safety:** Padel Point is in a well-lit, busy area in Indiranagar. Lots of women come solo and in groups. Zero incidents reported (we track this)."
  - "**Vibe:** Mostly relaxed, inclusive crowd. Zero tolerance for disrespect. Hosts are trained to intervene."
  - "**Logistics:** Parking available. Security on-site till 10 PM. Groups typically leave together."
  - "Specific concerns?"
3. **Customer:** "That's reassuring. OK I'll try it"
4. **Concierge:** "You'll love it! 😊 Want to book a slot?"

**Style:** WhatsApp. The safety response uses bold formatting (WhatsApp supports *bold*). Tone is honest and specific, not corporate.

**Platform:** Mobile 375px.

---

## Flow 5.8 — Booking Closure Chat

**Context:** Final booking confirmation flow in WhatsApp. The concierge confirms all details, gets explicit yes, and sends confirmation with next steps.

**Components (WhatsApp chat):**

1. **Concierge:** Confirmation recap:
  - "Let me confirm everything:"
  - "📅 Friday, March 28 at 6 PM"
  - "🏸 Court 2, Padel Point, Indiranagar"
  - "👥 4 people"
  - "💰 Rs 510/person (Rs 2,040 total)"
  - "✓ No hidden charges"
  - "Sound right?"
2. **Customer:** "Yes, let's do it"
3. **Concierge:** "🎉 Booking confirmed! Ref: TN20260328ABC"
  - Then next-steps message:
  - "**What happens next:**"
  - "• Check email for confirmation + directions"
  - "• 24h before: reminder"
  - "• 4h before: final check-in reminder"
  - "• Bring: Water bottle, towel (rackets provided)"
  - "• Arrive 10 min early"
4. **Concierge:** "Have fun with your crew! 🎾" then "(Need to reschedule? Reply CHANGE. Need help? Reply HELP.)"
5. **Quick Reply Buttons:** "CHANGE", "HELP", "Thanks!"

**Style:** Clean WhatsApp closure. Confirmation feels celebratory. Next steps are structured and scannable. CHANGE/HELP keywords are clear exit options.

**Platform:** Mobile 375px.
