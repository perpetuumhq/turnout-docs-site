# Turnout Beta — Stitch Prompt Library

> Production-ready prompts for [Google Stitch](https://stitch.withgoogle.com) to generate high-fidelity UI screens for Turnout.

## How to Use

1. **Open [stitch.withgoogle.com](https://stitch.withgoogle.com)**
2. **Paste the contents of `design.md`** as your first prompt to establish the design system context
3. **Generate screens** by pasting prompts from the journey files below, one screen at a time
4. **Iterate:** Use Stitch's edit mode to refine individual components after initial generation
5. **Export:** Use Stitch's code export (HTML/CSS or Tailwind) for development handoff

## Prompt Structure

Every prompt follows the **4-Layer Stitch Framework:**

| Layer        | Purpose                                      |
|--------------|----------------------------------------------|
| **Context**  | Product description, target user, screen goal |
| **Components** | Detailed UI elements, layout hierarchy      |
| **Style**    | Hex colors, fonts, radius, spacing tokens    |
| **Platform** | Mobile (375px) or Web, responsive behavior   |

## File Index

| File | Journey | Screens |
|------|---------|---------|
| `design.md` | — | Design tokens (paste first) |
| `01-owner-prelaunch.md` | Journey 1 | Screens 1.1–1.5 (Owner Pre-Launch) |
| `02-owner-onboarding.md` | Journey 2 | Screens 2.1–2.6 (Owner Onboarding) |
| `03-owner-testing.md` | Journey 3 | Screens 3.1–3.6 (Owner Testing & Approval) |
| `04-customer-experience.md` | Journey 4 | Screens 4.1–4.5 (Customer Page Experience) |
| `05-wa-concierge.md` | Journey 5 | Flows 5.1–5.8 (WhatsApp Concierge UI) |
| `06-post-booking.md` | Journey 6 | Screens 6.1–6.7 (Post-Booking + Owner Dashboard) |

## Tips for Best Results

- Always paste `design.md` first in a new Stitch session
- Generate one screen at a time for maximum fidelity
- Use hex codes exactly as specified (do not say "orange" — say `#FF6B35`)
- After generating, use Stitch's edit mode for refinements
- For persona variants, generate the base screen first, then use edit mode to swap content
