# LoreBary Laboratory CSS — Contribution Guide

## Contents

- [Getting Started](#getting-started)
  - [Combining Examples Safely](#combining-examples-safely)
  - [How to Import CSS Images in Lorebary](#how-to-import-css-images-in-lorebary)
- [Visual Expressions](#visual-expressions)
  - [Custom Visual Expression Icons](#custom-visual-expression-icons)
  - [Glowing Expression Portraits](#glowing-expression-portraits)
  - [Move Expression Portraits to the Right](#move-expression-portraits-to-the-right)
  - [Floating Expression Portraits](#floating-expression-portraits)
  - [Expression Toggle Button Colors](#expression-toggle-button-colors)
- [Chat Bubbles](#chat-bubbles)
  - [Custom Message Bubble Backgrounds](#custom-message-bubble-backgrounds)
  - [Different User and Character Message Bubbles](#different-user-and-character-message-bubbles)
  - [Bubble Tail Effects and Removal](#bubble-tail-effects-and-removal)
  - [Bubble Transparency Without Fading Text](#bubble-transparency-without-fading-text)
  - [Decorative Message Bubble Ornaments](#decorative-message-bubble-ornaments)
  - [Message Bubble Hover Glow](#message-bubble-hover-glow)
- [Message Text and Formatting](#message-text-and-formatting)
  - [Message Text, Bold, and Italic](#message-text-bold-and-italic)
  - [Dialogue, Dividers, and Headings](#dialogue-dividers-and-headings)
  - [Message List Items](#message-list-items)
- [Message Footer and Ratings](#message-footer-and-ratings)
  - [Message Footer and Timestamp Styling](#message-footer-and-timestamp-styling)
  - [Custom Rating Icons](#custom-rating-icons)
- [Thinking Panel](#thinking-panel)
  - [Thinking Panel Background and Text](#thinking-panel-background-and-text)
  - [Thinking Panel Hover Effects](#thinking-panel-hover-effects)
- [Header and Footer](#header-and-footer)
  - [Custom Header Button Icons](#custom-header-button-icons)
  - [Custom Navigation Icons](#custom-navigation-icons)
  - [Custom Footer Button Icons](#custom-footer-button-icons)
  - [Story Goals Footer Button](#story-goals-footer-button)
  - [Icon Glow — Search Example](#icon-glow-search-example)
  - [Rainbow Button Background — Search Example](#rainbow-button-background-search-example)
  - [Icon Hover Enlargement — Gallery Example](#icon-hover-enlargement-gallery-example)
  - [Animated Rainbow Button — Gallery Example](#animated-rainbow-button-gallery-example)
  - [Multicolor Icon Glow — Bookmarks Example](#multicolor-icon-glow-bookmarks-example)
  - [Rotating Rainbow Button Border — Bookmarks Example](#rotating-rainbow-button-border-bookmarks-example)
  - [Solid Button Border — Voice Call Example](#solid-button-border-voice-call-example)
  - [Gradient Button Border — Fullscreen Example](#gradient-button-border-fullscreen-example)
  - [Pulsing Button Glow — Fullscreen Example](#pulsing-button-glow-fullscreen-example)
  - [Bobbing Icon Animation — Statistics Example](#bobbing-icon-animation-statistics-example)
  - [Button Hover Glow — Statistics Example](#button-hover-glow-statistics-example)
  - [Shared Button Hover Brightness — Header Examples](#shared-button-hover-brightness-header-examples)
  - [Button Keyboard Focus Outlines — Header Examples](#button-keyboard-focus-outlines-header-examples)
  - [Rainbow Icon Recoloring — Gallery Example](#rainbow-icon-recoloring-gallery-example)
  - [Add Character Button](#add-character-button)
- [Time Skip](#time-skip)
  - [Time Skip Message](#time-skip-message)
  - [Time Skip Edit and Delete Buttons](#time-skip-edit-and-delete-buttons)
- [Message Actions and Input Controls](#message-actions-and-input-controls)
  - [Individual Message Action Colors and Hover](#individual-message-action-colors-and-hover)
  - [Custom Menu Button Icon](#custom-menu-button-icon)
  - [Custom Input Button Icons](#custom-input-button-icons)
  - [Custom Draft Version Controls](#custom-draft-version-controls)
  - [Custom Message Action Icons](#custom-message-action-icons)
  - [Calls and Fast Forward](#calls-and-fast-forward)
  - [Call Notifications](#call-notifications)
  - [Disconnected Call Indicator](#disconnected-call-indicator)
  - [Call Entry Options](#call-entry-options)
  - [Fast Forward / Speed Up](#fast-forward--speed-up)
- [Message Decorations and Indicators](#message-decorations-and-indicators)
  - [Bookmarked Message Indicator](#bookmarked-message-indicator)
  - [Backup Model Icon](#backup-model-icon)
  - [Managing Tinting, Filters, and Icon Replacements](#managing-tinting-filters-and-icon-replacements)
- [Write for Me](#write-for-me)
  - [Write Menu Heading Colors](#write-menu-heading-colors)
  - [Write Menu Actions and Help Text](#write-menu-actions-and-help-text)
  - [Write Menu Selected, Unselected, and Keyboard-Focus States](#write-menu-selected-unselected-and-keyboard-focus-states)
  - [Custom Write Menu Action Icons](#custom-write-menu-action-icons)
- [Search and Bookmarks](#search-and-bookmarks)
  - [Search & Bookmarks Panel Background](#search-bookmarks-panel-background)
  - [Search & Bookmarks Header Styling](#search-bookmarks-header-styling)
  - [Search & Bookmarks Title and Description](#search-bookmarks-title-and-description)
  - [Search & Bookmarks Header Icon Glow](#search-bookmarks-header-icon-glow)
  - [Custom Search & Bookmarks Header Icons](#custom-search-bookmarks-header-icons)
  - [Custom Search Bar Colors](#custom-search-bar-colors)
  - [Search Bar Focus Effect](#search-bar-focus-effect)
  - [Bookmarks Tab Bar Background](#bookmarks-tab-bar-background)
  - [Bookmarks Tab Colors](#bookmarks-tab-colors)
  - [Selected Bookmarks Tab Styling](#selected-bookmarks-tab-styling)
  - [Bookmarks Tab Hover and Keyboard Focus](#bookmarks-tab-hover-and-keyboard-focus)
  - [Bookmarks Tab Counters](#bookmarks-tab-counters)
  - [Bookmarks Empty-State Text](#bookmarks-empty-state-text)
  - [Custom Search Empty-State Illustration](#custom-search-empty-state-illustration)
  - [Search & Bookmarks Close Button](#search-bookmarks-close-button)
  - [Search & Bookmarks Footer Styling](#search-bookmarks-footer-styling)
  - [Custom Copy and Download Icons](#custom-copy-and-download-icons)
  - [Custom Search & Bookmarks Background Images](#custom-search-bookmarks-background-images)
  - [Custom Bookmarks Tab Icons](#custom-bookmarks-tab-icons)
- [Scene Notes](#scene-notes)
  - [Custom Scene Notes Window](#custom-scene-notes-window)
  - [Scene Notes Title and Close Button](#scene-notes-title-and-close-button)
  - [Scene Notes Template Colors](#scene-notes-template-colors)
  - [Scene Notes Selected and Hover Effects](#scene-notes-selected-and-hover-effects)
  - [Scene Notes Text Box Colors and Focus](#scene-notes-text-box-colors-and-focus)
  - [Scene Notes Additional Buttons](#scene-notes-additional-buttons)
  - [Scene Notes Keyboard Focus](#scene-notes-keyboard-focus)
  - [Custom Scene Notes Template Icons](#custom-scene-notes-template-icons)
- [Multiplayer](#multiplayer)
  - [Multiplayer Island Background and Controls](#multiplayer-island-background-and-controls)
  - [Multiplayer Icon Recoloring](#multiplayer-icon-recoloring)
  - [Custom Multiplayer Icon](#custom-multiplayer-icon)
  - [Multiplayer Participant Avatars](#multiplayer-participant-avatars)
  - [Multiplayer Author Names](#multiplayer-author-names)
  - [Multiplayer Session Notification Cards](#multiplayer-session-notification-cards)
  - [Multiplayer Notification Delete Button](#multiplayer-notification-delete-button)
  - [Multiplayer Message Reaction Button](#multiplayer-message-reaction-button)
  - [Multiplayer Reaction Counters](#multiplayer-reaction-counters)
  - [Floating Player-Chat Toggle](#floating-player-chat-toggle)
  - [Player-Chat Window Background and Header](#player-chat-window-background-and-header)
  - [Player-Chat Text and Buttons](#player-chat-text-and-buttons)
  - [Player-Chat Message Bubbles](#player-chat-message-bubbles)
  - [Player-Chat Composer](#player-chat-composer)
  - [Player-Chat Images GIFs and Stickers](#player-chat-images-gifs-and-stickers)  
- [Universes](#universes)
  - [Universe Sidebar Background and Header](#universe-sidebar-background-and-header)
  - [Universe Sidebar Titles and Text](#universe-sidebar-titles-and-text)
  - [Universe Selection Radio Buttons](#universe-selection-radio-buttons)
  - [Universe Cards and Content Panels](#universe-cards-and-content-panels)
  - [Universe Input Fields and Dropdowns](#universe-input-fields-and-dropdowns)
  - [Universe Buttons and Icons](#universe-buttons-and-icons)
  - [Universe Header Badge](#universe-header-badge)
  - [Universe Pills and Tags](#universe-pills-and-tags)
  - [Universe Additional Input Controls](#universe-additional-input-controls)
  - [Universe Sidebar Scrollbar](#universe-sidebar-scrollbar)
  - [Universe Clock](#universe-clock)
  - [Universe Minimap](#universe-minimap)
  - [Universe Recall Button](#universe-recall-button)  
- [Reply Choices](#reply-choices)
  - [Reply Choices Container](#reply-choices-container)
  - [Reply Choices Gradient Border](#reply-choices-gradient-border)
  - [Reply Choices Question](#reply-choices-question)
  - [Individual Reply Choices](#individual-reply-choices)
  - [Alternating Reply Choice Colors](#alternating-reply-choice-colors)
  - [Rainbow Reply Choice Borders](#rainbow-reply-choice-borders)
  - [Reply Choice Icons](#reply-choice-icons)
  - [Rainbow Reply Choice Icons and Pointers](#rainbow-reply-choice-icons-and-pointers)
  - [Reply Choice Dialogue Text](#reply-choice-dialogue-text)
  - [Remove Dialogue Background Decorations](#remove-dialogue-background-decorations)
  - [Reply Choices Action Buttons](#reply-choices-action-buttons)
  - [Regenerate and Dismiss Suggestions](#regenerate-and-dismiss-suggestions)
- [Pinned Scenes](#pinned-scenes)
  - [Pinned Scene Card](#pinned-scene-card)
  - [Pinned Scene Decorative Tape](#pinned-scene-decorative-tape)
  - [Custom Pinned Scene Tape](#custom-pinned-scene-tape)
  - [Pinned Scene Unpin Button](#pinned-scene-unpin-button)


---

### How to Import CSS Images in Lorebary

Learn how to upload artwork to Lorebary and use its image URL in your Laboratory CSS. ![Uploading artwork and using its URL in Laboratory CSS](./images/css-upload-custom-image.png)

1. Upload your image using Lorebary's image upload feature. Copy the image's Lorebary-hosted URL; an uploaded image may have a path resembling `/api/images/IMAGE_ID`.
2. Open your Laboratory CSS editor and find the selector for the element you want to customize.
3. Paste the URL into `content: url(...)` when replacing an existing `<img>` element, or into `background-image: url(...)` when decorating an element's background.
4. Save your CSS and refresh or revisit the affected Laboratory screen to check the result.

**Choosing an image source:** You can use either a LoreBary-uploaded `/api/images/...` path or a Base64 image data URL. For Base64, replace `XXX` with the complete `data:webp;base64,...` value (or the corresponding data URL for your image format). See [Converting Images to Base64](https://github.com/Caddel001/LoreBary-Theme-Snippets/blob/main/LoreBary%20CSS%20Quick%20Guide.md#converting-images-to-base64). No externally hosted image URL is required or supported here.

**Optional: Store an image source in a CSS variable**

```css
/* Set the image source once: uploaded path or Base64 data URL */
.lab-theme-scope {
  --menu-icon-image: url("XXX");
}

/* Reuse that image source on the matching icon */
img[data-lab="menu"] {
  content: var(--menu-icon-image) !important;
  object-fit: contain !important;
}
```

Replace `XXX` with `/api/images/YOUR_IMAGE_ID` or your complete Base64 data URL. The variable is optional: the direct `content: url(...)` method below works too. For other icons, choose a descriptive variable name and update the selector.

**Example: Replace an icon**

```css
img[data-lab="menu"] {
  content: url("/api/images/YOUR_IMAGE_ID") !important;
  object-fit: contain !important;
}
```

**Example: Add a background image**

```css
[data-lab="bookmarks-panel"] {
  background-image: url("/api/images/YOUR_IMAGE_ID") !important;
  background-position: center !important;
  background-size: cover !important;
}
```

**Customization:**
- `YOUR_IMAGE_ID` = replace this placeholder with the path of your uploaded image.
- `content: url(...)` = substitutes the visible image in an existing image element.
- `background-image: url(...)` = paints artwork behind the element's contents.
- `object-fit: contain` = keeps replacement artwork within its image box without stretching it.
- `background-size: cover` = fills a background area, potentially cropping its edges.
- A file path on your own computer is not a Lorebary-hosted image URL. You can also use Base64 image data instead of an uploaded image path.

---


## Visual Expressions

### Custom Visual Expression Icons

Replace the Visual Expressions toggle and management icon; optionally add an image overlay to the expression portrait.

![Custom Visual Expression Icons](./images/expression-decorative-portrait-overlay.png)

```css
/* Hide the original expression toggle image */
[data-lab="expression-toggle"] img {
  visibility: hidden !important;
}

/* Expression toggle replacement artwork */
[data-lab="expression-toggle"] span {
  width: 20px !important;
  height: 20px !important;
  background-image:
    url("/api/images/6ac8997342880c652f056e23") !important;
  background-repeat: no-repeat !important;
  background-position: center !important;
  background-size: contain !important;
}

/* Manage Expressions */
[data-lab="expression-manage"] img {
  content: url("/api/images/6ac8997ed2d7799fdce4e72a") !important;
  object-fit:contain!important;
}

/* Optional portrait decoration */
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
- `visibility: hidden` = hides the original toggle image while keeping the element present.
- `background-image` = displays replacement artwork on the toggle span.
- `content: url(...)` = replaces the Manage icon.
- `::after` = overlays decorative artwork without blocking pointer interactions.
- Replace the sample image URLs with your own.

**Note:** The portrait overlay is decorative rather than a button icon; remove its block if you only want icon replacements.

---

### Glowing Expression Portraits

Add a layered neon glow around a character expression image. ![Glowing Expression Portraits preview](./images/expression-glowing-portraits.png)

```css
[data-lab="expression"] img {
  filter: drop-shadow(0 0 8px #ff69c9)
          drop-shadow(0 0 14px #70dfff)
          drop-shadow(0 0 20px #a78bfa) !important;
}
```

**Customization:**
- Each `drop-shadow` adds another color and blur radius.
- Reduce the radii or remove layers for a subtler effect.

---

### Move Expression Portraits to the Right

Anchor the expression portrait on the right side of the chat. ![Move Expression Portraits to the Right preview](./images/expression-floating-portraits.png)

```css
[data-lab="expression"] {
  left: auto !important;
  right: 0 !important;
  bottom: 0 !important;
}
```

**Customization:**
- `right: 0` anchors the portrait to the right.
- `bottom: 0` aligns it to the bottom.
- `left: auto` releases the original left positioning.

**Compatibility:** Portrait placement examples are alternatives. Combine their positioning declarations deliberately rather than pasting all portrait-position rules together.

---

### Floating Expression Portraits

Lift and resize the portrait to create a floating side accent.

```css
[data-lab="expression"] {
  left: auto !important;
  right: 0 !important;
  bottom: 50px !important;
  width: clamp(16rem, 30vw, 28rem) !important;
  height: min(55dvh / var(--content-ui-scale, 1), 100%) !important;
  max-height: 32rem !important;
}
```

**Customization:**
- `bottom` controls how high the portrait floats.
- `width: clamp(...)` makes its width responsive.
- `max-height` limits its size.

---

### Expression Toggle Button Colors

Recolor the visual-expression toggle and its active state. ![Expression Toggle Button Colors preview](./images/expression-toggle-button-colors.png)

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
- `background` sets the normal button color.
- `border` and `box-shadow` provide the pink accent.
- `aria-pressed="true"` changes the background while active.

---


## Chat Bubbles

### Custom Message Bubble Backgrounds

Change the default message bubble background and border without changing the text. ![Custom Message Bubble Backgrounds preview](./images/bubble-custom-backgrounds.png)

```css
[data-lab="bubble"] {
  background: #232047 !important;
  border: 1px solid #7063a4 !important;
}
```

**Customization:**
- `background` sets the bubble fill.
- `border` adds an outline; change its color and width to match your theme.


---

### Different User and Character Message Bubbles

Give user and character messages different colors using LoreBary's built-in bubble variables. ![Different User and Character Message Bubbles preview](./images/bubble-user-character-colors.png)

```css
[data-lab="bubble"] {
  --lab-bubble-user-bg: #ff79ca;
  --lab-bubble-user-border-color: #8deaff;
  --lab-bubble-bg: #211b31;
  --lab-bubble-border-color: #ff79ca;
  --lab-bubble-border-width: 3px;
  --lab-bubble-border-style: solid;
}
```

**Customization:**
- `--lab-bubble-user-bg` and `--lab-bubble-user-border-color` style user messages.
- `--lab-bubble-bg` and `--lab-bubble-border-color` style character messages.
- `--lab-bubble-border-width` and `--lab-bubble-border-style` are shared by both.
- Bubble tails use the corresponding background variable, so their fill follows the bubble color.


---

### Bubble Tail Effects and Removal

LoreBary exposes the speech-bubble pointer as `[data-lab="bubble-tail"]`. Add a glow, or hide the pointer entirely.

```css
/* Optional glowing tails */
[data-lab="bubble-tail"] {
  filter: drop-shadow(0 0 5px #ff79ca) !important;
  transition: filter .2s ease !important;
}
@media (hover: hover) {
  [data-lab="bubble"]:hover > [data-lab="bubble-tail"] {
    filter: drop-shadow(0 0 9px #8deaff) !important;
  }
}
```

To **hide tails instead**, use this alternative:

```css
[data-lab="bubble-tail"] { display: none !important; }
```


---

### Bubble Transparency Without Fading Text

`--lab-bubble-opacity` controls the **entire bubble**, including its text and action buttons. For translucent backgrounds with crisp text, use alpha-transparent background colors and restore full opacity:

```css
[data-lab="bubble"] {
  --lab-bubble-opacity: 1;
  --lab-bubble-user-bg: #ff79ca55;
  --lab-bubble-bg: #8deaff33;
  --lab-bubble-user-border-color: #ff79ca;
  --lab-bubble-border-color: #8deaff;
  --lab-bubble-border-width: 2px;
  --lab-bubble-border-style: solid;
}
```


---

### Decorative Message Bubble Ornaments

Add a line of decorative symbols above each message. ![Decorative Message Bubble Ornaments preview](./images/bubble-decorative-ornaments.png)

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
- `content` sets the decorative characters.
- `padding-top` makes room so the ornament does not overlap text.
- `top`, `left`, and `right` control placement.
- `color` recolors the symbols.

**Note:** Check long messages and narrow/mobile layouts. This is an ornament above the text, not an uploaded-image replacement.

---

### Message Bubble Hover Glow

Highlight a message bubble when a pointer moves over it.

```css
[data-lab="bubble"] {
  transition: box-shadow .2s ease !important;
}

@media (hover: hover) {
  [data-lab="bubble"]:hover {
    box-shadow: 0 0 12px #ff85c466 !important;
  }
}

@media (prefers-reduced-motion: reduce) {
  [data-lab="bubble"] {
    transition: none !important;
  }
}
```

**Customization:**
- `box-shadow` sets the hover glow.
- `.2s` controls transition speed.
- `@media (hover: hover)` limits the effect to hover-capable devices.


**Compatibility:** This is an alternative hover shadow to **Bubble Hover Lift** above. Both set the bubble’s hover `box-shadow`; combine their shadow values if you want both effects.

---


## Message Text and Formatting

### Message Text, Bold, and Italic

```css
[data-lab="message-body"] > div[data-selection-root="true"] [data-lab="text"] {
  color: #ff79ca !important;
  text-shadow: 0 0 5px #ff79ca88 !important;
}
[data-lab="message-body"] > div[data-selection-root="true"] [data-lab="bold"] {
  color: #8deaff !important;
}
[data-lab="message-body"] > div[data-selection-root="true"] [data-lab="italic"] {
  color: #ffe17b !important;
}
```


---

### Dialogue, Dividers, and Headings

```css
[data-lab="message-body"] > div[data-selection-root="true"] [data-lab="dialog"] {
  color: #ff79ca !important;
  text-shadow: 0 0 5px #ff79ca88 !important;
}
[data-lab="message-body"] > div[data-selection-root="true"] [data-lab="rule"] {
  background: #ffe17b !important;
  height: 3px !important;
  box-shadow: 0 0 7px #ffe17b !important;
}
[data-lab="message-body"] > div[data-selection-root="true"] [data-lab="heading"] {
  border-bottom: 2px solid #8deaff !important;
  padding-bottom: 4px !important;
}
```


---

### Message List Items

```css
[data-lab="message-body"] > div[data-selection-root="true"] [data-lab="list-item"] {
  background: #ff79ca22 !important;
  border-left: 3px solid #ff79ca !important;
  border-radius: 6px !important;
  padding: 5px 8px !important;
  margin: 5px 0 !important;
  transition: background-color .2s ease !important;
}
@media (hover: hover) {
  [data-lab="message-body"] > div[data-selection-root="true"] [data-lab="list-item"]:hover {
    background: #8deaff33 !important;
  }
}
```


---


## Message Footer and Ratings

### Message Footer and Timestamp Styling

Style the footer container and its timestamp independently:

```css
[data-lab="message-footer"] {
  background: #211b31 !important;
  border: 2px solid #ff79ca !important;
  border-radius: 10px !important;
  padding: 6px 10px !important;
}
[data-lab="message-footer"] [data-lab="time"] {
  color: #8deaff !important;
  font-weight: 700 !important;
  text-shadow: 0 0 6px #8deaff !important;
  transition: color .2s ease, text-shadow .2s ease, transform .2s ease !important;
}
@media (hover: hover) {
  [data-lab="message-footer"] [data-lab="time"]:hover {
    color: #ff79ca !important;
    text-shadow: 0 0 8px #ff79ca !important;
    transform: scale(1.12) !important;
  }
}
```


---

### Custom Rating Icons

Replace each of the five rating symbols with a different uploaded image. ![Custom Rating Icons preview](./images/message-custom-rating-icons.png)

```css
/* Rating 1 of 5 */
[data-lab="rating"] button[aria-label="Rate 1 of 5"] img {
  content: url("/api/images/6ac898fd42880c652f055e95") !important;
}

/* Rating 2 of 5 */
[data-lab="rating"] button[aria-label="Rate 2 of 5"] img {
  content: url("/api/images/6ac8991542880c652f0562cb") !important;
}

/* Rating 3 of 5 */
[data-lab="rating"] button[aria-label="Rate 3 of 5"] img {
  content: url("/api/images/6ac8992042880c652f05646f") !important;
}

/* Rating 4 of 5 */
[data-lab="rating"] button[aria-label="Rate 4 of 5"] img {
  content: url("/api/images/6ac8995ad2d7799fdce4e272") !important;
}

/* Rating 5 of 5 */
[data-lab="rating"] button[aria-label="Rate 5 of 5"] img {
  content: url("/api/images/6ac8996500c414e8e2a2153e") !important;
}

/* Shared rating image styling */
[data-lab="rating"] button img {
  object-fit:contain!important;
  filter:none!important;
}
```

**Customization:**
- `Rate 1 of 5` through `Rate 5 of 5` = each individual rating button.
- `filter: none` = preserves the original colors of the uploaded artwork.
- Replace all five image URLs with your own images.

---


## Thinking Panel

### Thinking Panel Background and Text

Recolor the Thinking panel independently of the main message body. ![Thinking Panel Background and Text preview](./images/panel-thinking-panel-background-and-text.png)

```css
/* Panel and header */
[data-lab="thoughts"] {
  background: #211b31 !important;
  border: 2px solid #ff79ca !important;
  border-radius: 12px !important;
  box-shadow: 0 0 10px #ff79ca55 !important;
}
[data-lab="thoughts-toggle"] {
  background: #ff79ca33 !important;
  border-bottom: 1px solid #ff79ca !important;
}
/* Header title and icons */
[data-lab="thoughts-toggle"] > span {
  color: #ff79ca !important;
  font-weight: 700 !important;
  text-shadow: 0 0 6px #ff79ca !important;
}
[data-lab="thoughts-toggle"] > i {
  color: #8deaff !important;
  filter: drop-shadow(0 0 4px #8deaff) !important;
}
/* Thinking content */
[data-lab="thoughts-text"] {
  background: #211b31 !important;
  border-left: 3px solid #ff79ca !important;
  border-radius: 6px !important;
  padding: 10px !important;
}
[data-lab="thoughts-text"] [data-lab="text"] {
  color: #8deaff !important;
  text-shadow: 0 0 4px #8deaff88 !important;
}
[data-lab="thoughts-text"] [data-lab="italic"] {
  color: #ffe17b !important;
}
```


---

### Thinking Panel Hover Effects

```css
[data-lab="thoughts"] {
  transition: box-shadow .25s ease, border-color .25s ease !important;
}
@media (hover: hover) {
  [data-lab="thoughts"]:hover {
    border-color: #8deaff !important;
    box-shadow: 0 0 10px #8deaff88, 0 0 20px #ff79ca55 !important;
  }
  [data-lab="thoughts-toggle"]:hover {
    background: #ff79ca22 !important;
  }
}
```


---


## Header and Footer

**Effect examples, not button restrictions:** The named buttons in the effects below are simply convenient demonstrations. To apply an effect to a different header button, replace the example `aria-label` with the target button’s label. Some recipes style the `img` inside a button; others style the button itself or a `::before` ring. Keep that distinction when changing targets. Where a recipe combines multiple selectors, update every occurrence consistently.

### Custom Header Button Icons

Replace the six standard chat header icons without changing their buttons. ![Custom Header Button Icons preview](./images/header-custom-button-icons.png)

```css
/* Voice Call */
[data-lab="header-action"][aria-label="Voice call"] img {
  content: url("/api/images/6ac89c4900c414e8e2a275d5") !important;
}

/* Fullscreen */
[data-lab="header-action"][aria-label*="fullscreen" i] img {
  content: url("/api/images/6ac89c361a947bf5aa447504") !important;
}

/* Statistics & Export */
[data-lab="header-action"][aria-label="Chat statistics & export"] img {
  content: url("/api/images/6ac89c3f42880c652f05d37b") !important;
}

/* Search */
[data-lab="header-action"][aria-label="Search this chat"] img {
  content: url("/api/images/6ac897301a947bf5aa43d1c8") !important;
}

/* Scene Gallery */
[data-lab="header-action"][aria-label="Scene gallery"] img {
  content: url("/api/images/6ac896c642880c652f0508b0") !important;
}

/* Bookmarks */
[data-lab="header-action"][aria-label="Message bookmarks"] img {
  content: url("/api/images/6ac897231a947bf5aa43cf04") !important;
}
```

**Customization:**
- `aria-label` = identifies the particular header button.
- `content: url(...)` = the replacement image.
- You may keep only the button rules you want to customize.
- Replace each uploaded image URL with your own.

---

### Custom Navigation Icons

Replace the Back, Scroll Down, Previous Version, and Next Version icons. ![Custom Navigation Icons preview](./images/header-custom-navigation-icons.png)

```css
/* Back */
[data-lab="back"] img {
  content: url("/api/images/6ac8975242880c652f051da0") !important;
  object-fit:contain!important;
}

/* Scroll Down */
[data-lab="scroll-down"] img {
  content: url("/api/images/6ac896f900c414e8e2a1bffd") !important;
  object-fit:contain!important;
  transform: none !important;
}

/* Previous Version */
[data-lab="swipe"][aria-label="Previous version"] img {
  content: url("/api/images/6ac896e875e1eb8796dcf891") !important;
  object-fit:contain!important;
  transform: none !important;
  filter:none!important;
}

/* Next Version */
[data-lab="swipe"][aria-label="Next version"] img {
  content: url("/api/images/6ac896dc75e1eb8796dcf708") !important;
  object-fit:contain!important;
  transform: none !important;
  filter:none!important;
}
```

**Customization:**
- `aria-label` = distinguishes previous and next message versions.
- `transform: none` = removes a pre-existing transformation on selected navigation images.
- Replace the sample URLs with your own.

---

### Custom Footer Button Icons

Replace the footer control icons for Web Search, Director Pass, Auto Mode, Review Mode, Scene Music, Visual Expressions, Dice Roll, HTML Mode, Time Skip, and Reply Options. ![Custom Footer Button Icons preview](./images/footer-custom-button-icons.png)

```css
/* Web Search */
[data-lab="web-search"] img {
  content: url("/api/images/6ac89bb142880c652f05bb82") !important;
  object-fit: contain !important;
}

/* Director Pass */
[data-lab="director-pass"] img {
  content: url("/api/images/6ac89bbd00c414e8e2a263df") !important;
  object-fit: contain !important;
}

/* Auto Mode */
[data-lab="auto-mode"] img {
  content: url("/api/images/6ac89bc942880c652f05befd") !important;
  object-fit: contain !important;
}

/* Review Mode */
[data-lab="review-mode"] img {
  content: url("/api/images/6ac89bd5aab27ff458cf5f00") !important;
  object-fit: contain !important;
}

/* Scene Music */
[data-lab="scene-music"] img {
  content: url("/api/images/6ac89bffaab27ff458cf636e") !important;
  object-fit: contain !important;
}

/* Visual Expressions */
[data-lab="visual-expressions"] img {
  content: url("/api/images/6ac89c09d2d7799fdce54ff7") !important;
  object-fit: contain !important;
}

/* Dice Roll */
[data-lab="dice-roll"] img {
  content: url("/api/images/6ac89c1400c414e8e2a26e15") !important;
  object-fit: contain !important;
}

/* HTML Mode */
[data-lab="html-mode"] img {
  content: url("/api/images/6ac8a0a61a947bf5aa45143c") !important;
  object-fit: contain !important;
  filter: none !important;
}

/* Time Skip */
[data-lab="time-skip"] img {
  content: url("/api/images/6ac89bdf75e1eb8796dd8d1a") !important;
  object-fit: contain !important;
}

/* Reply Options / Reply Choices */
[data-lab="reply-options"] img {
  content: url("/api/images/6ac89bf3d2d7799fdce54db2") !important;
  object-fit: contain !important;
}
```

**Customization:**
- Each `data-lab` selector targets one footer button; remove rules for controls you don't want to change.
- `content: url(...)` = the uploaded replacement image for that button.
- `object-fit: contain` = keeps the image proportional within its existing icon box.
- `filter: none` = prevents inherited filters from changing HTML Mode's image colors.
- Replace the sample `/api/images/...` URLs with your own uploaded artwork.

---

The Story Goals button appears in the Laboratory footer. Its appearance can be customized to match the rest of your chat controls.
Use [data-lab="story-goals"] to customize the Story Goals button without changing the other footer controls.
```
/* Story Goals footer button */
[data-lab="footer"] [data-lab="story-goals"] {
  background: #30243f;
  border: 1px solid #b49aff;
  border-radius: 10px;
  color: #ffe3f4;
}

/* Story Goals icon */
[data-lab="footer"] [data-lab="story-goals"] img {
  filter: brightness(0) saturate(100%)
    invert(79%) sepia(28%) saturate(1060%)
    hue-rotate(288deg);
}

/* Hover */
@media (hover: hover) {
  [data-lab="footer"] [data-lab="story-goals"]:hover {
    background: #453457;
    border-color: #ff79ca;
  }
}

/* Story Goals enabled */
[data-lab="story-goals"][aria-pressed="true"] {
  background: #453457;
  box-shadow: 0 0 0 1px #ff79ca, 0 0 8px #ff79ca55;
  color: #ffe17b;
}

/* Story Goals disabled */
[data-lab="story-goals"][aria-pressed="false"] {
  background: #30243f;
  box-shadow: none;
}
```
Customization:
- background changes the button's surface.
- border controls its outline.
- border-radius adjusts its corners.
- color changes the button's text color.
- filter recolors the Story Goals icon.
- :hover provides a separate appearance when the pointer is over the button.
The button can also be targeted directly using [data-lab="story-goals"] if you prefer a shorter selector.

---

### Icon Glow — Search Example

Give an icon a neon halo, using Search as the example. ![Glowing Search Icon preview](./images/header-glowing-search-icon.png)

```css
[data-lab="header-action"][aria-label="Search this chat"] img {
  filter: drop-shadow(0 0 3px #ff79ca)
          drop-shadow(0 0 7px #ff79ca) !important;
}
```

**Customization:**
- Change `#ff79ca` to recolor both glow layers.
- Increase the blur radii for a softer, wider halo.

**Compatibility:** Other icon tint rules also set `filter`. Combine tint and glow in one `filter` declaration instead of applying separate competing rules.

---

### Rainbow Button Background — Search Example

Apply a stationary pastel rainbow to a button. Change the `aria-label` selector to target a different button. ![Rainbow button background preview](./images/header-rainbow-button-background.png)

```css
[data-lab="header-action"][aria-label="Search this chat"] {
  background: linear-gradient(135deg,
    #ff7a9c 0%, #ffdc79 20%, #8ee8b3 40%,
    #7fdfff 60%, #b69cff 80%, #ff8bd3 100%) !important;
  border: 1px solid #ffe2f3 !important;
}
```

**Customization:**
- Edit the gradient stops to choose a different rainbow.
- Change `135deg` to turn the gradient.
- Adjust `border` for a stronger or subtler outline.

---

### Icon Hover Enlargement — Gallery Example

Enlarge an icon on hover. The Scene gallery selector below is one example; change the `aria-label` to target another header action.

```css
[data-lab="header-action"][aria-label="Scene gallery"] img {
  transition: transform .2s ease !important;
}
@media (hover: hover) {
  [data-lab="header-action"][aria-label="Scene gallery"]:hover img {
    transform: scale(1.35) !important;
  }
}
@media (prefers-reduced-motion: reduce) {
  [data-lab="header-action"][aria-label="Scene gallery"] img {
    transition: none !important;
  }
}
```

**Customization:**
- `scale(1.35)` determines the hover enlargement.
- `.2s` controls the transition speed.

---

### Animated Rainbow Button — Gallery Example

Cycle the colors of a rainbow button background, using Gallery as the example. ![Animated Rainbow Gallery Button preview](./images/header-animated-rainbow-gallery-button.png)

```css
[data-lab="header-action"][aria-label="Scene gallery"] {
  background: conic-gradient(from 0deg,
    #ff7a9c, #ffdc79, #8ee8b3,
    #7fdfff, #b69cff, #ff8bd3, #ff7a9c) !important;
  background-size: 100% 100% !important;
  border: 1px solid #d5b8f5 !important;
  animation: lab-gallery-rainbow-spin 4s linear infinite !important;
}
@keyframes lab-gallery-rainbow-spin {
  0% { filter: hue-rotate(0deg); }
  100% { filter: hue-rotate(360deg); }
}
@media (prefers-reduced-motion: reduce) {
  [data-lab="header-action"][aria-label="Scene gallery"] {
    animation: none !important;
  }
}
```

**Customization:**
- `4s` sets the full color-cycle duration.
- Change the gradient colors to customize the palette.

**Note:** This confirmed method animates `filter` on the whole button, so the icon colors can shift too. A separate hover `filter: brightness(...)` rule can interrupt the hue-cycle while hovered; see the optional shared hover tutorial below.

---

### Multicolor Icon Glow — Bookmarks Example

Surround an icon with multicolor light on hover, using Bookmarks as the example. ![Multicolor Bookmarks Icon Glow preview](./images/header-multicolor-bookmarks-glow.png)

```css
[data-lab="header-action"][aria-label="Message bookmarks"] img {
  transition: filter .2s ease !important;
}
@media (hover: hover) {
  [data-lab="header-action"][aria-label="Message bookmarks"]:hover img {
    filter: drop-shadow(-3px 0 3px #ff6b9e)
            drop-shadow(3px 0 3px #75e8ff)
            drop-shadow(0 3px 4px #b78aff) !important;
  }
}
@media (prefers-reduced-motion: reduce) {
  [data-lab="header-action"][aria-label="Message bookmarks"] img {
    transition: none !important;
  }
}
```

**Customization:**
- The three hex values set the left, right, and lower glow colors.
- The shadow offsets determine where each color appears.

---

### Rotating Rainbow Button Border — Bookmarks Example

Build a rotating rainbow ring around a button while keeping its icon stationary, using Bookmarks as the example. ![Rotating Rainbow Bookmarks Border preview](./images/header-rotating-rainbow-bookmarks-border.png)

```css
[data-lab="header-action"][aria-label="Message bookmarks"] {
  position: relative !important;
  isolation: isolate !important;
  overflow: visible !important;
  background: #242b3c !important;
  border: 2px solid transparent !important;
  border-radius: 50% !important;
  animation: none !important;
}
[data-lab="header-action"][aria-label="Message bookmarks"]::before {
  content: "" !important;
  position: absolute !important;
  inset: -2px !important;
  border-radius: 50% !important;
  pointer-events: none !important;
  z-index: -1 !important;
  background: conic-gradient(
    #ff7a9c, #ffdc79, #8ee8b3,
    #7fdfff, #b69cff, #ff8bd3, #ff7a9c) !important;
  -webkit-mask: radial-gradient(farthest-side,
    transparent calc(100% - 3px), #000 calc(100% - 2px)) !important;
  mask: radial-gradient(farthest-side,
    transparent calc(100% - 3px), #000 calc(100% - 2px)) !important;
  animation: lab-bookmark-ring-spin 3s linear infinite !important;
}
@keyframes lab-bookmark-ring-spin {
  to { transform: rotate(360deg); }
}
@media (hover: hover) {
  [data-lab="header-action"][aria-label="Message bookmarks"]:hover::before {
    animation-play-state: paused !important;
  }
}
@media (prefers-reduced-motion: reduce) {
  [data-lab="header-action"][aria-label="Message bookmarks"]::before {
    animation: none !important;
  }
}
```

**Customization:**
- `3s` controls rotation speed.
- Change the conic-gradient colors for a different ring.
- The mask creates the narrow ring; its pixel values control thickness.

**Note:** The pseudo-element and its mask are both needed. Keep this tutorial together; replacing only the gradient will not reproduce the ring.

---

### Solid Button Border — Voice Call Example

Frame a button with a solid circular border, using Voice Call as the example. ![Custom Voice Call Button Border preview](./images/header-voice-call-button-border.png)

```css
[data-lab="header-action"][aria-label="Voice call"] {
  background: #242b3c !important;
  border: 2px solid #ff88c8 !important;
  border-radius: 50% !important;
}
```

**Customization:**
- `#242b3c` sets the inner fill.
- `#ff88c8` sets the outline color.
- `2px` sets the border thickness.

---

### Gradient Button Border — Fullscreen Example

Give a button a gradient border without filling its center with a gradient, using Fullscreen as the example. ![Gradient Fullscreen Button Border preview](./images/header-gradient-fullscreen-button-border.png)

```css
[data-lab="header-action"][aria-label*="fullscreen" i] {
  border: 2px solid transparent !important;
  border-radius: 50% !important;
  background: linear-gradient(#242b3c, #242b3c) padding-box,
              linear-gradient(135deg, #ff89ca, #76e7ff) border-box !important;
}
```

**Customization:**
- Change the two `border-box` colors to alter the gradient.
- Change `#242b3c` in both positions to recolor the center.
- `135deg` controls the gradient direction.

---

### Pulsing Button Glow — Fullscreen Example

Add a gentle two-color pulse around a button, using Fullscreen as the example. ![Pulsing Fullscreen Button preview](./images/header-pulsing-fullscreen-button.png)

```css
[data-lab="header-action"][aria-label*="fullscreen" i] {
  animation: lab-border-pulse 2.8s ease-in-out infinite !important;
}
@keyframes lab-border-pulse {
  0%, 100% {
    box-shadow: 0 0 3px #ff89ca55, 0 0 6px #76e7ff33;
  }
  50% {
    box-shadow: 0 0 8px #ff89caaa, 0 0 15px #76e7ff88;
  }
}
@media (prefers-reduced-motion: reduce) {
  [data-lab="header-action"][aria-label*="fullscreen" i] {
    animation: none !important;
  }
}
```

**Customization:**
- `2.8s` sets the pulse period.
- The two `box-shadow` colors set pink and cyan glows.

**Note:** Pairs with the Gradient Fullscreen Button Border tutorial; the border itself is not animated.

---

### Bobbing Icon Animation — Statistics Example

Give an icon a gentle floating motion, using Statistics as the example.

```css
[data-lab="header-action"][aria-label="Chat statistics & export"] img {
  animation: lab-icon-float 2.6s ease-in-out infinite !important;
}
@keyframes lab-icon-float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-3px); }
}
@media (prefers-reduced-motion: reduce) {
  [data-lab="header-action"][aria-label="Chat statistics & export"] img {
    animation: none !important;
  }
}
```

**Customization:**
- `-3px` controls how far the icon rises.
- `2.6s` controls the motion speed.

---

### Button Hover Glow — Statistics Example

Outline a button only while hovered, using Statistics as the example. ![Statistics Button Hover Glow preview](./images/header-statistics-button-hover-glow.png)

```css
[data-lab="header-action"][aria-label="Chat statistics & export"] {
  border: 2px solid transparent !important;
  border-radius: 50% !important;
  transition: border-color .2s ease, box-shadow .2s ease !important;
}
@media (hover: hover) {
  [data-lab="header-action"][aria-label="Chat statistics & export"]:hover {
    border-color: #8de8c0 !important;
    box-shadow: 0 0 9px #8de8c066 !important;
  }
}
@media (prefers-reduced-motion: reduce) {
  [data-lab="header-action"][aria-label="Chat statistics & export"] {
    transition: none !important;
  }
}
```

**Customization:**
- Change `#8de8c0` to recolor the mint border.
- `9px` adjusts glow spread.

---

### Shared Button Hover Brightness — Header Examples

Lighten selected header buttons when hovered.

```css
@media (hover: hover) {
  [data-lab="header-action"]:is(
    [aria-label="Voice call"],
    [aria-label*="fullscreen" i],
    [aria-label="Search this chat"],
    [aria-label="Scene gallery"]
  ):hover {
    filter: brightness(1.12) !important;
  }
}
```

**Customization:**
- `brightness(1.12)` controls the intensity.
- Remove a button label from `:is(...)` to exclude that control.

**Note:** Optional source rule. It sets `filter` on the Gallery button, the same property used by the Gallery hue-cycle animation; test their combined hover behavior before publishing them together.

---

### Button Keyboard Focus Outlines — Header Examples

Give keyboard users a visible pale-yellow outline on the main header actions.

```css
[data-lab="header-action"]:is(
  [aria-label="Voice call"],
  [aria-label*="fullscreen" i],
  [aria-label="Search this chat"],
  [aria-label="Scene gallery"],
  [aria-label="Chat statistics & export"],
  [aria-label="Message bookmarks"]
):focus-visible {
  outline: 2px solid #fff0a6 !important;
  outline-offset: 3px !important;
}
```

**Customization:**
- `#fff0a6` sets the focus-ring color.
- `outline-offset: 3px` adds breathing room around the button.

**Note:** This is keyboard focus, not a selected or toggled state. A screenshot may require navigating with Tab rather than clicking.

---

### Rainbow Icon Recoloring — Gallery Example



![Rainbow recolored Gallery icon example](./images/header-rainbow-recolored-gallery-icon.png)
```css
/* Recolor the icon itself. */
[data-lab="header-action"][aria-label="Scene gallery"] img {
  filter: hue-rotate(145deg) saturate(1.8) contrast(1.2) !important;
}

/* Add this to the animated Gallery button tutorial above:
   its existing parent-button hue-rotate animation remains in place. */
```

**Customization:**
- `hue-rotate(145deg)` shifts the icon's colors before the button animation runs.
- `saturate(1.8)` strengthens the icon colors; `contrast(1.2)` sharpens their separation.
- The existing **Animated Rainbow Gallery Button** tutorial animates `filter: hue-rotate(...)` on the *parent button*. This icon filter is static on the child image; together they create the observed changing rainbow icon.

## Additional Characters

The Laboratory includes an Add Character button for introducing additional characters into the current scene. Its circular button and image icon can be styled independently.

### Add Character Button

Use `[aria-label="Add a character to this scene"]` to customize the button's appearance.

```css
/* Add Character button */
button[aria-label="Add a character to this scene"] {
  background: #211b31;
  border: 2px solid #65ef9a;
  border-radius: 50%;
  box-shadow: 0 2px 8px #0005;
}

/* Add Character icon */
button[aria-label="Add a character to this scene"] img {
  filter: grayscale(1) sepia(1)
    saturate(3) hue-rotate(85deg)
    brightness(1.2);
}
```

**Customization:**

- `background` changes the button's surface.
- `border` controls its outline and color.
- `border-radius` adjusts the button's shape. Use `50%` for a circular appearance.
- `box-shadow` adds depth beneath the button.
- The nested `img` selector targets the Add Character icon.
- `filter` recolors the icon without replacing its artwork.

---
## Time Skip

Time Skip allows the story to advance forward in time. In the Laboratory, it includes a dedicated in-chat message, editing controls, and a menu for configuring the time skip.

These elements can be customized independently of the regular chat messages.

### Time Skip Message

The in-chat Time Skip message includes a decorative card, clock icon, title, description, and separator.

Use `[data-lab="time-skip"]` with its internal elements to style the message without changing the Time Skip button in the Laboratory footer.

```css
/* Time Skip message card */
[data-lab="time-skip"] > div.relative > div {
  background: #29243e;
  border: 2px solid #ffad55;
  border-radius: 16px;
  box-shadow: 0 4px 16px #0006;
}

/* Clock icon */
[data-lab="time-skip"] .fa-clock {
  color: #ffe36b;
}

/* Clock icon container */
[data-lab="time-skip"] div:has(> .fa-clock) {
  background: #453457;
  border: 1px solid #ffe36b;
}

/* Main message text */
[data-lab="time-skip"] p {
  color: #ffe3f4;
}

/* Highlighted text */
[data-lab="time-skip"] p span {
  color: #ffe36b;
}

/* Description */
[data-lab="time-skip"] p.mt-1 {
  color: #c5afd4;
}

/* Decorative separator */
[data-lab="time-skip"] > .flex-1 {
  background: linear-gradient(
    90deg,
    transparent,
    #cf83ff,
    #54e8ef,
    transparent
  );
}
```

**Customization:**
- `div.relative > div` styles the in-chat Time Skip card.
- `.fa-clock` recolors the clock icon.
- `div:has(> .fa-clock)` styles the clock's surrounding container.
- `p` controls the main message text.
- `p span` highlights text inside the message.
- `p.mt-1` styles the secondary description.
- `.flex-1` creates the decorative separator beside the message.

The gradient separator can be replaced with a solid color or a different gradient.

---

### Time Skip Edit and Delete Buttons

Time Skip messages include separate Edit and Delete controls. Each button can use its own border, background, and icon color.

```css
/* Edit button */
[data-lab="time-skip"] > button[aria-label="Edit"] {
  background: #30243f;
  border: 1px solid #b49aff;
  border-radius: 9px;
}

/* Edit icon */
[data-lab="time-skip"] > button[aria-label="Edit"] img {
  filter: sepia(1) saturate(2)
    hue-rotate(355deg);
}

/* Delete button */
[data-lab="time-skip"] > button[aria-label="Delete"] {
  background: #30243f;
  border: 1px solid #ff548d;
  border-radius: 9px;
}

/* Delete icon */
[data-lab="time-skip"] > button[aria-label="Delete"] img {
  filter: sepia(1) saturate(3)
    hue-rotate(285deg);
}
```

**Customization:**
- `[aria-label="Edit"]` targets the Time Skip editing control.
- `[aria-label="Delete"]` targets its deletion control.
- `background` changes the button surface.
- `border` creates a colored outline.
- `border-radius` adjusts the corners.
- The nested `img` selectors recolor each button's icon.

The direct-child selector (`> button`) keeps these rules focused on the in-chat message controls.

---

## Message Actions and Input Controls

### Individual Message Action Colors and Hover

Target the individual actions by their confirmed labels. Branch is present on character messages in the supplied sample but not on the user message.

```css
[data-lab="bubble"] [data-lab="action"][aria-label="Bookmark message"] { background: #ff79ca !important; }
[data-lab="bubble"] [data-lab="action"][aria-label="Edit message"] { background: #8deaff !important; }
[data-lab="bubble"] [data-lab="action"][aria-label="Delete message"] { background: #ffb36b !important; }
[data-lab="bubble"] [data-lab="action"][aria-label="Branch chat"] { background: #b49aff !important; }

[data-lab="bubble"] [data-lab="action"] {
  transition: transform .2s ease, box-shadow .2s ease, filter .2s ease !important;
}
@media (hover: hover) {
  [data-lab="bubble"] [data-lab="action"]:hover {
    transform: scale(1.2) !important;
    box-shadow: 0 0 10px #ff79ca !important;
    filter: brightness(1.3) !important;
  }
}
@media (prefers-reduced-motion: reduce) {
  [data-lab="bubble"] [data-lab="action"] { transition: none !important; }
}
```


---

### Custom Menu Button Icon

Replace the standard menu icon and the mobile More Chat Tools icon with your own artwork. ![Custom Menu Button Icon preview](./images/input-custom-menu-button-icon.png)

```css
/* Menu */
img[data-lab="menu"] {
  content: url("/api/images/6ac8974542880c652f051b0e") !important;
  object-fit:contain!important;
}

/* Mobile More Chat Tools */
[data-lab="header-action"][aria-label="More chat tools"] img {
  content: url("/api/images/6ac8cbd875e1eb8796e3a987") !important;
  object-fit: contain !important;
  filter: none !important;
}
```

**Customization:**
- `content: url(...)` = your uploaded menu artwork.
- `object-fit: contain` = preserves the image proportions.
- The mobile **More Chat Tools** control is a separate button from the main menu; each can use different artwork.
- Replace the sample `/api/images/...` URLs with your own.

---

### Custom Input Button Icons

Replace the composer icons for Send, Stop, Write, Upload Image, Scene Notes, and Toolbar Toggle. ![Custom Input Button Icons preview](./images/input-custom-input-button-icons.png)

```css
/* Send (excluding Stop) */
[data-lab="send"] img:not([src*="icon_stop"]) {
  content: url("/api/images/6ac8971700c414e8e2a1c37b") !important;
  object-fit:contain!important;
}

/* Stop */
[data-lab="send"] img[src*="icon_stop"],
[data-lab="stop"] img {
  content: url("/api/images/6ac8a09475e1eb8796de21e5") !important;
  object-fit:contain!important;
  filter:none!important;
}

/* Write */
[data-lab="write"] img {
  content: url("/api/images/6ac8970875e1eb8796dcfc4f") !important;
  object-fit:contain!important;
}

/* Upload Image */
[data-lab="attach-image"] img {
  content: url("/api/images/6ac89c2575e1eb8796dd935f") !important;
  object-fit:contain!important;
}

/* Scene Notes / Guidance */
[data-lab="guidance-toggle"] img {
  content: url("/api/images/6ac8967a1a947bf5aa43be05") !important;
  object-fit:contain!important;
}

/* Toolbar Toggle */
[data-lab="toolbar-toggle"] img {
  content: url("/api/images/6ac896b91a947bf5aa43c355") !important;
  object-fit:contain!important;
}
```

**Customization:**
- `data-lab` = identifies each composer control.
- The Send and Stop selectors are separated so their artwork can differ.
- `content: url(...)` = the image you uploaded.
- Replace the sample URLs with your own.

---

### Custom Draft Version Controls

Customize the separate draft-version navigation row, including its Previous, Next, Regenerate, and Keep Draft controls. This row uses `[data-lab="draft-versions"]` and is **not** the same as the normal message-version swipe controls. ![Draft version controls preview](./images/input-custom-draft-version-controls.png)

```css
/* Previous draft — use artwork facing left */
[data-lab="draft-versions"] button[aria-label="Previous draft version"] img {
  content: url("/api/images/6ac896e875e1eb8796dcf891") !important;
  object-fit: contain !important;
  transform: none !important;
  filter: none !important;
}

/* Next draft — use artwork facing right */
[data-lab="draft-versions"] button[aria-label="Next draft version"] img {
  content: url("/api/images/6ac896dc75e1eb8796dcf708") !important;
  object-fit: contain !important;
  transform: none !important;
  filter: none !important;
}

/* Regenerate draft — this is a Font Awesome <i>, not an <img> */
[data-lab="draft-versions"] button[aria-label="Regenerate draft versions"] i {
  color: #7fdfff !important;
  font-size: 14px !important;
  text-shadow: 0 0 5px #7fdfff88 !important;
}

/* Keep draft and close — also a Font Awesome <i> */
[data-lab="draft-versions"] button[aria-label="Keep draft and close versions"] i {
  color: #ff89ca !important;
  font-size: 14px !important;
  text-shadow: 0 0 5px #ff89ca88 !important;
}
```

**Customization:**
- `draft-versions` = limits changes to the draft-version controls, not ordinary message swipes or message regeneration.
- `Previous draft version` and `Next draft version` = separate buttons with their own images.
- `transform: none` = removes the default mirrored-arrow transformation; use correctly oriented replacement artwork.
- `Regenerate draft versions` and `Keep draft and close versions` = Font Awesome icons rendered with `<i>`, so `content: url(...)` image replacement is **not** used for them here.
- `color`, `font-size`, and `text-shadow` = recolor and emphasize those two icons without changing their symbols.

**Tip:** These controls belong to the draft-version row, not the regular message actions. Preview the example with draft versions visible before keeping it.

---

### Custom Message Action Icons

Desktop and mobile controls may use different images. For example, desktop Regenerate uses `/img/Icons/icon_regenerate.webp`, while mobile Regenerate uses `/img/pixel/msg-regenerate.webp` with a separate `/img/pixel/settings.webp` badge.

Replace the icons on individual chat messages, including Bookmark, Regenerate, Branch, Delete, Edit, and More Actions. ![Custom Message Action Icons preview](./images/input-custom-message-action-icons.png)

```css
/* Bookmark Message */
[data-lab="action"][aria-label="Bookmark message"] img {
  content: url("/api/images/6ac897231a947bf5aa43cf04") !important;
  object-fit:contain!important;
  filter:none!important;
}

/* Regenerate */
[data-lab="action"][aria-label="Regenerate"]
> span > img {
  content: url("/api/images/6ac8cba55a1227b9442bfe5a") !important;
  object-fit:contain!important;
  filter:none!important;
}

/* Branch Chat */
[data-lab="action"][aria-label="Branch chat"] img {
  content: url("/api/images/6ac8cbb442880c652f0bc31f") !important;
  object-fit:contain!important;
  filter:none!important;
}

/* Delete Message */
[data-lab="action"][aria-label="Delete message"] img {
  content: url("/api/images/6ac8cbc275e1eb8796e3a83d") !important;
  object-fit:contain!important;
  filter:none!important;
}

/* Edit Message */
[data-lab="action"][aria-label="Edit message"] img {
  content: url("/api/images/6ac8cbcf5a1227b9442c03e1") !important;
  object-fit:contain!important;
  filter:none!important;
}

/* More Actions */
[data-lab="action"][aria-label="More actions"] img {
  content: url("/api/images/6ac8cbd875e1eb8796e3a987") !important;
  object-fit:contain!important;
  filter:none!important;
}
```

**Customization:**
- `aria-label` = selects the message action to replace.
- The Regenerate selector targets the main image inside its button rather than other nested artwork.
- `filter: none` = preserves your image colors.
- Replace each sample image URL with your own.

---
## Calls and Fast Forward

The Laboratory includes in-chat call notifications and a Fast Forward control for accelerating text streaming. These elements can be customized separately from ordinary messages and footer controls.

### Call Notifications

Call notifications use `[data-lab="call"]`. Customize their text and decorative separator lines.

```css
/* Call notification text */
[data-lab="call"] {
  color: #ffe3f4;
}

/* Decorative separator */
[data-lab="call"] > div.flex-1.h-px {
  background: linear-gradient(
    90deg,
    transparent,
    #b49aff,
    transparent
  );
}

/* Notification label */
[data-lab="call"] span.text-gray-400 {
  color: #ffe3f4;
}

/* Call duration */
[data-lab="call"] span.tabular-nums {
  color: #c5afd4;
}
```

**Customization:**

- `[data-lab="call"]` targets the call notification.
- `color` changes the notification's text color.
- `.flex-1.h-px` styles its decorative separator.
- `.text-gray-400` targets the secondary notification label.
- `.tabular-nums` styles the call duration.

---

### Disconnected Call Indicator

The disconnected-call indicator includes a phone icon inside a decorated container.

```css
/* Disconnected call container */
[data-lab="call"] > div:has(> i.fa-phone-slash) {
  background: #29243e;
  border: 1px solid #b49aff;
  border-radius: 10px;
  box-shadow: 0 2px 8px #0005;
}

/* Disconnected phone icon */
[data-lab="call"] i.fa-phone-slash {
  color: #ff548d;
}
```

**Customization:**

- `div:has(> i.fa-phone-slash)` targets the container holding the disconnected-call icon.
- `background` changes the container's fill.
- `border` controls its outline.
- `border-radius` adjusts its corners.
- `box-shadow` adds depth.
- `.fa-phone-slash` recolors the disconnected-call icon.

---

### Call Entry Options

Call notifications include an Entry Options button, which can be styled independently from ordinary message actions.

```css
/* Call Entry Options button */
[data-lab="call"] button[aria-label="Entry options"] {
  background: #211b31;
  border: 1px solid #54e8ef;
  border-radius: 9px;
  color: #54e8ef;
}

/* Entry Options icon */
[data-lab="call"] button[aria-label="Entry options"] i {
  color: #54e8ef;
}
```

**Customization:**

- `[aria-label="Entry options"]` targets the call's options button.
- `background` changes its surface.
- `border` controls its outline.
- `border-radius` adjusts its corners.
- `color` changes the button's text.
- The nested `i` selector recolors its icon.

---

### Fast Forward / Speed Up

The Fast Forward control uses `[data-lab="speed-up-stream"]`. Customize its background, border, text, and icons independently from the regular Laboratory controls.

```css
/* Fast Forward control */
[data-lab="speed-up-stream"] {
  background: #211b31;
  border: 1px solid #ffad55;
  border-radius: 9px;
  color: #ffad55;
}

/* Fast Forward image icon */
[data-lab="speed-up-stream"] img {
  filter: grayscale(1) sepia(1)
    saturate(2.2) hue-rotate(355deg)
    brightness(1.18);
}

/* Fast Forward SVG icon */
[data-lab="speed-up-stream"] svg {
  color: #ffad55;
}
```

**Customization:**

- `background` changes the control's surface.
- `border` sets its outline.
- `border-radius` adjusts its corners.
- `color` changes its text color.
- `img` recolors image-based icons.
- `svg` recolors SVG icons.

### Fast Forward Speed Multiplier Badge

The Fast Forward button displays a small multiplier badge indicating the current streaming speed, such as `8×`. Customize its background, text, border, and positioning.

```css
/* Fast Forward multiplier badge */
[data-lab="speed-up-stream"] > span[aria-hidden="true"] {
  background: #ff79ca;
  color: #211b31;
  border: 1px solid #ffe36b;
  border-radius: 999px;
  box-shadow: 0 2px 6px #0005;
  font-size: 9px;
  font-weight: 800;
}
```

**Customization:**

- `background` changes the badge's fill.
- `color` changes the multiplier text.
- `border` creates a decorative outline.
- `border-radius` controls the badge's shape.
- `box-shadow` adds depth beneath the badge.
- `font-size` adjusts the multiplier's size.
- `font-weight` controls its emphasis.

The badge's position can also be adjusted using `bottom` and `right`:

```css
/* Adjust multiplier badge position */
[data-lab="speed-up-stream"] > span[aria-hidden="true"] {
  bottom: -3px;
  right: -5px;
}
```

---

## Message Decorations and Indicators

The Laboratory uses small icons and indicators to communicate additional information about messages. These elements can be recolored independently from message text, backgrounds, and action buttons.

### Bookmarked Message Indicator

Bookmarked messages display a small bookmark icon. Customize its color and optional glow without changing the Bookmark action button.

```css
/* Bookmarked message indicator */
i.fa-bookmark[title="Bookmarked"] {
  color: #ffad55;
  text-shadow: 0 0 5px #ffad5566;
}
```

**Customization:**

- `color` changes the bookmark indicator's color.
- `text-shadow` adds a soft glow around the icon.
- Increase the shadow's blur radius for a stronger glow.
- Remove `text-shadow` for a flat appearance.

---

### Backup Model Icon

The Laboratory includes a backup model indicator that uses an image icon. Its appearance can be adjusted using CSS filters.

```css
/* Backup model icon */
[data-lab="backup-model"] {
  filter: grayscale(1) sepia(1)
    saturate(3) hue-rotate(285deg)
    brightness(1.2);
  opacity: 1;
}
```

**Customization:**

- `grayscale()` removes the original colors.
- `sepia()` and `saturate()` prepare the icon for recoloring.
- `hue-rotate()` changes its tint.
- `brightness()` adjusts its lightness.
- `opacity` controls the icon's transparency.

---

### Managing Tinting, Filters, and Icon Replacements

A quick reference for choosing an approach.

| Goal | Use | Important distinction |
|---|---|---|
| Change the button's background | `background` / gradients on the button | Does not recolor the icon pixels |
| Tint the icon image | `filter` on `img` | Affects all visible image pixels together |
| Invert the icon | `invert()` on `img` | Reverses original colors, not a guaranteed target tint |
| Glow around icon artwork | `drop-shadow()` on `img` | Follows the image's visible silhouette |
| Rainbow-cycle icon and button together | `hue-rotate()` animation on the parent button | Also shifts the colors of rendered children |
| Replace the icon artwork entirely | `content: url(...)` on `img` | Covered in Phase 1; new artwork may respond differently to filters |

**Combining filters:** A single element has one computed `filter` property. Two matching CSS rules do **not** merge their filter functions automatically: the winning declaration replaces the other. For example, a tint and glow on the same icon must be combined:

```css
[data-lab="header-action"][aria-label="Search this chat"] img {
  filter: brightness(0) saturate(100%)
          invert(60%) sepia(75%) saturate(2500%)
          hue-rotate(290deg) brightness(105%)
          drop-shadow(0 0 3px #ff79ca)
          drop-shadow(0 0 7px #ff79ca) !important;
}
```

**Customization:**
- Put color-changing functions **before** `drop-shadow()` if you want to preserve the specified shadow color.
- If Phase 1 replaces an icon, test the filter again: the replacement image's starting colors affect the result.
- A multicolored image is not converted into a clean, independently controlled rainbow by `hue-rotate()` alone. True gradient-filled icon silhouettes generally require an asset-specific mask technique; our earlier icon-mask idea was **not validated**, so no working mask recipe is claimed here.


**Tip:** Combine icon replacement with filters and glow when you want a different finish without changing the surrounding button.

---


## Write for Me

### Write Menu Heading Colors

Recolor the two section headings inside the Write menu. ![Write Menu Heading Colors preview](./images/write-write-menu-heading-colors.png)

```css
[data-lab="write-menu"] > div:first-child
> div > div:first-child {
  color: #ffb4db !important;
}
[data-lab="write-menu"] > div:nth-child(2)
> div > div:first-child {
  color: #84dff0 !important;
}
```

**Customization:**
- `color` changes each heading independently.

**Tip:** These selectors depend on the menu’s child order and may need updating if the layout changes.

---

### Write Menu Actions and Help Text


![Write Menu option and hover styling example](./images/write-write-menu-options-and-hover-effects.png)
Recolor menu action rows and the information area at the bottom of the Write menu. ![Write Menu Actions and Help Text preview](./images/write-write-menu-actions-and-help-text.png)

```css
[data-lab="write-menu"] [data-lab="write-option"] {
  color: #f1d9ec !important;
}
[data-lab="write-menu"] [data-lab="write-option"]:hover {
  background: #3c3050 !important;
  border-color: #b88ddd !important;
}
[data-lab="write-menu"] > div:last-child {
  background: #141b2c !important;
  border: 1px solid #645477 !important;
  border-radius: 10px !important;
  color: #b9b7d0 !important;
}
```

**Customization:** `[data-lab="write-option"]` targets the menu options. The help-text area uses a structural selector.

### Write Menu Selected, Unselected, and Keyboard-Focus States


![Write Menu selected option styling example](./images/write-write-menu-selected-options.png)
Use the tested `aria-checked` state to distinguish the active choice from inactive choices. Keyboard focus remains independently visible.

```css
[data-lab="write-menu"] [data-lab="write-option"][aria-checked="true"] {
  background: #ff79ca !important;
  color: #211b31 !important;
  outline: 2px solid #8deaff !important;
  outline-offset: -2px !important;
  border-radius: 8px !important;
}
[data-lab="write-menu"] [data-lab="write-option"][aria-checked="false"] {
  opacity: .65 !important;
}
[data-lab="write-menu"] [data-lab="write-option"]:focus-visible {
  outline: 2px solid #8deaff !important;
  outline-offset: 2px !important;
}
```

**Customization:** `aria-checked="true"` styles the selected option, while `aria-checked="false"` styles the others. `:focus-visible` adds keyboard feedback. Use this in place of the earlier selected-state example if the colors conflict.

---

### Custom Write Menu Action Icons

Replace the Write menu pencil and arrow icons with uploaded artwork. ![Custom Write Menu Action Icons preview](./images/write-custom-write-menu-action-icons.png)

```css
[data-lab="write-menu"]
[data-lab="write-option"]
img[src*="/pixel/pencil.webp"] {
  content: url("/api/images/6ac8cbcf5a1227b9442c03e1") !important;
  object-fit: contain !important;
  filter: none !important;
}
[data-lab="write-menu"]
[data-lab="write-option"]
img[src*="/pixel/arrow-right-v2.webp"] {
  content: url("/api/images/6ac896dc75e1eb8796dcf708") !important;
  object-fit: contain !important;
  transform: none !important;
  filter: none !important;
}
```

**Customization:**
- `content: url(...)` sets the replacement artwork.
- `object-fit: contain` maintains image proportions.
- `filter: none` prevents existing filters from recoloring the images.
- `transform: none` removes the arrow image’s inherited transform.

**2.5 selector note:** The updated guide uses `[data-lab="write-menu"]` and `[data-lab="write-option"]` for the Write for Me menu. Verify any older icon-specific selectors against the current menu.

---


## Search and Bookmarks

### Search & Bookmarks Panel Background

Change the main background, side border, and shadow of the shared Search and Bookmarks panel. ![Search & Bookmarks Panel Background preview](./images/panel-search-and-bookmarks-panel-background.png)

```css
:is([data-lab="search-panel"], [data-lab="bookmarks-panel"]) {
  background: #171b2b !important;
  border-left: 2px solid #73d9ff !important;
  box-shadow: -8px 0 24px #0009, inset 2px 0 0 #ff7ecb55 !important;
}
```

**Customization:** `background`, `border-left`, and `box-shadow` style both panels. Both panel hooks were verified in the live tester.

---

### Search & Bookmarks Header Styling

Customize the panel header background, divider, and shadow. ![Search & Bookmarks Header Styling preview](./images/panel-search-and-bookmarks-header-styling.png)

```css
:is([data-lab="search-panel"], [data-lab="bookmarks-panel"]) .surface-header {
  background: #29243e !important;
  border-bottom: 1px solid #ff88c7 !important;
  box-shadow: 0 4px 12px #0006 !important;
}
```

**Customization:** Change the header `background`, divider, and `box-shadow`. The `.surface-header` class was verified in both panels.

---

### Search & Bookmarks Title and Description

Recolor the panel heading and its supporting description. ![Search & Bookmarks Title and Description preview](./images/panel-search-and-bookmarks-title-and-description.png)

```css
:is([data-lab="search-panel"], [data-lab="bookmarks-panel"]) .surface-header h3 {
  color: #ffe3f4 !important;
  text-shadow: 0 0 8px #ff7fc866 !important;
}
:is([data-lab="search-panel"], [data-lab="bookmarks-panel"]) .surface-header p {
  color: #d7c5e7 !important;
}
```

**Customization:** `h3` targets the title; `p` targets the supporting description. Both were verified.

---

### Search & Bookmarks Header Icon Glow

Resize and glow the pixel-art icons in both panel headers.

```css
:is([data-lab="search-panel"], [data-lab="bookmarks-panel"]) .surface-header img {
  width: 28px !important;
  height: 28px !important;
  object-fit: contain !important;
  image-rendering: pixelated !important;
  filter: drop-shadow(0 0 5px #ff79ca) !important;
  transition: transform .2s ease !important;
}
@media (hover: hover) {
  :is([data-lab="search-panel"], [data-lab="bookmarks-panel"]) .surface-header img:hover {
    transform: scale(1.2) !important;
  }
}
```

**Tip:** This glow affects the header icons, not the search-field magnifying glass or empty-state illustration.

---

### Custom Search & Bookmarks Header Icons

Replace the large artwork beside the **Search chat** and **Bookmarks** titles. These are the **panel header icons**, not the smaller icons inside the Messages and Marked tabs. ![Search and Bookmarks header icons before and after replacement](./images/panel-custom-bookmarks-tab-icons.png)

```css
/* Search panel — header icon artwork */
[data-lab="search-panel"] .surface-header img {
  content: url("/api/images/6ac897301a947bf5aa43d1c8") !important;
  object-fit: contain !important;
  filter: none !important;
}

/* Bookmarks panel — header icon artwork */
[data-lab="bookmarks-panel"] .surface-header img {
  content: url("/api/images/6ac897231a947bf5aa43cf04") !important;
  object-fit: contain !important;
  filter: none !important;
}
```

**Customization:** Replace the sample image URLs with your own artwork. The `.surface-header img` selector changes panel header icons; [Custom Bookmarks Tab Icons](#custom-bookmarks-tab-icons) changes the Messages and Marked tab images. For glow effects, see [Search & Bookmarks Header Icon Glow](#search-bookmarks-header-icon-glow).

---

### Custom Search Bar Colors

Style the search field, typed text, cursor, placeholder, and search icon. ![Custom Search Bar Colors preview](./images/panel-custom-search-bar-colors.png)

```css
.header-search:has(
  .header-search-input:is(
    [aria-label="Search this chat"],
    [aria-label="Search marked text"]
  )
) {
  background: #202a3b !important;
  border: 1px solid #79d9ef !important;
  border-radius: 10px !important;
  box-shadow: inset 0 1px 5px #0005 !important;
}
.header-search-input:is(
    [aria-label="Search this chat"],
    [aria-label="Search marked text"]
  ) {
  background: transparent !important;
  border: none !important;
  box-shadow: none !important;
  outline: none !important;
  color: #f1eaff !important;
  caret-color: #ff8dd3 !important;
}
.header-search-input:is(
    [aria-label="Search this chat"],
    [aria-label="Search marked text"]
  )::placeholder {
  color: #a9bdd5 !important;
  opacity: 1 !important;
}
.header-search:has(
  .header-search-input:is(
    [aria-label="Search this chat"],
    [aria-label="Search marked text"]
  )
) > i.fa-search {
  color: #82e5ed !important;
  filter: drop-shadow(0 0 5px #82e5ed) !important;
}
```

**Customization:** The outer `.header-search` wrapper controls the full visible box, including the icon area. The input controls typed text, caret, and placeholder; `> i.fa-search` controls the magnifying glass. Both search variants were verified by their distinct ARIA labels. For placeholder styling, the tested `::placeholder` selector also supports `font-style: italic` and `letter-spacing: .4px` alongside `color` and `opacity`; add those declarations if desired.

---

### Search Bar Focus Effect

Highlight the search field when someone clicks or tabs into it.

```css
.header-search:has(
  .header-search-input:is(
    [aria-label="Search this chat"],
    [aria-label="Search marked text"]
  ):focus-visible
) {
  outline: 2px solid #ff92d5 !important;
  outline-offset: 2px !important;
  box-shadow: 0 0 10px #ff92d555 !important;
}
```

**Customization:** Keyboard focus on either input highlights the entire outer search box. Verified in both Search and Bookmarks.

---

### Bookmarks Tab Bar Background

Customize the container behind the Messages and Marks tabs.

```css
[data-lab="bookmarks-panel"] [role="tablist"] {
  background: #121b2c !important;
  border: 1px solid #6a83a6 !important;
  border-radius: 12px !important;
}
```

**Customization:**
- `background` changes the tab-bar backdrop.
- `border` defines its outline.

---

### Bookmarks Tab Colors


![Bookmarks Messages and Marked tab border and background comparison](./images/bookmarks-tab-border-and-background.png)
Set the normal appearance of the Messages and Marks tabs.

```css
[data-lab="bookmarks-panel"] [role="tab"] {
  color: #b5c4db !important;
  border: 1px solid transparent !important;
  border-radius: 9px !important;
  background: transparent !important;
}
```

**Customization:**
- `color` changes the tab labels.
- `background` controls the unselected fill.
- `[role="tab"]` applies the same rule to both Messages and Marked tabs.

---

### Selected Bookmarks Tab Styling


![Selected Bookmarks tab highlight comparison](./images/bookmarks-selected-tab-highlight.png)
Give the active Messages or Marks tab its own color, border, and glow.

```css
[data-lab="bookmarks-panel"] [role="tab"][aria-selected="true"] {
  color: #fff0f8 !important;
  background: #563454 !important;
  border-color: #ff8dc8 !important;
  box-shadow: inset 0 1px 0 #ffffff24, 0 0 9px #ff8dc844 !important;
}
```

**Customization:**
- `[aria-selected="true"]` targets whichever tab is currently active.
- `background` and `border-color` identify the active tab.
- `box-shadow` adds a subtle highlight and glow.

---

### Bookmarks Tab Hover and Keyboard Focus

Add separate visual feedback for mouse hover and keyboard navigation.

```css
@media (hover: hover) {
  [data-lab="bookmarks-panel"] [role="tab"]:hover {
    color: #fff0f8 !important;
    border-color: #a4a4eb !important;
  }
}
[data-lab="bookmarks-panel"] [role="tab"]:focus-visible {
  outline: 2px solid #8be8ed !important;
  outline-offset: 2px !important;
}
```

**Customization:**
- `@media (hover: hover)` limits hover styling to hover-capable devices.
- `:focus-visible` highlights keyboard focus.
- `outline-offset` adds breathing room around the focus outline.

---

### Bookmarks Tab Counters

Style the number badges independently of their tabs. The selected counter follows the active tab.

```css
[data-lab="bookmarks-panel"] [role="tab"] > span:last-child {
  background: #211b31 !important;
  color: #ff79ca !important;
  border: 1px solid #8deaff !important;
  border-radius: 999px !important;
  box-shadow: 0 0 8px #ff79ca66 !important;
}
[data-lab="bookmarks-panel"] [role="tab"][aria-selected="true"] > span:last-child {
  background: #ff79ca !important;
  color: #211b31 !important;
  border-color: #ff79ca !important;
  box-shadow: 0 0 10px #ff79ca88 !important;
}
```

**Tip:** The final direct `span` inside each tab is its counter.

---

### Bookmarks Empty-State Text

Recolor the message shown when the Bookmarks list has no saved entries.

```css
#lab-bookmarks-list > div:has(> p + p) {
  background: #171b2b !important;
  border: 2px dashed #8deaff !important;
  border-radius: 12px !important;
  padding: 16px !important;
}
#lab-bookmarks-list > div:has(> p + p) > p:first-of-type {
  color: #f3dcf4 !important;
  font-weight: 800 !important;
}
#lab-bookmarks-list > div:has(> p + p) > p:nth-of-type(2) {
  color: #b8c5dc !important;
}
```

**Customization:** These selectors style the empty-state content box and its two text lines rather than the whole panel. They depend on the empty-state HTML structure, so check them if the interface changes.

---

### Custom Search Empty-State Illustration

Replace the Search view’s default Bary illustration with uploaded artwork. ![Custom Search Empty-State Illustration preview](./images/panel-custom-search-empty-state-illustration.png)

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
- `img[src*="bary_search.webp"]` selects the Search illustration.
- `content: url(...)` replaces the image.
- `width` and `height` control its display box.
- `object-fit: contain` preserves the replacement proportions.

**Tip:** The Search empty-state illustration lives inside the shared `bookmarks-panel` wrapper. Its native image is `/img/bary/bary_search.webp`.

---

### Search & Bookmarks Close Button


![Search and Bookmarks close button styling comparison](./images/panel-search-and-bookmarks-close-button.png)
Recolor the panel’s close button and add a hover glow.

```css
:is([data-lab="search-panel"], [data-lab="bookmarks-panel"]) .surface-header button[aria-label="Close bookmarks"] {
  background: #393049 !important;
  color: #ffd8ee !important;
  border: 1px solid #d58dcb !important;
  border-radius: 8px !important;
}
@media (hover: hover) {
  :is([data-lab="search-panel"], [data-lab="bookmarks-panel"]) .surface-header button[aria-label="Close bookmarks"]:hover {
    background: #583a62 !important;
    box-shadow: 0 0 10px #ff89d266 !important;
  }
}
```

**Customization:** Both Search and Bookmarks currently use `Close bookmarks` as the close button’s ARIA label.

---

### Search & Bookmarks Footer Styling

Change the footer background, text, and top border. ![Search & Bookmarks Footer Styling preview](./images/panel-search-and-bookmarks-footer-styling.png)

```css
:is([data-lab="search-panel"], [data-lab="bookmarks-panel"]) .surface-footer {
  background: #29243e !important;
  border-top: 1px solid #74d9f0 !important;
  box-shadow: 0 -4px 12px #ff89d244 !important;
}
:is([data-lab="search-panel"], [data-lab="bookmarks-panel"]) .surface-footer > span {
  color: #d4c9e9 !important;
  font-style: italic !important;
  text-shadow: 0 0 6px #8deaff66 !important;
}
```

**Customization:** `.surface-footer` styles the strip; its direct `span` styles the message text. Change or remove `font-style` and `text-shadow` to control the optional italic/glow treatment. Tested across the displayed footer variants.

---

### Custom Copy and Download Icons

Replace the action images used to copy or download marked passages. ![Custom Copy and Download Icons preview](./images/bookmarks-copy-download-icons.png)

```css
[data-lab="bookmarks-panel"]
button[aria-label="Copy marked passages"]
img[src="/img/pixel/copy.webp"] {
  content: url("/api/images/6ac8970875e1eb8796dcfc4f") !important;
  object-fit: contain !important;
  filter: none !important;
}

[data-lab="bookmarks-panel"]
button[aria-label="Download marked passages"]
img[src="/img/pixel/download.webp"] {
  content: url("/api/images/6ac896f900c414e8e2a1bffd") !important;
  object-fit: contain !important;
  filter: none !important;
  transform: none !important;
}
```

**Customization:**
- `Copy marked passages` targets the Copy control.
- `Download marked passages` targets the Download control.
- `content: url(...)` selects the replacement artwork.
- `transform: none` prevents the Download image from inheriting an unwanted transform.

---

### Custom Search & Bookmarks Background Images


![Search and Bookmarks custom background image example](./images/search-bookmarks-image-background.png)
Optionally use uploaded artwork beneath a translucent color overlay instead of a solid panel background. 

```css
/* Optional variation: use instead of the solid panel background */
[data-lab="bookmarks-panel"] {
  background: linear-gradient(#171b2bcc, #171b2bcc),
              url("/api/images/YOUR_IMAGE_ID")
              center / cover no-repeat !important;
  border-left: 2px solid #73d9ff !important;
}

/* Optional: allow the image to show through the list area */
[data-lab="bookmarks-panel"] #lab-bookmarks-list {
  background: transparent !important;
}
```

**Customization:**
- `YOUR_IMAGE_ID` is the reader’s own uploaded image.
- `linear-gradient(...)` adds a translucent readability overlay.
- `cover` fills the panel and may crop the artwork.
- `background: transparent` allows the list area to reveal the panel artwork.

**Optional / not yet tested:** The header and footer have independent opaque backgrounds in the source theme. Keep them solid for readability or customize them separately. This example is a proposed image-background variation, not a verified finished effect.

---

### Custom Bookmarks Tab Icons

The original Messages icon is `/img/pixel/lab-bookmark.webp`; the Marked icon is `/img/pixel/lab-mark.webp`. Each tab can use different replacement artwork.

Replace the small artwork inside the **Messages** and **Marked** tabs in the Bookmarks panel. The **Marked** icon is the pencil beside the MARKED label—not the Copy or Download controls. The screenshot for the separate [header icon replacement tutorial](#custom-search-bookmarks-header-icons) does **not** show these tab icons.

```css
/* Messages tab icon */
[data-lab="bookmarks-panel"]
#lab-bookmarks-tab-messages img {
  content: url("/api/images/YOUR_MESSAGES_ICON_ID") !important;
  object-fit: contain !important;
  filter: none !important;
}

/* Marked tab icon (pencil beside MARKED) */
[data-lab="bookmarks-panel"]
#lab-bookmarks-tab-marks img {
  content: url("/api/images/YOUR_MARKED_ICON_ID") !important;
  object-fit: contain !important;
  filter: none !important;
}
```

**Customization:**
- `YOUR_MESSAGES_ICON_ID` replaces the Messages tab artwork.
- `YOUR_MARKED_ICON_ID` replaces the Marked tab artwork.
- The tab IDs target each button independently (`#lab-bookmarks-tab-messages` and `#lab-bookmarks-tab-marks`); `content` supplies your replacement artwork.
- These examples use [LoreBary-uploaded images](#how-to-import-css-images-in-lorebary). You can also use [Base64 image data](https://github.com/Caddel001/LoreBary-Theme-Snippets/blob/main/LoreBary%20CSS%20Quick%20Guide.md#converting-images-to-base64).
- Tab colors, counters, hover, and selected states have their own tutorials above. Copy and Download icon replacements are covered in [Custom Copy and Download Icons](#custom-copy-and-download-icons).

---


## Scene Notes

### Custom Scene Notes Window

Change the Scene Notes window background, outline, corners, and shadow. ![Custom Scene Notes Window preview](./images/panel-custom-scene-notes-window.png)

```css
[data-lab="input"] > div:has(#lab-scene-notes) {
  background: #211b31 !important;
  border: 1px solid #ee8ec9 !important;
  border-radius: 16px !important;
  box-shadow: 0 0 14px #ed83c32b, 0 12px 32px #00000080 !important;
}
```

**Customization:** The verified Scene Notes panel selector replaces the older label-wrapper traversal. Change `background`, `border`, `border-radius`, and `box-shadow` to customize the window.

---

### Scene Notes Title and Close Button


![Scene Notes close button styling comparison](./images/scene-notes-close-button.png)
Recolor the Scene Notes title and close button.

```css
[data-lab="input"] > div:has(#lab-scene-notes)
label[for="lab-scene-notes"] {
  color: #ffd5ec !important;
  text-shadow: 0 0 7px #f98ac566 !important;
}
[data-lab="input"] > div:has(#lab-scene-notes)
label[for="lab-scene-notes"] + button {
  background: #49304f !important;
  color: #ffc5e6 !important;
  border: 1px solid #dc85c3 !important;
}
```

**Customization:** Style the Scene Notes heading and its close button independently. The close button follows the heading in the current panel layout and also has `aria-label="Close scene notes"`.

---

### Scene Notes Template Colors

Assign different accent colors to the eight Scene Notes templates and their icon frames. ![Scene Notes Template Colors preview](./images/panel-scene-notes-template-colors.png)

```css
[aria-label="Scene note templates"]
button {
  color: #d8cbe2 !important;
}
[aria-label="Scene note templates"]
button > span:first-child {
  background: #302b42 !important;
  border: 1px solid #7f719d !important;
  box-shadow: 0 2px 6px #0006 !important;
}
[aria-label="Select Talk more template"] {
  --note-color: #ff89b7;
}
[aria-label="Select Stay real template"] {
  --note-color: #ffc38b;
}
[aria-label="Select Living world template"] {
  --note-color: #f6df83;
}
[aria-label="Select Your move template"] {
  --note-color: #88e5b1;
}
[aria-label="Select Slow burn template"] {
  --note-color: #80dfff;
}
[aria-label="Select Romance template"] {
  --note-color: #b99aff;
}
[aria-label="Select Sex template"] {
  --note-color: #f39bdf;
}
[aria-label="Select Kink template"] {
  --note-color: #ff9a9f;
}
[aria-label="Scene note templates"]
button > span:first-child {
  border-color: var(--note-color, #7f719d) !important;
}
```

**Customization:**
- `--note-color` is the accent color assigned to each template.
- `button > span:first-child` styles the template icon frame.
- Change individual hex values to build your own palette.

---

### Scene Notes Selected and Hover Effects

Give the selected Scene Notes template a clearly visible pink glow and a slight enlargement, with a separate hover highlight for other templates. ![Scene Notes Selected and Hover Effects preview](./images/panel-scene-notes-selected-and-hover-effects.png)

```css
/* Selected template — confirmed working */
[aria-label="Scene note templates"]
button[aria-pressed="true"] > span:first-child {
  background: #674467 !important;
  border: 2px solid #ff89b7 !important;
  box-shadow:
    0 0 0 2px #ff89b755,
    0 0 12px 4px #ff89b7aa,
    0 0 22px #ff89b766 !important;
  transform: scale(1.08) !important;
}

/* Hover over templates that are not selected */
@media (hover: hover) {
  [aria-label="Scene note templates"]
  button:not([aria-pressed="true"]):hover > span:first-child {
    background: #3a304d !important;
    box-shadow: 0 0 9px var(--note-color, #ff89b7) !important;
  }
}
```

**Customization:**
- `[aria-pressed="true"]` identifies the selected template.
- `#674467` sets the selected icon circle's background; `#ff89b7` is the selected border color.
- The three `box-shadow` layers create a visible pink ring and glow. Reduce their blur, spread, or opacity for a softer effect.
- `scale(1.08)` enlarges the selected circle slightly; use `scale(1)` to remove the enlargement.
- The hover rule uses each template's `--note-color` when **Scene Notes Template Colors** is also installed, with pink as a fallback.
- `:not([aria-pressed="true"])` keeps hover styling from overriding the selected appearance.

**Tip:** The hover adjustment keeps the selected glow visible while the pointer is over a template.

---

### Scene Notes Text Box Colors and Focus

Customize the Scene Notes text area, placeholder, and focused appearance. ![Scene Notes Text Box Colors and Focus preview](./images/panel-scene-notes-text-box-colors-and-focus.png)

```css
[data-lab="input"] #lab-scene-notes {
  background: #121b2b !important;
  color: #f3e7f6 !important;
  border: 1px solid #6bcde5 !important;
  border-radius: 12px !important;
  box-shadow: inset 0 2px 6px #0007 !important;
}
[data-lab="input"] #lab-scene-notes::placeholder {
  color: #a9b8ce !important;
}
[data-lab="input"] #lab-scene-notes:focus-visible {
  outline: 2px solid #ff92d0 !important;
  outline-offset: 2px !important;
}
```

**Customization:**
- `background` and `color` set the editor colors.
- `::placeholder` styles the hint text.
- `:focus-visible` shows the focus outline when the browser determines a visible focus indicator is needed.

---

### Scene Notes Additional Buttons


![Scene Notes Apply to dropdown styling comparison](./images/scene-notes-apply-to-dropdown.png)
Recolor the saved-template button and the Apply To control, including its hover state. 

```css
[data-lab="input"] > div:has(#lab-scene-notes)
button[aria-label="Open saved scene note templates"] {
  background: #453457 !important;
  border: 1px solid #c49bff !important;
  color: #f0cfff !important;
  border-radius: 50% !important;
}
@media (hover: hover) {
  [data-lab="input"] > div:has(#lab-scene-notes)
  button[aria-label="Open saved scene note templates"]:hover {
    background: #674467 !important;
  }
}
/* Apply To dropdown: inspected structure, verified live */
[data-lab="input"] > div:has(#lab-scene-notes)
div:has(> #lab-scene-notes) ~ div button {
  background: #121b2b !important;
  border: 1px solid #846aa9 !important;
  color: #e8d7f2 !important;
  border-radius: 12px !important;
}
```

**Customization:** Use the lightbulb button selector to style its appearance. The Apply To dropdown uses a structural selector in this example; its `aria-label="Apply to"` can also be used for more direct targeting.

---

### Scene Notes Keyboard Focus

Give Scene Notes controls a visible keyboard-focus outline.

```css
[aria-label="Scene note templates"] button:focus-visible,
[data-lab="input"] > div:has(#lab-scene-notes) button[aria-label="Apply to"]:focus-visible,
[data-lab="input"] > div:has(#lab-scene-notes) button[aria-label="Close scene notes"]:focus-visible {
  outline: 2px solid #ff92d0 !important;
  outline-offset: 2px !important;
}
```

**Customization:**
- `focus-visible` shows the outline during keyboard navigation.
- `outline-offset` creates space between the outline and control.

---

### Custom Scene Notes Template Icons

The eight native template icons are `scene-talk-more.webp`, `scene-stay-real.webp`, `scene-living-world.webp`, `scene-your-move.webp`, `scene-slow-burn.webp`, `scene-romance.webp`, `scene-intimacy.webp` (Sex), and `scene-kink.webp`, all under `/img/pixel/`.

Replace the artwork for all eight Scene Notes templates. ![Custom Scene Notes Template Icons preview](./images/panel-custom-scene-notes-template-icons.png)

```css
[aria-label="Select Talk more template"] img {
  content: url("/api/images/6ac933d9774248b6e840f548") !important;
  object-fit: contain !important;
}
[aria-label="Select Stay real template"] img {
  content: url("/api/images/6ac933bc774248b6e840f1a4") !important;
  object-fit: contain !important;
}
[aria-label="Select Living world template"] img {
  content: url("/api/images/6ac9337f71408e65b12b8235") !important;
  object-fit: contain !important;
}
[aria-label="Select Your move template"] img {
  content: url("/api/images/6ac9339a774248b6e840ec7c") !important;
  object-fit: contain !important;
}
[aria-label="Select Slow burn template"] img {
  content: url("/api/images/6ac933e874200038737ef983") !important;
  object-fit: contain !important;
}
[aria-label="Select Romance template"] img {
  content: url("/api/images/6ac933a88825371476f13213") !important;
  object-fit: contain !important;
}
[aria-label="Select Sex template"] img {
  content: url("/api/images/6ac93403041fbd15cfcc8e14") !important;
  object-fit: contain !important;
}
[aria-label="Select Kink template"] img {
  content: url("/api/images/6ac933f742849615a40a8ab3") !important;
  object-fit: contain !important;
}
```

**Customization:**
- Each `aria-label` selects one template.
- `content: url(...)` replaces its icon.
- Replace each `/api/images/...` address with your own uploaded image URL.

---
## Multiplayer

Multiplayer sessions introduce participant portraits, player-specific author names, session notifications, message reactions, and a separate player-chat window. These elements can be customized independently of the standard Laboratory interface.

### Multiplayer Island Background and Controls

The Multiplayer Island appears near the top of the Laboratory. It contains the multiplayer icon, participant portraits, session status, and Summon or Stop button.

```css
/* Multiplayer island */
[data-lab="mp-island"] {
  background: #29243e ;
  border: 2px solid #8deaff !important;
  border-radius: 999px ;
  box-shadow: 0 3px 12px #0006, 0 0 10px #ff79ca33 !important;
}

/* Multiplayer label */
[data-lab="mp-island"] > span:first-child,
[data-lab="mp-island"] > span:first-child span {
  color: #ffe17b ;
  font-weight: 800 ;
}

/* Internal divider */
[data-lab="mp-island"] > span:nth-child(2) {
  background: #8deaff ;
}

/* Session status */
[data-lab="mp-island"] > span:nth-last-of-type(1) {
  color: #8deaff ;
  font-weight: 700 ;
  opacity: 1 ;
}

/* Summon / Stop button */
[data-lab="mp-island"] > button:last-child {
  background: #171b2b ;
  border: 1px solid #ff79ca ;
  border-radius: 999px ;
  color: #ff79ca ;
}

/* Summon / Stop button text */
[data-lab="mp-island"] > button:last-child span {
  color: #ff79ca ;
  font-weight: 800 ;
}

/* Button hover */
@media (hover: hover) {
  [data-lab="mp-island"] > button:last-child:hover {
    background: #453457 ;
    border-color: #ffe17b ;
  }
}
```

**Customization:**
- `background` changes the island's main surface.
- `border` and `box-shadow` control its outline and glow.
- `span:first-child` targets the Multiplayer label.
- `span:nth-child(2)` styles the internal divider.
- `span:nth-last-of-type(1)` styles the session status.
- `button:last-child` targets the Summon or Stop control.

---

### Multiplayer Icon Recoloring

The Multiplayer Island uses the native image `/img/pixel/multiplayer.webp`. Recolor it without changing the surrounding island.

```css
[data-lab="mp-island"] img[src="/img/pixel/multiplayer.webp"] {
  filter: brightness(0) invert(1) ;
  opacity: 1 ;
}
```

**Customization:**
- `filter` changes the icon's appearance; the example produces white artwork.
- `opacity: 1` keeps the icon fully visible.
- Replace the filter with a different combination to create a colored tint.

---

### Custom Multiplayer Icon

Replace the Multiplayer Island icon with your own uploaded artwork.

```css
[data-lab="mp-island"] img[src="/img/pixel/multiplayer.webp"] {
  content: url("/api/images/YOUR_IMAGE_ID") ;
  object-fit: contain ;
  filter: none ;
}
```

**Customization:**
- `YOUR_IMAGE_ID` is the path of your uploaded artwork.
- `content: url(...)` replaces the native image.
- `filter: none` preserves the colors of your replacement.
- `object-fit: contain` maintains its proportions.

---

### Multiplayer Participant Avatars

Multiplayer participant portraits appear together inside the island. Their frames can be styled separately from the avatars beside ordinary chat messages.

```css
/* Participant avatar frames */
[data-lab="avatar"][style*="rgba("]:not(
  [data-lab="message"] [data-lab="avatar"]
) {
  background: #29243e !important;
  border: 3px solid #8deaff ;
  border-radius: 50% ;
  outline: 2px solid #ff79ca ;
  box-shadow: 0 0 10px #ff79ca55 ;
}

/* Participant portrait images */
[data-lab="avatar"][style*="rgba("]:not(
  [data-lab="message"] [data-lab="avatar"]
) img {
  border-radius: 50% ;
  outline: 1px solid #ffe17b ;
}
```

**Customization:**
- `background` changes the portrait frame's backing.
- `border` creates the inner outline.
- `outline` adds a second decorative ring.
- `box-shadow` produces a glow around the avatar.
- The nested `img` rule styles the portrait image itself.

---

### Multiplayer Author Names

Multiplayer messages display participant names through `[data-lab="mp-author"]`.

Recolor the author name and its clickable identity control.

```css
/* Multiplayer author name */
[data-lab="mp-author"] {
  color: #ff79ca ;
  font-weight: 800 ;
  text-shadow: 0 0 6px #ff79ca66 ;
}

/* Clickable player identity */
[data-lab="mp-author"] button[data-lab="identity"] {
  color: #8deaff ;
  font-weight: 800 ;
  text-shadow: 0 0 5px #8deaff55 ;
}
```

**Customization:**
- `[data-lab="mp-author"]` styles multiplayer author names.
- `button[data-lab="identity"]` targets the clickable player identity.
- `color` overrides individual author colors with a shared theme color.
- `text-shadow` adds a subtle glow.

---

### Multiplayer Session Notification Cards

Multiplayer notifications announce events such as participants joining or changing their personas.

Customize the notification card, text, avatar frame, and separator lines.

```css
/* Notification card */
[data-lab="divider"] > div:nth-child(2) > div {
  background: #29243e ;
  border: 2px solid #8deaff !important;
  border-radius: 14px ;
  box-shadow: 0 3px 12px #0005 ;
}

/* Notification text */
[data-lab="divider"] > div:nth-child(2) p,
[data-lab="divider"] > div:nth-child(2) p span {
  color: #ffe3f4 ;
}

/* Notification avatar frame */
[data-lab="divider"] > div:nth-child(2) .rounded-full {
  background: #453457 ;
  border: 2px solid #ff79ca !important;
}

/* Separator lines */
[data-lab="divider"] > div:first-child,
[data-lab="divider"] > div:last-child {
  background: #b49aff ;
}
```

**Customization:**
- `[data-lab="divider"]` identifies the notification row.
- `div:nth-child(2) > div` styles the notification card.
- `p` and `p span` recolor its message text.
- `.rounded-full` targets the notification's circular avatar frame.
- `div:first-child` and `div:last-child` style the decorative separator lines.

---

### Multiplayer Notification Delete Button

The notification's Delete button can be styled separately from ordinary message deletion controls.

```css
/* Notification delete button */
[data-lab="divider"] button[aria-label="Delete"] {
  background: #211b31 ;
  border: 1px solid #ff79ca ;
  border-radius: 50% ;
}

/* Delete icon */
[data-lab="divider"] button[aria-label="Delete"] img {
  filter: brightness(0) invert(1) ;
}
```

**Customization:**
- `background` changes the delete button's fill.
- `border` sets its outline color.
- `border-radius: 50%` keeps the control circular.
- `filter` recolors the icon independently.

---

### Multiplayer Message Reaction Button

Messages can display a reaction control using a Font Awesome icon.

```css
/* Reaction button */
[data-lab="message"] button[aria-label="React to message"] {
  background: #211b31 ;
  border: 2px solid #ff79ca ;
  border-radius: 50% ;
  color: #ffe17b ;
  box-shadow: 0 0 8px #ff79ca44 ;
}

/* Reaction icon */
[data-lab="message"] button[aria-label="React to message"] i {
  color: #ffe17b ;
}
```

**Customization:**
- `button[aria-label="React to message"]` targets the reaction control.
- `background` and `border` style the button.
- The nested `i` selector recolors the Font Awesome icon.
- `box-shadow` adds a soft glow.

---

### Multiplayer Reaction Counters

When a message has reactions, a separate counter displays its reaction information.

```css
/* Reaction counter */
[data-lab="message"] button[aria-label*="reactions. View who reacted"] {
  background: #453457 ;
  border: 1px solid #8deaff !important;
  border-radius: 999px ;
  box-shadow: 0 0 8px #8deaff33 ;
}

/* Reaction count */
[data-lab="message"] button[aria-label*="reactions. View who reacted"] > span:last-child {
  color: #ffe17b ;
  font-weight: 800 ;
}
```

**Customization:**
- `[aria-label*="reactions. View who reacted"]` selects reaction counters.
- `background` styles the counter's surface.
- `border-radius: 999px` produces a pill shape.
- `span:last-child` targets the reaction count label.

---

### Floating Player-Chat Toggle

The floating Player Chat button opens or hides the conversation shared between multiplayer participants.

```css
/* Player-chat toggle */
button:is(
  [aria-label="Open player chat"],
  [aria-label="Hide player chat"]
) {
  background: #211b31 ;
  border: 2px solid #8deaff ;
  border-radius: 50% ;
  box-shadow: 0 0 10px #8deaff55 ;
}

/* Toggle icon */
button:is(
  [aria-label="Open player chat"],
  [aria-label="Hide player chat"]
) img {
  filter: brightness(0) invert(1) ;
  opacity: 1 ;
}
```

**Customization:**
- Both ARIA labels are included so the styling remains consistent when the chat is opened or hidden.
- `background` changes the button's surface.
- `border` and `box-shadow` provide the accent.
- The nested `img` selector recolors the toggle icon.

---

### Player-Chat Window Background and Header

The floating Player Chat window has its own header, conversation area, and lower controls.

```css
/* Player-chat window */
.home-widgets.surface-post:has(button[aria-label="Close player chat"]) {
  background: #211b31 ;
  border: 2px solid #b49aff ;
  border-radius: 16px ;
  box-shadow: 0 10px 26px #0008 ;
}

/* Window header */
.home-widgets.surface-post:has(button[aria-label="Close player chat"]) > div:first-child {
  background: #453457 ;
  border-bottom: 1px solid #ff79ca ;
}

/* Header text */
.home-widgets.surface-post:has(button[aria-label="Close player chat"]) > div:first-child * {
  color: #ffe3f4 ;
}

/* Conversation and lower surfaces */
.home-widgets.surface-post:has(button[aria-label="Close player chat"]) > div:not(:first-child) {
  background-color: #211b31 ;
}
```

**Customization:**
- `.home-widgets.surface-post:has(...)` targets the floating Player Chat window.
- `background` changes the main window color.
- `border` and `box-shadow` style its outer frame.
- `div:first-child` targets the header.
- `div:not(:first-child)` styles the remaining direct window sections.

---

### Player-Chat Text and Buttons

Recolor the text and buttons inside the floating Player Chat window.

```css
/* Player-chat text */
.home-widgets.surface-post:has(button[aria-label="Close player chat"]) p,
.home-widgets.surface-post:has(button[aria-label="Close player chat"]) span {
  color: #e8d7f2 ;
}

/* Player-chat buttons */
.home-widgets.surface-post:has(button[aria-label="Close player chat"]) button {
  background: #453457 ;
  border: 1px solid #8deaff ;
  border-radius: 10px ;
  color: #ffe3f4 ;
}
```

**Customization:**
- `p` and `span` recolor text inside Player Chat.
- `button` styles the window's interactive controls.
- `background`, `border`, and `color` can be adjusted independently.

**Compatibility:** These are shared styles for the entire Player Chat window. More specific button and bubble rules can be added afterward for individual elements.

---

### Player-Chat Message Bubbles

Player Chat uses left- and right-aligned message bubbles. Give each side a different background, border, and decorative tail.

```css
/* Left-aligned message bubble */
.home-widgets.surface-post:has(button[aria-label="Close player chat"])
.flex.flex-col.items-start > div.relative.max-w-\[85\%\] {
  background: #30243f !important;
  border: 1px solid #8deaff !important;
  border-radius: 4px 14px 14px 14px ;
  color: #ffe3f4 ;
  box-shadow: 0 2px 8px #0005 !important;
}

/* Left bubble tail */
.home-widgets.surface-post:has(button[aria-label="Close player chat"])
.flex.flex-col.items-start > div.relative.max-w-\[85\%\]
> svg[data-lab="bubble-tail"] {
  fill: #30243f ;
}

/* Right-aligned message bubble */
.home-widgets.surface-post:has(button[aria-label="Close player chat"])
.flex.flex-col.items-end > div.relative.max-w-\[85\%\] {
  background: #49304f !important;
  border: 1px solid #ff79ca !important;
  border-radius: 14px 4px 14px 14px ;
  color: #ffe3f4 ;
  box-shadow: 0 2px 8px #0005 ;
}

/* Right bubble tail */
.home-widgets.surface-post:has(button[aria-label="Close player chat"])
.flex.flex-col.items-end > div.relative.max-w-\[85\%\]
> svg[data-lab="bubble-tail"] {
  fill: #49304f !important;
  
}
```

**Customization:**
- `.items-start` identifies left-aligned messages.
- `.items-end` identifies right-aligned messages.
- `background` sets each bubble's color.
- `border-radius` creates the different left and right bubble shapes.
- `svg[data-lab="bubble-tail"]` styles each bubble's decorative pointer.
- Keep each tail's `fill` matched to its bubble's `background` for a seamless appearance.

---

### Player-Chat Composer

Customize the Player Chat text field, typed text, cursor, and placeholder.

```css
/* Player-chat text input */
.home-widgets.surface-post:has(button[aria-label="Close player chat"]) textarea {
  background: #171b2b ;
  border: 1px solid #8deaff ;
  border-radius: 10px ;
  color: #ffe3f4 ;
  caret-color: #ff79ca ;
}

/* Input placeholder */
.home-widgets.surface-post:has(button[aria-label="Close player chat"]) textarea::placeholder {
  color: #b8a9cc ;
  opacity: 1 ;
}
```

**Customization:**
- `background` changes the text field's fill.
- `border` sets the input outline.
- `color` controls typed text.
- `caret-color` recolors the typing cursor.
- `::placeholder` styles the text shown before typing.

---

### Player-Chat Images, GIFs, and Stickers

Add decorative frames to images shared through Player Chat.

```css
.home-widgets.surface-post:has(button[aria-label="Close player chat"]) img {
  border: 2px solid #8deaff ;
  border-radius: 12px ;
  box-shadow: 0 0 8px #ff79ca44 ;
}
```

**Customization:**
- `border` frames the image.
- `border-radius` rounds its corners.
- `box-shadow` creates a colored glow.
- Change the border width or shadow intensity to make media decorations more or less prominent.

**Note:** This rule affects images throughout the Player Chat window, including interface artwork. For media-only decoration, narrow the selector to the image container you want to customize.

---

## Universes

LoreBary's Universes feature includes a dedicated sidebar, universe selection controls, an in-chat clock, a minimap, and a recall button. Each component can be customized independently to match your Laboratory theme.

### Universe Sidebar Background and Header

Customize the Universe sidebar's background, border, shadow, and header.

```css
/* Universe sidebar */
[data-lab="universe-panel"] {
  background: #211b31 ;
  border-left: 2px solid #b49aff ;
  color: #ffe3f4 ;
  box-shadow: -8px 0 30px #0006 ;
}

/* Sidebar header */
[data-lab="universe-panel"] > div > div:first-child {
  background: #453457 ;
  border-bottom: 1px solid #b49aff ;
  box-shadow: 0 4px 12px #0003 ;
}
```

**Customization:**
- `background` sets the sidebar's main surface.
- `border-left` adds an accent along the sidebar edge.
- `box-shadow` creates depth between the sidebar and chat.
- The second selector styles the header area independently.

---

### Universe Sidebar Titles and Text

Recolor the Universe sidebar's headings, descriptions, and secondary labels.

```css
/* Headings */
[data-lab="universe-panel"] h3 {
  color: #ffe3f4 ;
  font-family: Georgia, serif ;
  letter-spacing: .04em ;
}

/* Descriptions */
[data-lab="universe-panel"] p {
  color: #d1bddf ;
}

/* Secondary labels */
[data-lab="universe-panel"] :is(
  .text-slate-400,
  .text-slate-500
) {
  color: #c5afd4 ;
}
```

**Customization:**
- `h3` styles section headings.
- `p` recolors descriptive text.
- `.text-slate-400` and `.text-slate-500` target additional muted labels.
- `font-family` and `letter-spacing` can give the headings a different personality.

---

### Universe Selection Radio Buttons

Universes use a radio group to display selectable options. Style the group, unselected buttons, and selected option independently.

```css
/* Radio group container */
[data-lab="universe-panel"] [role="radiogroup"] {
  background: #171b2b ;
  border: 1px solid #b49aff ;
  border-radius: 12px ;
}

/* Unselected options */
[data-lab="universe-panel"] [role="radio"] {
  color: #d1bddf ;
  border: 1px solid transparent ;
  border-radius: 10px ;
}

/* Selected option */
[data-lab="universe-panel"] [role="radio"][aria-checked="true"] {
  background: #ffb36b ;
  color: #211b31 ;
  border-color: #ffb36b ;
  box-shadow: 0 2px 8px #0003 ;
}
```

**Customization:**
- `[role="radiogroup"]` styles the container around the options.
- `[role="radio"]` targets individual options.
- `[aria-checked="true"]` identifies the selected option.
- `background` and `color` distinguish the active selection.

---

### Universe Cards and Content Panels

Recolor the smaller content panels displayed inside the Universe sidebar.

```css
[data-lab="universe-panel"] .surface-post {
  background: #30243f ;
  border: 1px solid #b49aff ;
  border-radius: 12px ;
  box-shadow: 0 3px 10px #0003 ;
}
```

**Customization:**
- `.surface-post` targets the sidebar's internal content surfaces.
- `background` changes the card fill.
- `border` defines its outline.
- `border-radius` and `box-shadow` control its shape and depth.

---

### Universe Input Fields and Dropdowns

Customize text inputs, text areas, and dropdown menus inside the Universe sidebar.

```css
/* Input fields */
[data-lab="universe-panel"] :is(input, textarea, select) {
  background: #171b2b ;
  border: 1px solid #b49aff ;
  border-radius: 8px ;
  color: #ffe3f4 ;
  caret-color: #ff79ca ;
}

/* Placeholder text */
[data-lab="universe-panel"] :is(input, textarea)::placeholder {
  color: #c5afd4 ;
  opacity: .8 ;
}

/* Focused fields */
[data-lab="universe-panel"] :is(input, textarea):focus {
  outline: 2px solid #ffb36b ;
  outline-offset: 1px ;
}
```

**Customization:**
- `input`, `textarea`, and `select` share the same field colors.
- `color` controls typed text.
- `caret-color` recolors the typing cursor.
- `::placeholder` changes the hint text.
- `:focus` highlights an active text field.

---

### Universe Buttons and Icons

Style the sidebar's regular buttons and recolor its Font Awesome and pixel-art icons.

```css
/* Regular buttons */
[data-lab="universe-panel"] button:not([role="radio"]) {
  border-color: #b49aff ;
  color: #ffe3f4 ;
}

/* Font Awesome icons */
[data-lab="universe-panel"] i {
  color: #ffb36b ;
}

/* Pixel-art icons */
[data-lab="universe-panel"] img[src^="/img/pixel/"] {
  filter: sepia(1) saturate(2) hue-rotate(330deg) ;
}

/* Hover */
@media (hover: hover) {
  [data-lab="universe-panel"] button:not([role="radio"]):hover {
    filter: brightness(1.15) ;
  }
}
```

**Customization:**
- `button:not([role="radio"])` styles regular controls without changing the radio selections.
- `i` recolors Font Awesome icons.
- `img[src^="/img/pixel/"]` targets native pixel-art images.
- `filter` changes their tint.
- `brightness(1.15)` makes buttons slightly brighter on hover.

---

### Universe Header Badge

Recolor the small badge displayed in the Universe sidebar's header.

```css
[data-lab="universe-panel"] .surface-header > span.rounded-md {
  background: #453457 ;
  border: 1px solid #b49aff ;
  border-radius: 8px ;
  color: #ffb36b ;
  box-shadow: inset 0 1px 2px #0003 ;
}
```

**Customization:**
- `background` sets the badge fill.
- `border` creates its outline.
- `color` changes the badge text.
- `box-shadow` adds subtle inner depth.

---

### Universe Pills and Tags

Customize the small pill-shaped controls used inside the Universe sidebar.

```css
/* Universe pills */
[data-lab="universe-panel"] .group\/pill {
  background: #453457 ;
  border: 1px solid #b49aff ;
  border-radius: 999px ;
  color: #ffe3f4 ;
  box-shadow: 0 2px 4px #0003 ;
}

/* Pill buttons and icons */
[data-lab="universe-panel"] .group\/pill button,
[data-lab="universe-panel"] .group\/pill button i {
  color: #ffb36b ;
}

/* Hover */
@media (hover: hover) {
  [data-lab="universe-panel"] .group\/pill:hover {
    background: #30243f ;
    border-color: #ffb36b ;
  }
}
```

**Customization:**
- `.group\/pill` targets the pill container.
- `background` and `border` define its appearance.
- The nested button and icon selectors style its controls.
- `border-radius: 999px` maintains the rounded pill shape.

---

### Universe Additional Input Controls

Some Universe controls use the `data-no-haptic` attribute. These can be styled separately from the regular inputs.

```css
[data-lab="universe-panel"] [data-no-haptic] {
  background: #171b2b ;
  border: 1px solid #b49aff ;
  border-radius: 10px ;
}

/* Active input group */
[data-lab="universe-panel"] [data-no-haptic]:focus-within {
  border-color: #ffb36b ;
}
```

**Customization:**
- `[data-no-haptic]` targets the additional control.
- `background` and `border` style its surface.
- `:focus-within` highlights the container when an internal input receives focus.

---

### Universe Clock

The Universe Clock appears in the chat interface and can be styled independently from the sidebar.

```css
/* Clock container */
[data-lab="universe-clock"] {
  background: #211b31 ;
  border: 1px solid #ffb36b ;
  border-top: 0 ;
  color: #ffe3f4 ;
  box-shadow: 0 3px 10px #0006 ;
}

/* Clock icon */
[data-lab="universe-clock"] img {
  filter: sepia(1) saturate(2) hue-rotate(330deg) ;
  opacity: 1 ;
}

/* Clock labels */
[data-lab="universe-clock"] span {
  color: #d1bddf ;
}

/* First clock label */
[data-lab="universe-clock"] span:first-of-type {
  color: #ffe17b ;
  font-weight: 800 ;
}

/* Final clock label */
[data-lab="universe-clock"] span:last-child {
  color: #8deaff ;
}

/* Hover */
@media (hover: hover) {
  [data-lab="universe-clock"]:hover {
    background: #453457 ;
  }
}
```

**Customization:**
- `background` changes the clock's surface.
- `border` sets its outline.
- `border-top: 0` removes the upper border.
- `img` styles the clock icon.
- `span:first-of-type` and `span:last-child` allow different text accents.
- The hover rule changes the clock's background when the pointer is over it.

---

### Universe Minimap

The Universe Minimap can be styled with a gradient border, shadow, and colored badge.

```css
/* Minimap container */
[data-lab="universe-minimap"] {
  border: 3px solid transparent ;
  border-radius: 14px ;
  background:
    linear-gradient(#171b2b, #171b2b) padding-box,
    linear-gradient(135deg, #ff79ca, #ffe17b, #8deaff, #b49aff) border-box ;
  box-shadow: 0 4px 16px #0009, 0 0 12px #b49aff55 ;
}

/* Minimap badge */
[data-lab="universe-minimap"] > span:last-child {
  background: #211b31 ;
  border: 1px solid #b49aff ;
  color: #ffe17b ;
  box-shadow: 0 0 7px #b49aff55 ;
}

/* Hover glow */
@media (hover: hover) {
  [data-lab="universe-minimap"]:hover {
    box-shadow: 0 4px 18px #000a, 0 0 18px #8deaff88 ;
  }
}
```

**Customization:**
- `border: 3px solid transparent` makes room for the gradient outline.
- The first gradient paints the interior.
- The second gradient paints the border.
- `span:last-child` styles the minimap's badge.
- `box-shadow` adds a decorative glow.

---

### Universe Recall Button

The Universe Recall button can have its own pill-shaped appearance, icon tint, and hover treatment.

```css
/* Recall button */
[data-lab="universe-recall"] {
  background: #171b2b ;
  border: 1px solid #b49aff ;
  border-radius: 999px ;
  padding: 3px 7px ;
  color: #ffe17b ;
  box-shadow: 0 0 8px #b49aff33 ;
}

/* Recall icon */
[data-lab="universe-recall"] img {
  filter: sepia(1) saturate(2) hue-rotate(135deg) ;
  opacity: 1 ;
}

/* Recall text */
[data-lab="universe-recall"] span {
  color: #ffe17b ;
  font-weight: 800 ;
}

/* Hover */
@media (hover: hover) {
  [data-lab="universe-recall"]:hover {
    background: #453457 ;
    border-color: #8deaff ;
  }
}
```

**Customization:**
- `background` sets the Recall button's fill.
- `border` controls its outline.
- `border-radius: 999px` creates the pill shape.
- `padding` adjusts the spacing around its contents.
- `img` styles the Recall icon.
- `span` recolors and emphasizes the button text.

---

## Pinned Scenes

Pinned Scenes display saved moments inside the Laboratory chat. Their appearance includes a decorative card, tape artwork, a scene preview, and an Unpin control.

Each element can be customized independently.

### Pinned Scene Card

Use `[data-lab="scene-pin"]` to customize the pinned scene's main card.

```css
/* Pinned Scene card */
[data-lab="scene-pin"] > div > div.relative.p-1\.5 {
  background: #29243e !important;
  border: 2px solid #b49aff !important;
  border-radius: 12px;
  box-shadow: 0 4px 16px #0006;
}
```

**Customization:**

- `background` changes the card's surface.
- `border` controls its outline.
- `border-radius` adjusts the corners.
- `box-shadow` creates depth beneath the card.

---

### Pinned Scene Decorative Tape

Pinned Scenes use decorative tape artwork that can be recolored independently of the card.

```css
/* Pinned Scene tape */
[data-lab="scene-pin"] img[src="/img/sketch/tape_plain.webp"] {
  filter:
    grayscale(1)
    sepia(1)
    saturate(3)
    hue-rotate(285deg)
    brightness(1.12)
    drop-shadow(0 2px 3px #0008);
}
```

**Customization:**

- `grayscale()` removes the original colors.
- `sepia()` and `saturate()` prepare the image for recoloring.
- `hue-rotate()` changes the tape's tint.
- `brightness()` adjusts its lightness.
- `drop-shadow()` adds depth beneath the artwork.

---

### Custom Pinned Scene Tape

Replace the native tape with your own uploaded artwork.

```css
/* Custom Pinned Scene tape */
[data-lab="scene-pin"] img[src="/img/sketch/tape_plain.webp"] {
  content: url("/api/images/YOUR_IMAGE_ID");
  object-fit: contain;
  filter: none;
}
```

**Customization:**

- Replace `YOUR_IMAGE_ID` with your uploaded artwork's path.
- `content: url(...)` replaces the original tape image.
- `object-fit: contain` preserves the replacement's proportions.
- `filter: none` displays the artwork's original colors.

---

### Pinned Scene Unpin Button

The Unpin control can be styled independently from the other Laboratory message actions.

```css
/* Unpin button */
[data-lab="scene-pin"] button[aria-label="Unpin scene"] {
  background: #171421;
  border: 1px solid #ff548d;
  border-radius: 9px;
  color: #ff548d;
}

/* Unpin icon */
[data-lab="scene-pin"] button[aria-label="Unpin scene"] img {
  filter:
    grayscale(1)
    sepia(1)
    saturate(3)
    hue-rotate(285deg)
    brightness(1.12);
}
```

**Customization:**

- `background` changes the Unpin button's surface.
- `border` sets its outline.
- `border-radius` adjusts its corners.
- `color` changes the button's text color.
- The nested `img` selector recolors its icon.

---

