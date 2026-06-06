# HK Weather Website — Design Brainstorm

## Approach A — "Atmospheric Depth" (Glassmorphism + Dark Sky)
<response>
<text>
**Design Movement:** Contemporary Glassmorphism meets Meteorological Dashboard

**Core Principles:**
1. Dark, deep-sky gradient background (midnight navy to deep indigo) evoking the Hong Kong night skyline
2. Frosted glass cards with backdrop-blur for each forecast day — information floats above the atmosphere
3. Layered depth: background gradient → blurred glass panels → crisp typography on top
4. Accent colors shift subtly based on weather conditions (warm amber for sunny, cool cyan for rain)

**Color Philosophy:**
- Base: deep navy `#0a0f2e` → indigo `#1a1f5e`
- Glass: `rgba(255,255,255,0.08)` with `backdrop-filter: blur(16px)`
- Accent: electric cyan `#00d4ff` for temperature, amber `#ffa726` for sunny, steel blue `#4fc3f7` for rain
- Text: crisp white with subtle opacity hierarchy

**Layout Paradigm:**
- Full-bleed gradient hero with current conditions prominently displayed at top-left
- Horizontal scrollable strip of 7 day cards below
- Asymmetric hero: current weather occupies 60% width, general situation text on right

**Signature Elements:**
1. Animated particle/rain/cloud SVG overlay in the hero background
2. Temperature gradient bar showing min–max range per day
3. Subtle glow effect on the active/today card

**Interaction Philosophy:** Hover reveals additional detail (humidity, wind) with smooth fade-in

**Animation:** Cards stagger-entrance from bottom (40ms delay each), temperature bars animate width on load

**Typography System:** `Syne` (display, bold) + `DM Sans` (body) — geometric authority with warmth
</text>
<probability>0.08</probability>
</response>

---

## Approach B — "Ink & Mist" (Editorial Brutalism + Monochrome)
<response>
<text>
**Design Movement:** Editorial Brutalism — newspaper grid meets weather data visualization

**Core Principles:**
1. High-contrast monochrome base with a single vivid accent (HK red `#D42B2B`)
2. Heavy typographic hierarchy — oversized date numbers dominate each card
3. Raw, structured grid with deliberate misalignment for visual tension
4. Data-forward: every pixel serves the weather information

**Color Philosophy:**
- Background: off-white `#F5F2ED` (newsprint warmth)
- Ink: near-black `#1A1A1A`
- Accent: HK Observatory red `#D42B2B` for warnings and highlights
- Muted: warm gray `#8A8580` for secondary info

**Layout Paradigm:**
- Asymmetric 7-column grid where today's forecast is a large feature block (spanning 2 columns)
- Remaining 6 days in single columns to the right
- Thick horizontal rule separates header from forecast grid

**Signature Elements:**
1. Oversized day-of-week typography (e.g., "MON" at 80px) as card background watermark
2. Bold temperature displayed as a large numeral, unit as superscript
3. Red dot indicator for weather warnings

**Interaction Philosophy:** Click expands a day card to full-width detail view with smooth layout animation

**Animation:** Entrance via clip-path wipe (left to right), staggered 60ms per card

**Typography System:** `Bebas Neue` (display numerals) + `IBM Plex Mono` (data labels) + `Spectral` (descriptions)
</text>
<probability>0.07</probability>
</response>

---

## Approach C — "Coastal Luminance" (Soft Modernism + Warm Sky Palette) ✅ SELECTED
<response>
<text>
**Design Movement:** Soft Modernism — inspired by Hong Kong's coastal light and Victoria Harbour haze

**Core Principles:**
1. Warm sky gradient background (dawn peach → sky blue → horizon gold) that shifts based on time of day
2. Clean, airy card layout with generous whitespace — each day breathes
3. Subtle depth via soft shadows and very light frosted overlays (not heavy glassmorphism)
4. Data visualization integrated naturally: temperature range shown as a colored pill bar

**Color Philosophy:**
- Background: warm sky gradient `#FFF5E6` → `#E8F4FD` → `#FEF9F0`
- Primary card: pure white with `box-shadow: 0 4px 24px rgba(0,0,0,0.06)`
- Accent: sky blue `#2196F3` for temperature/rain, warm amber `#FF9800` for sunny conditions
- Text: deep slate `#1E293B` for headings, `#64748B` for secondary

**Layout Paradigm:**
- Tall hero section with current weather on the left and a large HKO weather icon on the right
- Below: horizontal row of 7 compact day-cards with equal width
- Sticky header with HKO branding and last-updated timestamp

**Signature Elements:**
1. Smooth animated sky gradient background that subtly shifts hues
2. Temperature range bar (min–max) as a colored gradient pill under each day's temp
3. Weather icon from HKO's official icon set (pic{N}.png)

**Interaction Philosophy:** Hover on day card elevates it with shadow + slight scale-up, revealing wind/humidity tooltip

**Animation:** Hero fades in (300ms), cards stagger-enter from bottom (50ms delay each, translateY 20px → 0)

**Typography System:** `Nunito` (rounded, friendly, great for weather) + `Roboto Mono` (temperature numerals)
</text>
<probability>0.09</probability>
</response>
