# Brutalist Theme for Obsidian
Compatible with Style Settings

![](/cover.png)

**What is it?**

**Brutalist is a theme designed specifically for heavy readers and writers.**

Its stark, geometric aesthetics prioritise function and raw form over embellishment. The interface features a strictly angular, squared-off architecture, eliminating rounded corners for a precise, purposeful appearance. The colour scheme utilises low-contrast shades of grey and restrained accents, engineered to maintain focus and minimise visual strain during prolonged sessions. As the name suggests, the aesthetic derives from Brutalist architecture: honest, utilitarian, and bold.

**Design Philosophy**

The objective was to create a comfortable environment that facilitates focused reading and note creation through a low-distraction, text-centric interface. This aids deep work by removing visual clutter.

* **Dark Mode:** Inspired by dedicated reading applications such as Instapaper and Safari’s 'Reader View', the palette is calibrated for optimal comfort in low-light conditions.
* **Light Mode:** Offers a distinct alternative for those who prefer a brighter interface, whilst strictly adhering to the core principles of text primacy and minimal visual interruption.

**Who is this theme for?**

This theme is tailored for individuals who dedicate significant time to reading notes or drafting content within Obsidian. It is particularly effective for users leveraging the Obsidian Web Clipper to manage long-form articles, treating the vault as a reading repository. Similarly, it provides writers with an immersive environment conducive to focused output.

## Customisation
There are two distinct methods for customising the theme: globally via the **Style Settings** plugin, or on a per-note basis using **cssclasses**, or you can use them all combined.

### Global Configuration (Style Settings)
You can configure the following visual elements via the [**Style Settings**](https://github.com/mgmeyers/obsidian-style-settings) plugin:

* **Fonts:** Select distinct typefaces for the body text and the UI/headers (Default: Marcellus).
* **Alignment:** Switch between Left Align (default) and Justified text.
* **Layout:** Adjust the maximum note width (default: 600px) and line height (default: 1.8).

### Per-Note Configuration
**1. Note Width Controls**
By default, notes are restricted to a readable width (800px). You can force specific notes to use more horizontal space. The options available:

* 500px
* 600px (Default)
* 700px
* 800px
* 900px
* 1000px
* Wide (1200px)
* Full Width (100%)

> **Note on Mobile:** These width constraints apply to **Desktop** only. On mobile devices, the theme ignores these classes and fits content to the screen width.

**2. Table Column Layouts**
This theme supports the `cssclasses` property to override global settings for specific files. Add these to your note's YAML frontmatter.

The width you choose for your notes will also affect your tables. However, if you want a specific table to have a particular width, you can use CSS classes incorporated into the theme. In the YAML, simply add one of the following CSS classes:

* width-800
* width-900
* width-1000
* width-1200
* width-1600

Example:

```yaml
---
cssclasses: width-1200
---
```

## Gallery
### Dark Mode
![Brutalist Dark Mode](screenshot.png)

### Light Mode
*Features distinct accents and clear visual hierarchy.*
![Brutalist Light Mode](screenshot-light.png)

## Installation

### Method 1: Community Themes (Currently this plugin is pending review)
1. Open **Settings** > **Appearance**.
2. Click **Manage** under Themes.
3. Search for **Brutalist**.
4. Click **Install** and then **Use**.

### Method 2: Manual Installation
1. Download `theme.css` and `manifest.json` from this repository.
2. Move these files into your vault's hidden folder: `.obsidian/themes/Brutalist/`.
3. Reload Obsidian and select the theme.
### Fonts Used in This Theme

This theme uses the following typefaces:

**iA Writer Family**
* **iA Writer Duo S**, **iA Writer Mono S**, and **iA Writer Quattro S** are sourced from the [iA-Fonts GitHub repository](https://github.com/iaolo/iA-Fonts).

**Google Fonts**
The following fonts are sourced from Google Fonts:
* **Literata** by TypeTogether : [Source](https://fonts.google.com/specimen/Literata).
* **Libre Baskerville** by Impallari Type: [Source](https://fonts.google.com/specimen/Libre+Baskerville)
* **Marcellus** by Astigmatic: [Source](https://fonts.google.com/specimen/Marcellus)
* **Montserrat** by Julieta Ulanovsky, Sol Matas, Juan Pablo del Peral and Jacques Le Bailly: [Source](https://fonts.google.com/specimen/Montserrat)
* **Noto Sans Mono** by Google: [Source](https://fonts.google.com/noto/specimen/Noto+Sans+Mono)
* **Sen** by Kosal Sen: [Source](https://fonts.google.com/specimen/Sen)
* **Spectral** by Production Type: [Source](https://fonts.google.com/specimen/Spectral)

 **Clarification:** Typefaces are embedded within the theme, ensuring availability regardless of internet connection or device.

---

Created by **DuckTapeKiller**
