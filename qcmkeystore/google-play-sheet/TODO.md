# TODO — Google Play Promotional Screenshots · Qcm Locker

## Purpose

Transform the 5 raw ADB screenshots in `promotional/raw/` into polished
**1 080 × 1 920 px** Google Play promotional cards.

Each card = one raw screenshot placed inside a phone mockup frame,
set on a branded background, with a short promotional tagline overlaid
at the bottom of the card.

Finished cards go in `promotional/ready/` as `1.jpg` … `5.jpg`.

---

## Global Specs

| Property | Value |
|---|---|
| Canvas size | 1 080 × 1 920 px |
| Output format | JPEG, quality ≥ 95 |
| Background style | Vertical linear gradient — `#2D5A3D` (top) → `#4A7C59` (bottom) |
| Primary accent | Gold `#C8922A` |
| Text color | White `#FFFFFF` |
| Headline font | Bold / ExtraBold sans-serif (Nunito, Poppins, or system equivalent) |
| Sub-copy font | Regular sans-serif, same family as headline |
| Brand footer | `Qcm Locker` · small · white · centered · bottom 60 px |

### Composition template

```
┌──────────────────────────────┐  y = 0
│                              │
│   [gradient background]      │  top padding ≈ 80 px
│                              │
│   ┌────────────────────┐     │
│   │  phone frame       │     │  phone mockup centered
│   │  + screenshot      │     │  width ≈ 780 px
│   │  inside            │     │  top of frame ≈ y 100
│   └────────────────────┘     │  bottom of frame ≈ y 1 380
│                              │
│   [HEADLINE — bold white]    │  y ≈ 1 420, size 72–80 px
│   [sub-copy — white 80 % ]   │  y ≈ 1 520, size 38–44 px
│                              │
│   [Qcm Locker footer]        │  y ≈ 1 860, size 28 px
└──────────────────────────────┘  y = 1 920
```

### Phone frame
Use a clean flat Android frame (no brand markings).
Mask the status bar (top 24 px of screenshot) and the gesture nav bar
(bottom 60 px of screenshot) before placing the screenshot inside the frame.
The raw screenshots are **1 080 × 2 340 px**; scale them to fit the frame height
(≈ 1 280 px inner height) while keeping aspect ratio, then center-crop horizontally.

### Text rules
- Headline: center-aligned, max 2 lines.
- Key word(s) listed in the per-image section must be rendered in gold `#C8922A`,
  all other words in white.
- Add a soft drop shadow (rgba 0,0,0,0.4 · blur 8 px · offset 0,3) to all text.
- Sub-copy: center-aligned, white at 80 % opacity, line height 1.4.

---

## Image 1 — `raw/1.jpg` → `ready/1.jpg`

### Screen analysis
**Onboarding slide 1.** Illustration of a quiz sheet (with graduation-cap badge) flanked
by a green security shield and a golden padlock. In-app text: *"Lock your quizzes —
Create a lock and apply it to your .qcm files before sharing them."*
First promise of the app: the author is in full control before a file leaves the device.

### Promotional tagline

| | Text |
|---|---|
| **Headline (EN)** | Your quiz. Your **rules**. |
| Sub-copy (EN) | Lock any .qcm file before sharing — no one gets in without your say. |
| **Headline (FR)** | Votre quiz. Vos **règles**. |
| Sub-copy (FR) | Verrouillez vos fichiers avant de les partager — vous décidez qui peut les ouvrir. |

Gold word: **rules** (EN) / **règles** (FR).

### Crop hint
Center the screenshot vertically; the illustration sits in the upper half of the screen,
so cropping from the bottom is safe.

---

## Image 2 — `raw/2.jpg` → `ready/2.jpg`

### Screen analysis
**Onboarding slide 2.** A central dark vault/safe with a shield emblem radiates arrows
outward to 5 user avatars (students, professionals), each receiving a PassCode key.
In-app text: *"Distribute access codes — Generate PassCodes to only allow intended
people to open your quizzes."*
Visual metaphor: the author holds the vault; learners only receive individual keys.

### Promotional tagline

| | Text |
|---|---|
| **Headline (EN)** | One code. One student. **Full control**. |
| Sub-copy (EN) | Generate PassCodes and share them — only the right people unlock your content. |
| **Headline (FR)** | Un code. Un apprenant. **Zéro compromis**. |
| Sub-copy (FR) | Générez des PassCodes et distribuez-les — seules les bonnes personnes accèdent à vos quiz. |

Gold words: **Full control** (EN) / **Zéro compromis** (FR).

### Crop hint
The radial illustration is centered; crop evenly top and bottom.

---

## Image 3 — `raw/3.jpg` → `ready/3.jpg`

### Screen analysis
**Onboarding slide 3 / Google sign-in.** A profile avatar sits above a tablet showing a
quiz grid; a cloud sync icon and a gold padlock orbit the avatar. The button at the bottom
reads *"Continue with Google"*. In-app text: *"Connect your space — Sign in with your
Google account to find and manage your locks."*
Message: locks are stored in the cloud, tied to the author's Google identity —
accessible from anywhere, always in sync.

### Promotional tagline

| | Text |
|---|---|
| **Headline (EN)** | Your locks. **Wherever you are**. |
| Sub-copy (EN) | Sign in with Google — manage all your protected quizzes from one place. |
| **Headline (FR)** | Vos loquets. **Où que vous soyez**. |
| Sub-copy (FR) | Connectez-vous avec Google — gérez tous vos quiz protégés depuis un seul endroit. |

Gold words: **Wherever you are** (EN) / **Où que vous soyez** (FR).

### Crop hint
Keep the "Continue with Google" button visible inside the phone frame —
it reinforces the Google sign-in story. Crop from the top if needed.

---

## Image 4 — `raw/4.jpg` → `ready/4.jpg`

### Screen analysis
**Home screen — populated state.** Green toolbar titled *"My locks"*. Three lock cards:
- Cybersecurity Certification - Level 2
- Medical Entrance Exam 2026
- SAT Practice Test - Math

Each shows a padlock icon and creation date. A "+" FAB sits bottom-right.
The three diverse subjects (security cert, medical entrance, standardized test)
demonstrate that Qcm Locker is for any serious quiz author, any domain.

### Promotional tagline

| | Text |
|---|---|
| **Headline (EN)** | All your quizzes. **All locked in**. |
| Sub-copy (EN) | One dashboard for every protected quiz — from one subject to a full curriculum. |
| **Headline (FR)** | Tous vos quiz. **Tous sécurisés**. |
| Sub-copy (FR) | Un seul tableau de bord pour chaque quiz protégé — d'une matière à tout un programme. |

Gold words: **All locked in** (EN) / **Tous sécurisés** (FR).

### Crop hint
The three lock cards all fit within the top 60 % of the screenshot.
Crop from the bottom (empty list area) to keep all cards fully visible in the frame.

---

## Image 5 — `raw/5.jpg` → `ready/5.jpg`

### Screen analysis
**Access codes list screen.** Toolbar reads *"Access codes"* with a share icon.
Four active PassCodes listed: `1MCQRRZM`, `5MgNNKIM`, `6NA11XND`, `DMwRRRBI`.
Each row shows status **Active · 0/1** and a **Copy** button.
This is the author's distribution center: codes are generated, individually copyable,
and exportable as CSV via the share icon. Three-step action loop: generate → copy → share.

### Promotional tagline

| | Text |
|---|---|
| **Headline (EN)** | **Generate.** Copy. Share. |
| Sub-copy (EN) | Instant PassCodes, ready to hand to your learners in seconds. |
| **Headline (FR)** | **Générez.** Copiez. Partagez. |
| Sub-copy (FR) | Des PassCodes instantanés, prêts à distribuer à vos apprenants en quelques secondes. |

Gold word: **Generate.** (EN) / **Générez.** (FR) — first verb only, the others in white.

### Crop hint
The 4 PassCode rows all fit in the top 50 % of the screenshot.
Crop from the bottom; keep the share icon in the toolbar visible.

---

## Phone Frame

Use the workspace canvas as the phone mockup — do NOT generate a thick or 3D frame:

- **Frame overlay:** `Ai-prompts/resources/promotional/mobile_canevas.png`
- **GIMP source:** `Ai-prompts/resources/promotional/mobile_canevas.xcf`

The canvas is a flat, minimal outline. Composite the screenshot behind the frame layer.
Reference style: `Ai-prompts/screenshots/web-site/en/home.png` (QcmMaker approved look).

The existing `ready/en/1.jpg` … `5.jpg` were generated with a thick bezel frame and
**must be regenerated** using `mobile_canevas.png`. Force re-generation of all 5 images
even if `ready/` files are newer than `raw/`.

## Generation Checklist

- [ ] `ready/en/1.jpg` — "Your quiz. Your **rules**." — 1 080 × 1 920 px
- [ ] `ready/en/2.jpg` — "One code. One student. **Full control**." — 1 080 × 1 920 px
- [ ] `ready/en/3.jpg` — "Your locks. **Wherever you are**." — 1 080 × 1 920 px
- [ ] `ready/en/4.jpg` — "All your quizzes. **All locked in**." — 1 080 × 1 920 px
- [ ] `ready/en/5.jpg` — "**Generate.** Copy. Share." — 1 080 × 1 920 px
- [ ] Phone frame uses `mobile_canevas.png` (thin outline) on all cards
- [ ] Status bar and nav bar masked on every card
- [ ] Gradient background consistent across all 5 cards
- [ ] Gold accent applied to the correct word(s) per card
- [ ] Drop shadow applied to all text
- [ ] Brand footer "Qcm Locker" present, centered, bottom 60 px
- [ ] Output JPEG quality ≥ 95
