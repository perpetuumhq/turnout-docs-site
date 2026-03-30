# Turnout Design System — Stitch Design Tokens

> This file defines the persistent design tokens for Google Stitch. Reference this as context when generating any Turnout screen.

## Brand Identity

- **Product:** Turnout — a venue demand operating system for India's go-out economy
- **Platform:** Mobile-first web app (primary target: 375px width)
- **Personality:** Warm, competent, outcome-first, WhatsApp-native simplicity
- **Voice:** Conversational, uses contractions, no jargon, no passive voice. One emoji per header max.

## Color Tokens

### Primary Brand

| Token           | Hex       | Usage                              |
|-----------------|-----------|-------------------------------------|
| `brand-orange`  | `#FF6B35` | Primary CTAs, accents, brand marks  |
| `brand-orange-hover` | `#E55A28` | CTA hover state               |
| `dark-navy`     | `#0F172A` | Headlines, primary text             |
| `clean-white`   | `#FFFFFF` | Page background (60% of surface)    |
| `pale-sky`      | `#F8FAFC` | Card backgrounds, sections          |

### Orange Scale

| Token | Hex       |
|-------|-----------|
| 50    | `#FFF3ED` |
| 100   | `#FFE4D6` |
| 200   | `#FFC4A3` |
| 300   | `#FF9B6B` |
| 500   | `#FF6B35` |
| 600   | `#E55A28` |
| 700   | `#C44A1C` |
| 900   | `#8F3510` |

### Navy Scale

| Token | Hex       |
|-------|-----------|
| 50    | `#F8FAFC` |
| 100   | `#F1F5F9` |
| 200   | `#E2E8F0` |
| 400   | `#94A3B8` |
| 500   | `#64748B` |
| 600   | `#475569` |
| 800   | `#1E293B` |
| 950   | `#0F172A` |

### Extended / Functional

| Token             | Hex       | Usage                  |
|-------------------|-----------|------------------------|
| `whatsapp-green`  | `#25D366` | WhatsApp CTA buttons   |
| `action-blue`     | `#4F8DFF` | Links, info elements   |
| `ai-teal`         | `#36E4C7` | AI-powered indicators  |
| `premium-purple`  | `#7C3AED` | Premium tier badges    |
| `success-green`   | `#059669` | Success states         |
| `warning-amber`   | `#D97706` | Warning states         |
| `error-red`       | `#DC2626` | Error states           |
| `highlight-pink`  | `#EC4899` | Highlight moments      |

### Color Ratio Rule

60% white · 25% navy · 10% orange · 5% extended

## Typography

| Style       | Font                | Size  | Weight | Line-height | Tracking  |
|-------------|---------------------|-------|--------|-------------|-----------|
| Hero        | Plus Jakarta Sans   | 48px  | 800    | 1.08        | -1px      |
| H1          | Plus Jakarta Sans   | 32px  | 800    | 1.15        | -0.02em   |
| H2          | Plus Jakarta Sans   | 26px  | 700    | 1.15        | -0.01em   |
| H3          | Plus Jakarta Sans   | 18px  | 700    | 1.2         | —         |
| Body Large  | Inter               | 16px  | 400    | 1.7         | —         |
| Body        | Inter               | 14px  | 400    | 1.65        | —         |
| Body Small  | Inter               | 13px  | 400    | —           | —         |
| Caption     | Inter               | 12px  | 500    | —           | 1px (uppercase) |
| Label       | Inter               | 10px  | 700    | —           | 1.5px (uppercase) |
| Data/Mono   | JetBrains Mono      | 20px  | 600    | —           | —         |

## Spacing (4px Base Unit)

| Token | Value | Use Case                |
|-------|-------|-------------------------|
| xs    | 4px   | Tight within components |
| sm    | 8px   | Small gaps, icon spacing |
| md    | 12px  | Standard component padding |
| base  | 16px  | Default padding, margins |
| lg    | 20px  | Card padding            |
| xl    | 24px  | Section padding         |
| 2xl   | 32px  | Large section spacing   |
| 3xl   | 40px  | Major sections          |
| 4xl   | 48px  | Hero sections           |
| 5xl   | 64px  | Page breaks             |

## Border Radius

| Token  | Value    | Usage           |
|--------|----------|-----------------|
| sm     | 4px      | Tight elements  |
| md     | 8px      | Standard, images |
| lg     | 12px     | Cards, inputs   |
| xl     | 16px     | Large cards     |
| pill   | 9999px   | Badges, tags    |
| cta    | 24px     | Sticky CTA bar  |

## Shadows

| Token | Value                            | Usage               |
|-------|----------------------------------|----------------------|
| sm    | 0 1px 2px rgba(0,0,0,0.05)      | Subtle elevation     |
| md    | 0 4px 12px rgba(0,0,0,0.08)     | Card hover, dropdowns |
| lg    | 0 8px 24px rgba(0,0,0,0.1)      | Modals, expanded     |
| xl    | 0 20px 40px rgba(0,0,0,0.15)    | Fullscreen overlays  |

## Grid & Layout

- **Mobile (primary):** 375px width, 16px side padding, 343px content width, 12px card gap
- **Tablet:** 768px, 24px padding, 2-column grid, 24px gap
- **Desktop:** 1100px max-width, 32px padding, 3-column grid, 32px gap

## Component Patterns

### Buttons

- **Primary CTA:** `#FF6B35` bg, white text, 14px/700, 12px radius, 14px 24px padding. Hover: `#E55A28`, scale(1.02)
- **WhatsApp CTA:** `#25D366` bg, white text, full-width on mobile, 24px radius, fixed bottom bar (60px height)
- **Secondary:** White bg, `#0F172A` text, 1px `#E2E8F0` border, 8px radius. Hover: border `#FF6B35`

### Cards

- White bg, 1px `#E2E8F0` border, 12-14px radius, 20px padding. Hover: border `#FF6B35`, shadow-md, translateY(-2px)

### Badges/Tags

- 6px 12px padding, 20px radius (pill), 11px/600 uppercase, 0.5px tracking
- Orange badge: `#FFC4A3` bg / `#8F3510` text
- Green badge: `#D1FAE5` bg / `#065F46` text
- Purple badge: `#E9D5FF` bg / `#581C87` text

### Form Inputs

- 1px `#E2E8F0` border, 12px radius, 14px 12px padding, 14px Inter. Focus: 2px `#FF6B35` border

### Trust Block

- `#F8FAFC` bg, 12px radius, 20px padding. 3-column grid for rating/credential/verification

### Navigation Tabs

- Pill-style tabs: Active = `#FF6B35` bg white text, Inactive = transparent `#94A3B8` text, 20px radius, 12px font

## Touch Targets

- Minimum: 44px x 44px
- Spacing between targets: 8px
- Focus state: 2px orange outline, 2px offset

## Animation

- All transitions: 200-300ms
- Card hover: translateY(-2px) + shadow increase
- CTA hover: darken 10%, scale(1.02)
- Scroll reveal: opacity 0→1, translateY(12px→0), stagger 80ms
- Loading: Orange spinner, 2px stroke, 24px diameter
