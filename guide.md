# Lorebary Laboratory CSS Guide

## Table of Contents

- [LAB-006 — Bookmarks Panel](#lab-006--bookmarks-panel)
- [LAB-009 — Message Bubble Ornament](#lab-009--message-bubble-ornament)
- [LAB-014 — Focus Visibility](#lab-014--focus-visibility)
- [LAB-015 — Portrait Glow](#lab-015--portrait-glow)
- [LAB-015 — Portrait Positioning](#lab-015--portrait-positioning)
- [LAB-016C — Pink Neon Search Icon](#lab-016c--pink-neon-search-icon)
- [LAB-016D — Search Rainbow Button Fill](#lab-016d--search-rainbow-button-fill)
- [LAB-016E — Fullscreen Gradient Outline](#lab-016e--fullscreen-gradient-outline)
- [LAB-016F — Bookmarks Rotating Rainbow Ring](#lab-016f--bookmarks-rotating-rainbow-ring)
- [LAB-016H — Gallery Layered Icon Recoloring](#lab-016h--gallery-layered-icon-recoloring)

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

## Next Batch Suggestions

The next entries to add should likely be:

1. LAB-001 — Menu icon replacement
2. LAB-002 — Header icon replacements
3. LAB-003 — Composer + utility icon styling
4. LAB-007 — Distinct Bookmarks tabs
5. LAB-010 — User vs character message differentiation
6. LAB-011 — Thinking panel styling
7. LAB-012 — Write menu states
8. LAB-013 — Scene notes and template controls

This keeps the guide balanced between image replacements, message styling, and UI effects.