# Lorebary Laboratory CSS Guide

## Table of Contents

- [LAB-001 — Menu Icon Replacement](#lab-001--menu-icon-replacement)
- [LAB-002 — Header Icon Replacements](#lab-002--header-icon-replacements)
- [LAB-003 — Composer + Utility Actions](#lab-003--composer--utility-actions)
- [LAB-004 — Rating Artwork](#lab-004--rating-artwork)
- [LAB-005 — Empty-State Illustration](#lab-005--empty-state-illustration)
- [LAB-006 — Bookmarks Panel](#lab-006--bookmarks-panel)
- [LAB-007 — Distinct Bookmarks Tabs](#lab-007--distinct-bookmarks-tabs)
- [LAB-009 — Message Bubble Ornament](#lab-009--message-bubble-ornament)
- [LAB-010 — Differentiate User Messages](#lab-010--differentiate-user-messages)
- [LAB-011 — Thinking Panel Styling](#lab-011--thinking-panel-styling)
- [LAB-012 — Write Menu States](#lab-012--write-menu-states)
- [LAB-013 — Scene Notes Controls](#lab-013--scene-notes-controls)
- [LAB-014 — Focus Visibility](#lab-014--focus-visibility)
- [LAB-015 — Portrait Glow](#lab-015--portrait-glow)
- [LAB-015 — Portrait Positioning](#lab-015--portrait-positioning)
- [LAB-015 — Expression Toggle](#lab-015--expression-toggle)
- [LAB-015 — Decorative Overlay](#lab-015--decorative-overlay)
- [LAB-015 — Expression Gear](#lab-015--expression-gear)
- [LAB-016C — Pink Neon Search Icon](#lab-016c--pink-neon-search-icon)
- [LAB-016D — Search Rainbow Button Fill](#lab-016d--search-rainbow-button-fill)
- [LAB-016E — Fullscreen Gradient Outline](#lab-016e--fullscreen-gradient-outline)
- [LAB-016F — Bookmarks Rotating Rainbow Ring](#lab-016f--bookmarks-rotating-rainbow-ring)
- [LAB-016G — Search Illustration Recolor Experiment](#lab-016g--search-illustration-recolor-experiment)
- [LAB-016H — Gallery Layered Icon Recoloring](#lab-016h--gallery-layered-icon-recoloring)

---

## LAB-001 — Menu Icon Replacement
Replace the Lab menu icon with a creator-provided asset while keeping the control intact.

```css
img[data-lab="menu"] {
  content: url("/api/images/6ac8974542880c652f051b0e") !important;
  object-fit: contain !important;
}
```

**Customization:**
- `content: url(...)` = swaps the image source
- `object-fit: contain` = keeps the replacement proportional
- Use a local asset later by replacing the URL with your own file path

**Before / After:** Show the default menu icon before and the customized replacement after.

**Device notes:** Desktop: Confirmed. Mobile: Not separately tested; verify if the menu is still visually clear on narrow screens.

---

## LAB-002 — Header Icon Replacements
Swap common header controls like Search, Bookmarks, and HTML mode with custom art while preserving clickability and layout spacing.

```css
[data-lab="header-action"][aria-label="Search this chat"] img {
  content: url("/api/images/6ac897301a947bf5aa43d1c8") !important;
}

[data-lab="header-action"][aria-label="Message bookmarks"] img {
  content: url("/api/images/6ac897231a947bf5aa43cf04") !important;
  object-fit: contain !important;
  filter: none !important;
}

[data-lab="html-mode"] img {
  content: url("/api/images/6ac8a0a61a947bf5aa45143c") !important;
  object-fit: contain !important;
  filter: none !important;
}
```

**Customization:**
- Each selector matches a specific header action by `aria-label`
- Replace the `url(...)` values with your own art
- `filter: none` prevents inherited tint rules from clashing with the custom asset

**Before / After:** Capture the original header row, then show the customized icon set after replacement.

**Device notes:** Desktop: Confirmed. Mobile: Header layouts may compress differently; check visual spacing and icon hit area.

---

## LAB-003 — Composer + Utility Actions
Replace composer and utility icons across the toolbar without changing their function or structure.

```css
[data-lab="send"] img:not([src*="icon_stop"]) {
  content: url("/api/images/6ac8971700c414e8e2a1c37b") !important;
  object-fit: contain !important;
}

[data-lab="write"] img {
  content: url("/api/images/6ac8970875e1eb8796dcfc4f") !important;
  object-fit: contain !important;
}

[data-lab="scroll-down"] img {
  content: url("/api/images/6ac896f900c414e8e2a1bffd") !important;
  object-fit: contain !important;
  transform: none !important;
}

[data-lab="swipe"][aria-label="Previous version"] img {
  content: url("/api/images/6ac896e875e1eb8796dcf891") !important;
  object-fit: contain !important;
  transform: none !important;
  filter: none !important;
}
```

**Customization:**
- Target each action via `data-lab` and `aria-label`
- `transform: none` prevents inherited animation or layout transforms from affecting replacement art
- Update asset URLs to fit your own custom icon bundle

**Before / After:** Show the toolbar in its default state before and the new icon set after.

**Device notes:** Desktop: Confirmed. Mobile: Some toolbar controls may collapse or reposition; verify visible hierarchy and spacing.

---

## LAB-004 — Rating Artwork
Give each rating choice a unique graphic so the user sees clear visual differentiation at a glance.

```css
[data-lab="rating"] button[aria-label="Rate 1 of 5"] img {
  content: url("/api/images/6ac898fd42880c652f055e95") !important;
}

[data-lab="rating"] button[aria-label="Rate 2 of 5"] img {
  content: url("/api/images/6ac8991542880c652f0562cb") !important;
}

[data-lab="rating"] button[aria-label="Rate 3 of 5"] img {
  content: url("/api/images/6ac8992042880c652f05646f") !important;
}

[data-lab="rating"] button[aria-label="Rate 4 of 5"] img {
  content: url("/api/images/6ac8995ad2d7799fdce4e272") !important;
}

[data-lab="rating"] button[aria-label="Rate 5 of 5"] img {
  content: url("/api/images/6ac8996500c414e8e2a2153e") !important;
}
```

**Customization:**
- Each selector targets one specific rating choice
- Use custom icon art for each value instead of a shared generic symbol
- Great for making feedback more playful or more on-brand

**Before / After:** Show the default rating row before and the five unique icon variations after.

**Device notes:** Desktop: Confirmed. Mobile: Keep the row readable and not too visually dense on compact screens.

---

## LAB-005 — Empty-State Illustration
Replace the empty-state illustration with a custom image while preserving the panel size and layout balance.

```css
[data-lab="bookmarks-panel"] img[src*="bary_search.webp"] {
  content: url("/api/images/6ac899a700c414e8e2a21d73") !important;
  width: 112px !important;
  height: 138px !important;
  object-fit: contain !important;
  filter: none !important;
}
```

**Customization:**
- `width` and `height` = keep the illustration from breaking the panel proportions
- `object-fit: contain` = preserves the artwork without cropping distortion
- Replace the uploaded URL with your own local image later

**Before / After:** Capture the standard empty state before and the custom replaced illustration after.

**Device notes:** Desktop: Confirmed. Mobile: Check how the illustration scales in tighter sidebars or stacked layouts.

---

## LAB-006 — Bookmarks Panel
Change the Bookmarks sidebar from the default panel look to a deeper purple gradient with a neon pink accent edge.

```css
[data-lab="bookmarks-panel"] {
  background: linear-gradient(155deg, #3b215b, #151b45) !important;
  border-left: 2px solid #ff77c8 !important;
}
```

**Customization:**
- `background` = panel tone and gradient depth
- `border-left` = accent rail for quick visual separation
- `!important` = keeps the styling from being overridden by app defaults

**Before / After:** Place the original sidebar screenshot in the "before" slot and the recolored version in the "after" slot.

**Device notes:** Desktop: Yes. Mobile: Check overlay width and compact spacing.

---

## LAB-007 — Distinct Bookmarks Tabs
Give the Bookmarks tabs different accents so active states remain visually distinct without changing the layout.

```css
#lab-bookmarks-tab-messages {
  border: 2px solid #ff70b6 !important;
}

#lab-bookmarks-tab-marks {
  border: 2px solid #78d9ff !important;
}
```

**Customization:**
- `border` = uses color to differentiate each tab without rewriting the structure
- `#ff70b6` and `#78d9ff` create a pink/blue split
- Keep the tab hierarchy and semantics intact while changing the visual treatment

**Before / After:** Place the original bookmarks tab strip before and the accented version after.

**Device notes:** Desktop: Source-theme implementation. Mobile: Check tab widths and tap targets in compact layouts.

---

## LAB-009 — Message Bubble Ornament
Add a decorative ornament above the message text so bubbles feel more stylized without changing the message content area.

```css
[data-lab="bubble"] {
  position: relative !important;
  padding-top: 48px !important;
}

[data-lab="bubble"]::before {
  content: "✦ · ✧ · ✦" !important;
  position: absolute !important;
  top: 12px;
  left: 18px;
  right: 18px;
  text-align: center;
  color: #ff8bd8;
  pointer-events: none;
}
```

**Customization:**
- `padding-top` = creates space for the top ornament
- `content` = edit the text ornament to another symbol pattern
- `color` = adjust the ornament to match your theme palette

**Before / After:** Insert the original bubble screenshot before and the ornamented version after.

**Device notes:** Desktop: Yes. Mobile: Verify long-message wrapping and spacing.

---

## LAB-010 — Differentiate User Messages
Style user bubbles differently from character bubbles so conversation turns read clearly and feel more readable in chat threads.

```css
[data-lab="bubble"] {
  background: #232047 !important;
}

[data-lab-role="user"] [data-lab="bubble"] {
  background: #4b245c !important;
  border: 1px solid #ff85c4 !important;
}
```

**Customization:**
- `background` = defines the default character bubble palette
- `user` override = creates a stronger, more distinct reply bubble
- `border` = helps separate role-based messaging without forcing a layout change

**Before / After:** Show the standard message thread before and the color-differentiated user messages after.

**Device notes:** Desktop: Source-theme implementation. Mobile: Verify contrast and readability in dark/light mode transitions.

---

## LAB-011 — Thinking Panel Styling
Restyle the thinking panel and toggle so the chat feedback area feels more like an intentional UI surface instead of a blank default block.

```css
[data-lab="thoughts"] {
  background: #201d3e !important;
  border: 1px solid #a18bff !important;
}

[data-lab="thoughts-toggle"] {
  background: #352954 !important;
  color: #fff !important;
}
```

**Customization:**
- `background` = darkens the panel while keeping a structured UI feel
- `border` = adds a subtle purple boundary for separation
- `color` = keeps toggle text readable on darker backgrounds

**Before / After:** Place the plain thinking panel before and the styled panel after.

**Device notes:** Desktop: Source-theme implementation. Mobile: Confirm the toggle still remains obvious and touch-friendly on compact screens.

---

## LAB-012 — Write Menu States
Style the write menu and its options so selected states, hover states, and panel structure are easier to distinguish.

```css
[data-lab="write-menu"] {
  background: #201c3e !important;
  border: 1px solid #ff83ce !important;
}

[data-lab="write-option"]:hover {
  background: #46305d !important;
}

[data-lab="write-option"][aria-checked="true"] {
  box-shadow: inset 3px 0 #ffcf70 !important;
}
```

**Customization:**
- `background` = gives the menu a richer visual shell
- `hover` = differentiates selection and interaction states
- `box-shadow` = highlights the active option without changing layout

**Before / After:** Show the plain write panel before and the styled, stateful menu after.

**Device notes:** Desktop: Source-theme implementation. Mobile: Verify menu spacing and tap targets when space is constrained.

---

## LAB-013 — Scene Notes Controls
Add contrast and emphasis to the Scene Notes panel and selected template controls so important actions stand out more clearly.

```css
#lab-scene-notes {
  background: #282449 !important;
  border: 1px solid #8ce9e2 !important;
}

[aria-label="Scene note templates"] button[aria-pressed="true"] {
  border: 2px solid #ffcf79 !important;
}
```

**Customization:**
- `background` = improves contrast in the note panel
- `border` = visually separates the panel from surrounding chat UI
- `aria-pressed` selector = makes the selected template state obvious

**Before / After:** Use a default notes panel screenshot before and the accentuated version after.

**Device notes:** Desktop: Source-theme implementation. Mobile: Confirm notes remain legible and buttons still easy to tap.

---

## LAB-014 — Focus Visibility
Make keyboard focus states obvious while leaving the rest of the interface intact.

```css
[data-lab="header-action"]:focus-visible,
[data-lab="write"]:focus-visible,
[data-lab="send"]:focus-visible {
  outline: 3px solid #ffdf76 !important;
  outline-offset: 3px !important;
}
```

**Customization:**
- `outline` = thickness and color of the visible focus ring
- `outline-offset` = pushes the ring away from the element edge
- `:focus-visible` = only targets keyboard users, not mouse clicks

**Before / After:** Place a screenshot of the default focus state before and the highlighted focus ring after.

**Device notes:** Desktop: Yes. Mobile: Focus styling is relevant for keyboard and assistive tech, but touch-first states should still be checked.

---

## LAB-015 — Portrait Glow
Add a layered neon glow around the character portrait so the expression has more presence without changing the actual image asset.

```css
[data-lab="expression"] img {
  filter: drop-shadow(0 0 8px #ff69c9)
          drop-shadow(0 0 14px #70dfff)
          drop-shadow(0 0 20px #a78bfa) !important;
}
```

**Customization:**
- `drop-shadow` = adds color glows one layer at a time
- `0 0 8px` style = controls glow radius and intensity
- Color stack = change hues to match your character palette

**Before / After:** Keep the original portrait before and the glowing variant after.

**Device notes:** Desktop: Confirmed. Mobile: Not separately tested; verify performance and layout.

---

## LAB-015 — Portrait Positioning
Shift the expression portrait to the right side of the layout so it sits as a floating side accent rather than a centered element.

```css
[data-lab="expression"] {
  left: auto !important;
  right: 0 !important;
  bottom: 0 !important;
}
```

**Customization:**
- `right` = pushes the portrait toward the right edge
- `bottom` = controls vertical offset
- `left: auto` = keeps the element from clinging to the default side

**Before / After:** Show the original portrait alignment before and the right-side positioning after.

**Device notes:** Desktop: Confirmed. Mobile: Check for clipping on narrower layouts.

---

## LAB-015 — Expression Toggle
Style the expression toggle to feel like a dedicated button with a clear pressed state and glow.

```css
[data-lab="expression-toggle"] {
  background: #27214c !important;
  border: 2px solid #ff84d5 !important;
  box-shadow: 0 0 8px #ff84d566 !important;
}

[data-lab="expression-toggle"][aria-pressed="true"] {
  background: #623c7d !important;
}
```

**Customization:**
- `border` = adds a pleasing accent edge around the toggle
- `box-shadow` = gives the button a soft glow without overpowering the UI
- `aria-pressed` = visually differentiates the active state clearly

**Before / After:** Show the default expression control before and the glow/highlighted version after.

**Device notes:** Desktop: Confirmed. Mobile: Ensure the control still reads as a button when compressed.

---

## LAB-015 — Decorative Overlay
Add a decorative background asset behind the expression frame to create a more elaborate portrait presentation without changing the main portrait itself.

```css
[data-lab="expression"]::after {
  content: "" !important;
  position: absolute !important;
  inset: 0 !important;
  background:
    url("/api/images/6ac8999c42880c652f0572b8")
    center bottom / contain no-repeat !important;
  pointer-events: none !important;
}
```

**Customization:**
- `background` = overlays a decorative asset behind the face art
- `center bottom` = keeps the image anchored to the lower frame
- `pointer-events: none` = ensures the overlay does not interfere with interaction

**Before / After:** Show the portrait without the overlay before and the decorated final treatment after.

**Device notes:** Desktop: Confirmed. Mobile: Keep decorative layers subtle so they do not compete with the portrait.

---

## LAB-015 — Expression Gear
Add a gear action beside the expression controls so the expression management UI reads as a more intentional toolset.

```css
[data-lab="expression-manage"] img {
  content: url("/api/images/6ac8997ed2d7799fdce4e72a") !important;
  object-fit: contain !important;
}
```

**Customization:**
- `content: url(...)` = swaps the gear icon asset for the custom version
- `object-fit: contain` = preserves proportions and avoids distortion
- Keep the gear action visually familiar so it remains obvious as a settings control

**Before / After:** Use the default expression tool cluster before and the gear-enhanced version after.

**Device notes:** Desktop: Confirmed. Mobile: Verify the gear control remains easy to hit and visually clear in tighter panels.

---

## LAB-016C — Pink Neon Search Icon
Apply a neon pink glow to the Search icon while preserving the image transparency and artwork details.

```css
[data-lab="header-action"][aria-label="Search this chat"] img {
  filter: drop-shadow(0 0 3px #ff79ca)
          drop-shadow(0 0 7px #ff79ca) !important;
}
```

**Customization:**
- `drop-shadow` = creates a clean glow without heavy tinting
- `#ff79ca` = neon pink accent
- `0 0 7px` = stronger outer glow for emphasis

**Before / After:** Use the plain icon before and the glowing pink version after.

**Device notes:** Desktop: Confirmed. Mobile: Only appears on desktop-specific header states where the icon is present.

---

## LAB-016D — Search Rainbow Button Fill
Turn the Search action into a rainbow gradient background while keeping it a single cohesive button control.

```css
[data-lab="header-action"][aria-label="Search this chat"] {
  background: linear-gradient(135deg, #ff7a9c, #ffdc79, #8ee8b3, #7fdfff, #b69cff, #ff8bd3) !important;
  border: 1px solid #ffe2f3 !important;
}
```

**Customization:**
- `linear-gradient` = sets the rainbow order and intensity
- `border` = outlines the button softly without overpowering the color fill
- `!important` = prevents theme overrides

**Before / After:** Put the original Search button before and the rainbow-filled action after.

**Device notes:** Desktop: Confirmed. Mobile: Layout can be checked but the effect is most effective in desktop header layouts.

---

## LAB-016E — Fullscreen Gradient Outline
Create a modern gradient border around the Fullscreen control with a soft neon glow.

```css
[data-lab="header-action"][aria-label*="fullscreen" i] {
  border: 2px solid transparent !important;
  border-radius: 50% !important;
  background: linear-gradient(#242b3c, #242b3c) padding-box,
              linear-gradient(135deg, #ff89ca, #76e7ff) border-box !important;
}
```

**Customization:**
- `border` = creates a clear outline without changing the icon art
- `background` = uses a two-layer gradient to keep the fill and border separate
- `border-radius: 50%` = standard circular control shape

**Before / After:** Insert the default fullscreen control before and the neon gradient version after.

**Device notes:** Desktop: Confirmed. Mobile: Control may appear only where the fullscreen action is visible.

---

## LAB-016F — Bookmarks Rotating Rainbow Ring
Add a rotating rainbow ring around the Bookmarks button without replacing the actual icon artwork.

```css
[data-lab="header-action"][aria-label="Message bookmarks"] {
  position: relative !important;
  isolation: isolate !important;
  overflow: visible !important;
  background: #242b3c !important;
  border: 2px solid transparent !important;
  border-radius: 50% !important;
}

[data-lab="header-action"][aria-label="Message bookmarks"]::before {
  content: "" !important;
  position: absolute !important;
  inset: -2px !important;
  border-radius: 50% !important;
  pointer-events: none !important;
  z-index: -1 !important;
  background: conic-gradient(#ff7a9c, #ffdc79, #8ee8b3, #7fdfff, #b69cff, #ff8bd3, #ff7a9c) !important;
  -webkit-mask: radial-gradient(farthest-side, transparent calc(100% - 3px), #000 calc(100% - 2px)) !important;
  mask: radial-gradient(farthest-side, transparent calc(100% - 3px), #000 calc(100% - 2px)) !important;
  animation: lab-bookmark-ring-spin 3s linear infinite !important;
}

@keyframes lab-bookmark-ring-spin {
  to {
    transform: rotate(360deg);
  }
}
```

**Customization:**
- `conic-gradient` = defines the ring's rainbow cycle
- `mask` = keeps the ring open in the center while preserving button visibility
- `animation` = adds motion without changing the icon itself

**Before / After:** Place the standard Bookmarks button before and the animated rotating ring after.

**Device notes:** Desktop: Confirmed; clickable. Mobile: Not separately tested; confirm touch hit area and spacing.

---

## LAB-016G — Search Illustration Recolor Experiment
Optional recolor experiment for the Search empty-state illustration. Keep this clearly labeled as a stylistic variant rather than a baseline recommendation.

```css
[data-lab="bookmarks-panel"] img[src*="bary_search.webp"] {
  filter: invert(1) drop-shadow(0 0 3px #ff79ca) drop-shadow(0 0 7px #ff79ca) !important;
}
```

**Customization:**
- `invert(1)` = flips the artwork toward a high-contrast look
- `drop-shadow` = adds a pink glow to the illustration
- Best for experimentation, not as the default styling baseline

**Before / After:** Show the default Search illustration before and the recolored version after.

**Device notes:** Desktop: Confirmed as optional experiment. Mobile: Not a default recommendation; validate visual clarity in smaller layouts before publishing.

---

## LAB-016H — Gallery Layered Icon Recoloring
Layer a color-adjusted filter onto the Gallery icon so the icon stays recognizable while the parent button cycles rainbow tones.

```css
[data-lab="header-action"][aria-label="Scene gallery"] img {
  filter: hue-rotate(145deg) saturate(1.8) contrast(1.2) !important;
}
```

**Customization:**
- `hue-rotate` = shifts the icon into a warmer or cooler palette
- `saturate` = increases the icon intensity
- `contrast` = makes the icon stand out against the button background

**Before / After:** Use the default gallery icon before and the layered recolored version after.

**Device notes:** Desktop: Confirmed. Mobile: The effect is best preserved where the full gallery button exists.

---

## Notes for Future Snippets

- All examples in this starter set are intentionally independent and copy-paste friendly.
- Use placeholders in markdown where the final image or asset will be inserted later.
- Keep the label structure consistent: title / one-sentence effect / CSS block / customization / before-after / device notes.
- When a snippet is desktop-only, mobile-only, or desktop-confirmed but not separately mobile-tested, note it directly in the documentation.
- Public facing tutorials should use placeholder asset URLs where personal uploads are not yet finalized.

---

## Final Batch Status

The guide now covers the main Lorebary Laboratory styling categories:

- icon replacements
- panel redesigns
- message differentiation
- focus visibility
- expression styling
- contextual effects and glow treatments

This is now in a strong state for a final pass: tighten wording, remove internal-only notes, and prepare a cleaner public README/public tutorial version later.
