---
name: BizFlow
description: A clear, capable work-order ledger for independent businesses.
colors:
  navy: "#14243a"
  ink: "#17263b"
  ink-soft: "#41536b"
  muted: "#64748b"
  paper: "#ffffff"
  canvas: "#f2f5f8"
  line: "#dce3eb"
  blue: "#275ee8"
  blue-dark: "#1849ca"
  blue-pale: "#e9efff"
  lime: "#d9f36a"
  lime-ink: "#34420b"
  green: "#187c52"
  green-pale: "#e8f6ee"
  red: "#b5413e"
  red-pale: "#fff0ef"
typography:
  display:
    fontFamily: '"Segoe UI", "Helvetica Neue", Arial, sans-serif'
    fontSize: "clamp(29px, 3.2vw, 43px)"
    fontWeight: 780
    lineHeight: 1.08
    letterSpacing: "-0.055em"
  title:
    fontFamily: '"Segoe UI", "Helvetica Neue", Arial, sans-serif'
    fontSize: "22px"
    fontWeight: 760
    letterSpacing: "-0.04em"
  body:
    fontFamily: '"Segoe UI", "Helvetica Neue", Arial, sans-serif'
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: '"Segoe UI", "Helvetica Neue", Arial, sans-serif'
    fontSize: "10px"
    fontWeight: 800
    letterSpacing: "0.13em"
rounded:
  sm: "7px"
  md: "10px"
  lg: "12px"
  xl: "16px"
spacing:
  xs: "8px"
  sm: "12px"
  md: "16px"
  lg: "22px"
  xl: "34px"
components:
  button-primary:
    backgroundColor: "{colors.blue}"
    textColor: "{colors.paper}"
    rounded: "{rounded.sm}"
    padding: "0 16px"
    height: "42px"
  button-secondary:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.sm}"
    padding: "0 16px"
    height: "42px"
  work-ticket:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    padding: "20px 21px 17px"
---

# Design System: BizFlow

## Overview

**Creative North Star: The Shop-Counter Ledger**

BizFlow feels like a well-kept order book translated into a dependable, fast
web tool. A deep ink-blue work rail gives the service its frame; white work
slips, ruled dividers, and crisp cobalt action stamps make each next step
legible. A small hit of acid lime draws the eye to time-sensitive states and
the primary marketplace action. The overall tone is direct, approachable, and
capable.

**Key Characteristics:**
- High-contrast work surfaces with clear status states.
- Dense order records balanced by generous page spacing.
- Lime is a selective signal, never decoration across whole panels.

## Colors

Cool paper and ink establish working contrast; cobalt marks action and lime
marks a timely decision.

### Primary
- **Ink navy** (#14243a): Navigation rail and large work-order feature panels.
- **Action cobalt** (#275ee8): Primary actions, links, and focused emphasis.
- **Timing lime** (#d9f36a): The marketplace invitation and due-soon state.

### Neutral
- **Order ink** (#17263b): Primary text and strong business names.
- **Soft ink** (#41536b): Explanatory and secondary text.
- **Quiet text** (#64748b): Supporting descriptions and timestamps.
- **Work white** (#ffffff): Product, listing, form, and order surfaces.
- **Ledger canvas** (#f2f5f8): Main page background.
- **Ruled line** (#dce3eb): Card outlines and list separators.

### Named Rules
**The Status Is Not Color Alone Rule.** A state always includes a text label;
the background tint is supplementary.

## Typography

**Display Font:** Segoe UI (with Helvetica Neue, Arial, sans-serif fallbacks)  
**Body Font:** Segoe UI (with Helvetica Neue, Arial, sans-serif fallbacks)

**Character:** A familiar system sans-serif makes order details quick to scan
and keeps the browser UI responsive without remote font dependencies.

### Hierarchy
- **Display** (780, clamp(29px, 3.2vw, 43px), 1.08): Page titles and the
  shop-counter proposition.
- **Headline** (760, 22px, normal): Section and panel headings.
- **Title** (760, 14–17px, normal): Product names and order subjects.
- **Body** (400, 15px, 1.5): Main instructions and business descriptions;
  constrain long copy to a readable measure.
- **Label** (800, 10–12px, normal, tracked or uppercase where appropriate):
  State, category, and metadata labels.

### Named Rules
**The Work First Rule.** Use a strong subject line for each task; metadata
never competes with the product or order name.

## Layout

The owner workspace uses a 244px ink-blue navigation rail beside a flexible
content column; at narrower desktop widths the rail contracts to 210px and
the listing grid drops from three columns to two. At 800px the rail becomes an
icon strip and the order workspace stacks. At 560px the rail gives way to a
fixed three-destination bottom bar, business listings become a single column,
and filters remain in a horizontally scrollable row. The sticky white header
keeps search and account actions visible. Content uses fluid side padding,
16px list and card gaps, and more vertical separation between sections than
within a work record.

## Elevation & Depth

Ruled borders and contrast establish most hierarchy. Use a soft, offset
shadow sparingly on the floating sample order ticket and on listing hover;
don't replace visible structure with layered shadows.

### Shadow Vocabulary
- **Floating ticket** (`0 18px 45px rgba(0,0,0,.24)`): The feature sample
  ticket against the dark route-board.
- **Raised listing** (`0 16px 40px rgba(20,36,58,.08)`): Subtle hover lift on
  a business listing.

## Shapes

Prefer compact, familiar work surfaces: buttons use 7px corners, fields
7px, cards 10–12px, and the feature panel 15px. The sample order ticket is a
straight-edged paper slip with a dashed separator; round pills are reserved
for filters, business counts, and order states.

## Components

### Buttons
- **Shape:** 7px radius, 42px standard height.
- **Primary:** Cobalt with white text, 16px horizontal padding, 750 weight.
- **Hover / Focus:** Slight upward movement on hover, darker blue; visible
  focus ring on keyboard focus. Disabled actions are visibly muted.
- **Secondary / Ghost:** White surface with a ruled border, or a blue text
  action for low-priority navigation.

### Chips
- **Style:** White surface, fine ruled outline, compact horizontal padding.
- **State:** Filters use dark navy and white for the selected state; unselected
  options stay legible and horizontally scroll rather than wrapping on phones.

### Cards / Containers
- **Corner Style:** 10–12px radius.
- **Background:** White work surfaces on the cool canvas.
- **Shadow Strategy:** Mostly ruled borders; shadows are reserved for the
  feature sample ticket and interactive business-list hover.
- **Border:** One-pixel ledger-gray outline, with thin dividers in lists.
- **Internal Padding:** 15–20px on work surfaces.

### Inputs / Fields
- **Style:** White background, one-pixel blue-gray border, 7px radius.
- **Focus:** Clearly visible cobalt focus ring.
- **Error / Disabled:** Action errors use readable toast copy; disabled submit
  actions visibly mute during processing.

### Navigation
- **Style:** Fixed dark rail with pale inactive labels and a white-on-ink
  active row; the active icon is lime.
- **Mobile:** Replace the rail with an always-available, three-action bottom
  bar and keep the search field in the sticky header.

### Work Ticket
The sample order ticket demonstrates the unique product mechanism: request,
owner confirmation, and completion as distinct steps, with a specific
requested product and slot rather than anonymous marketplace chrome.

## Do's and Don'ts

### Do:
- **Do** keep product or order subjects visually ahead of the surrounding
  metadata.
- **Do** use explicit state labels alongside status colors.
- **Do** preserve a visible focus ring and full text labels for icon-only
  navigation.
- **Do** keep business location and prices scannable at narrow widths.

### Don't:
- **Don't** claim an order was sent, accepted, paid, completed, or backed up
  unless that action actually happened.
- **Don't** show payment details on a public business profile.
- **Don't** imply bank balance, production-grade security, background
  reminders, or millions of supported users in this local prototype.
- **Don't** rely on color, hover, shadows, or gradients as the only way to
  convey a state or action.
