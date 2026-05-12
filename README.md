# 🤝 SilverHelpers

> **A civic tech tool connecting seniors who need help with verified local volunteers — built for a hackathon on the theme: *"Build a civic tech tool with the biggest positive real-world impact if it existed tomorrow."***

---

## The Problem

- **54 million Americans** are over 65. **1 in 3 live alone.**
- Many can't afford services like TaskRabbit, and don't trust strangers from the internet.
- Simple physical tasks — mowing a lawn, moving a chair, clearing a garage — become genuine barriers to dignity and independence as people age.
- The gap isn't technology. It's **trust infrastructure**.

SilverHelpers closes that gap.

---

## What It Does

SilverHelpers is a **neighborhood-scale, trust-first task platform** with two sides:

### 🙋 Senior View (I Need Help)
Seniors see large, high-contrast cards for common tasks:
- 🌿 **Mow Lawn**
- 🛋️ **Move Furniture**
- 📦 **Clear Garage**

One tap sends a help request. A progress animation confirms the match, and a verified volunteer's name + arrival time appears — no app account, no payment, no friction.

### 💪 Volunteer View (I Want to Help)
Verified volunteers see a live feed of open neighbor requests with:
- Distance from their location
- Senior's first name, age, and a personal note
- One-tap task acceptance with instant confirmation to the senior

### 🗺️ Map View
An interactive neighborhood map shows:
- All open requests as **pulsing pins** (color-coded by task type)
- The volunteer's current location marked as **"You"**
- Dashed distance lines between volunteer and each request
- Tap any pin to pull up the full request and accept directly from the map

---

## Why It Wins on Impact

| Metric | Reality |
|---|---|
| Americans 65+ living alone | 14.7 million |
| Annual unclaimed social services | ~$60B+ |
| Trust as the #1 barrier to help-seeking in seniors | Documented in AARP 2023 research |
| Cost to deploy this tool | ~$0 infrastructure for an MVP |

Unlike TaskRabbit (optimized for speed + price), SilverHelpers is optimized for **vulnerability and dignity**. The trust layer — ID verification, background checks, community endorsements, star ratings — is the product.

---

## Trust & Safety Model

Every volunteer on SilverHelpers must pass:
1. **Government ID verification**
2. **Background check** (criminal + sex offender registry)
3. **Community endorsement** (vouched by 2 existing members or local organization)
4. **Ongoing reputation** (star ratings visible to seniors before accepting)

This is shown permanently in the sticky footer of every screen — because safety is not a feature, it's the foundation.

---

## Prototype

The prototype is a single, self-contained HTML file — no build tools, no npm, no backend.

```
build/
└── index.html    ← Full clickable prototype (open in any browser)
```

**Built with:**
- [Tailwind CSS Play CDN](https://tailwindcss.com/docs/installation/play-cdn) — utility styling
- [Google Fonts — Inter](https://fonts.google.com/specimen/Inter) — accessible, friendly typography
- Vanilla JavaScript — zero dependencies
- Inline SVG — hand-crafted neighborhood map

**To run:** Open `build/index.html` in any browser. No server needed.

---

## Design System

| Token | Value | Usage |
|---|---|---|
| Cream | `#FEF9F0` | App background |
| Deep Teal | `#0F766E` | Header, verified badges, accept buttons |
| Coral Orange | `#F97316` | Primary CTA, Mow Lawn accent |
| Golden Yellow | `#F59E0B` | Move Furniture accent, road markings |
| Text Dark | `#1C1917` | Headings |
| Text Muted | `#78716C` | Body copy |

The header uses a **textured diagonal gradient** (repeating-linear-gradient overlay) to give warmth without requiring images.

---

## Screens

| Screen | Description |
|---|---|
| **Senior — Task Selection** | 3 large cards, large text, single-tap request flow |
| **Senior — Request Sent** | Progress bar → matched volunteer confirmation with arrival time |
| **Map — Neighborhood** | SVG bird's-eye neighborhood with pulsing request pins and volunteer marker |
| **Map — Pin Detail Sheet** | Slide-up bottom sheet with senior quote, distance, and Accept button |
| **Volunteer — Request List** | Cards sorted by distance with senior quotes and one-tap accept |
| **Volunteer — Profile** | Verified badge, star rating, task count, show rate stats |

---

## Hackathon Context

**Theme:** Build a civic tech tool with the biggest positive real-world impact if it existed tomorrow.

**Why SilverHelpers:**
- The problem is real, widespread, and emotionally undeniable
- The solution is technically simple — the hard part (trust) is a design and ops problem, not a software problem
- It works at the neighborhood scale before it needs to scale globally
- It doesn't require government buy-in, VC funding, or a new behavior — neighbors helping neighbors is ancient; we're just making it trusted and findable

---

## Future Roadmap

- [ ] SMS-first interface for seniors without smartphones
- [ ] Integration with local senior centers and churches as trust anchors
- [ ] Volunteer hour tracking + community recognition program
- [ ] Family notification system (ping a senior's adult child when help is matched)
- [ ] Multi-language support (Spanish, Mandarin, Portuguese)

---

## Authors

Built with ❤️ for a civic tech hackathon — May 2026.
