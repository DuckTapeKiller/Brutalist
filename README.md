# Brutalist: A Theme for Obsidian

Compatible with Style Settings.

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/ducktapekiller)

![brutalist](screenshots/brutalist_pixel_art.jpg)

## Table of Contents
1. [Introduction](#1-introduction)
2. [Global Configuration](#2-global-configuration)
   1. [Fonts](#21-fonts)
   2. [Alignment](#22-alignment)
   3. [Note Width Control](#23-note-width-control)
   4. [Line Height](#24-line-height)
   5. [Inline Title Size](#25-inline-title-size)
   6. [Auto-hide Side Ribbon](#26-auto-hide-side-ribbon)
   7. [Mobile Settings](#27-mobile-settings)
3. [Per-Note Overrides](#3-per-note-overrides)
   1. [Custom Widths and Interface Hiding](#31-custom-widths-and-interface-hiding)
4. [Dashboard and Masonry Layout](#4-dashboard-and-masonry-layout)
   1. [Using Callouts](#41-using-callouts)
   2. [Dashboard Banners](#42-dashboard-banners)
5. [CSS-Only Timelines](#5-css-only-timelines)
6. [Gallery](#6-gallery)
7. [Installation](#7-installation)
- [SUMMARY: ALL CSSCLASSES AVAILABLE](#summary-all-cssclasses-available)

## 1 Introduction

**What is it?**
“Brutalist” is a theme designed for heavy readers and writers. Its stark, geometric aesthetics prioritise function and raw form over embellishment. The interface features a strictly angular architecture, eliminating rounded corners for a precise appearance. The colour scheme utilises low-contrast shades of grey and restrained accents to maintain focus and minimise visual strain. The aesthetic derives from Brutalist architecture: honest, utilitarian, and bold.

**Design Philosophy**
The objective is to create a comfortable environment that facilitates focused reading and note creation through a low-distraction, text-centric interface.

* **Dark Mode:** Inspired by dedicated reading applications such as Instapaper and Safari’s “Reader View”, the palette is calibrated for low-light conditions.
* **Light Mode:** Offers a brighter interface whilst adhering to the core principles of text primacy.

**Who is this theme for?**
It is tailored for individuals who dedicate significant time to reading or drafting content within Obsidian. It is effective for users leveraging the Obsidian Web Clipper to manage long-form articles, treating the vault as a reading repository.

## 2 Global Configuration

You can configure the following visual elements via the [Style Settings](https://github.com/mgmeyers/obsidian-style-settings) plugin.

### 2.1 Fonts

The theme embeds several typefaces, ensuring offline availability without local installation. In Style Settings, you can choose these for Body or UI/Headers (Default: Sen for UI, iA Writer Quattro S for Body).

* **Serif:** Hepta Slab, Libre Baskerville, Libre Caslon Text, Marcellus, Spectral.
* **Sans Serif:** iA Writer Duo S, iA Writer Quattro S, Libre Franklin, Montserrat, Sen.
* **Monospace:** iA Writer Mono S, Noto Sans Mono.

### 2.2 Alignment

Modify text alignment via the dropdown menu in Style Settings:
* Left aligned (default)
* Right aligned
* Centre aligned
* Justified

### 2.3 Note Width Control

Notes are restricted to a readable width (800px) by default. Options include:
* 500px, 600px, 700px, 800px, 900px, 1000px, Wide (1200px), Full Width (100%).

> **Note on Mobile:** Width constraints apply to desktop only. On mobile devices, the theme fits content to the screen width.

### 2.4 Line Height

Default decimal line spacing is 1.5. Adjust between 1.0 and 3.0 via the Style Settings slider.

### 2.5 Inline Title Size

Adjust the size of the inline title relative to the text. Range: 1.0em to 5.0em (Default: 2em).

### 2.6 Auto-hide Side Ribbon

Toggle this option to hide the left ribbon interface. It appears when hovering over the left edge.

### 2.7 Mobile Settings

Configure the mobile drawer and navigation bar.
* **Drawer:** Set background colour for Light and Dark modes.
* **Navigation Bar:** Set border thickness (0px - 10px), opacity (0.0 - 1.0), background colour, and radius (0px - 30px).

![brutalist](screenshots/mobile_navbar_1.png)
![brutalist](screenshots/mobile_navbar_2.png)

## 3 Per-Note Overrides

Use the `cssclasses` property in your frontmatter to override global settings for specific files.

### 3.1 Custom Widths and Interface Hiding

To set a custom width, add one of the following classes: `width-800`, `width-900`, `width-1000`, `width-1200`, `width-1600`.

To hide frontmatter and note titles (useful for homepages or tables), use `hide-all`.

Example combining both:
```yaml
---
cssclasses:
  - width-1200
  - hide-all
---
```

## 4 Dashboard and Masonry Layout

Organise notes into a clean grid. The system supports native Obsidian callouts, automatically distributing columns (2 by default, 3 on wide screens, 1 on mobile). To activate, add `cssclasses: dashboard` to your frontmatter.

### 4.1 Using Callouts

Every callout within a `dashboard` note transforms into a masonry card.

```markdown
---
cssclasses: dashboard
---

> [!info] My Card
> - [[Link 1]]
> - [[Link 2]]
```

![Dashboard Callout Result](screenshots/dashboard-callout-result.png)

### 4.2 Dashboard Banners

Create a full-width banner callout that spans to the tab header. Adjust height, card vertical offset, and banner transparency (for a “frosted glass” effect) via Style Settings.

```markdown
> [!banner]
> ![[your_banner.jpg]]
```

**Important Considerations:**
* **Desktop Only:** Banners are hidden on mobile to save space.
* **Fixed Positioning:** The banner is fixed. For dashboards requiring scrolling, it is recommended to use the [Brutalist Persistent Banner](https://github.com/DuckTapeKiller/brutalist-persistent-banner) plugin to keep it permanently visible.

<img width="1388" height="1064" alt="Screenshot" src="https://github.com/user-attachments/assets/e20502d8-af85-447c-9c0f-e03825de871b" />

## 5 CSS-Only Timelines

A native layout transforming bulleted lists into a split-view chronology. Add `cssclasses: custom-timeline` to the frontmatter. Structure the timeline as a single unordered list with three bullet points per event: Date, Title, and Content.

```markdown
---
cssclasses:
  - custom-timeline
  - hide-all
---

- 1950–1953
- Land Reform Movement
- Shortly after the establishment of the PRC, the Chinese Communist Party (CCP) launched a nationwide campaign to confiscate land from rural landlords and redistribute it to landless peasants. This movement violently dismantled the traditional rural class structure and consolidated CCP control in the countryside.

- 1951–1952
- Three-Anti and Five-Anti Campaigns
- These were urban reform movements designed to consolidate state control over the economy. The "Three-Anti" campaign targeted communist cadres for corruption, waste, and bureaucracy. The "Five-Anti" campaign targeted the capitalist class, penalising business owners for bribery, tax evasion, theft of state property, cheating on government contracts, and stealing state economic information.
```

![timeline](screenshots/timeline.png)

---
Would you like me to map out the built-in callout types and their corresponding rgb colour values from the CSS?

## 6 Gallery

### Dark Mode
![Brutalist Dark Mode](screenshot.png)

### Light Mode
![Brutalist Light Mode](screenshot-light.png)

## 7 Installation

### Method 1: Community Themes
1. Open **Settings > Appearance**.
2. Click **Manage** under Themes.
3. Search for **Brutalist**.
4. Click **Install** and then **Use**.

### Method 2: Manual Installation
1. Download `theme.css` and `manifest.json` from this repository.
2. Move these files into your vault's hidden folder: `.obsidian/themes/Brutalist/`.
3. Reload Obsidian and select the theme.

---

## SUMMARY: ALL CSSCLASSES AVAILABLE

| `cssclass` | Function | Behaviour Details |
| :--- | :--- | :--- |
| `width-800` | Sets fixed note width | Constrains the editor and reading view content to a maximum width of 800px. Centers the content. |
| `width-900` | Sets fixed note width | Constrains the editor and reading view content to a maximum width of 900px. Centers the content. |
| `width-1000` | Sets fixed note width | Constrains the editor and reading view content to a maximum width of 1000px. Centers the content. |
| `width-1200` | Sets fixed note width | Constrains the editor and reading view content to a maximum width of 1200px. Centers the content. |
| `width-1600` | Sets fixed note width | Constrains the editor and reading view content to a maximum width of 1600px. Centers the content. |
| `full-width` | Sets responsive width | Forces the note content to span 100% of the available viewing pane. |
| `hide-all` | UI visibility toggle | Completely hides the frontmatter container, metadata properties, and inline note titles. |
| `dashboard` | Activates grid layout | Transforms the note into a responsive masonry grid structure. Converts standard callouts into floating dashboard cards. |
| `custom-timeline` | Activates timeline layout | Converts standard unordered lists into a split-view, CSS-only vertical chronology grid. |

_This theme is a perpetual work in progress._

Created by **DuckTapeKiller**
