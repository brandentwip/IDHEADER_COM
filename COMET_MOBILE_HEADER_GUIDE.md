# Comet Mobile Header & Drawer Menu - User & Configuration Guide

Welcome to the **Comet Mobile Header & Drawer Menu** for your Shopify store! This feature replicates the mobile menu design of [WearComet](https://www.wearcomet.com/) with full-width drawer navigation, category tabs (e.g. `MEN`, `WOMEN`, `ABOUT US`), footwear category icons, customizable colors, and mobile responsiveness.

---

## 🌟 Key Features

1. **Full Width Mobile Drawer Navigation**:
   - Spans 100% viewport width on mobile devices for an expansive, modern user experience.

2. **Top Header Bar inside Drawer**:
   - **Close Button `(X)`**: Instantly closes the drawer.
   - **Search Icon `(Magnifying Glass)`**: Quick link to the search page `/search`.
   - **Store Logo / Name**: Clean centered branding.

3. **Tabbed Category Navigation**:
   - Switch between top-level categories (`MEN`, `WOMEN`, `ABOUT US`, etc.) smoothly.
   - Animated active tab indicator line.
   - Automatic fallback: automatically uses top-level Main Menu items if custom tabs are not configured.

4. **Footwear Category Icons**:
   - Dedicated SVG silhouettes for all primary footwear categories:
     - 🥾 **BOOTS**
     - 👞 **CASUALS**
     - 👔 **FORMALS**
     - 👞 **LOAFERS**
     - 🩴 **SANDALS / SLIPPERS**
     - 👟 **SNEAKERS**
     - ➡️ **SHOP ALL**
   - Automatically displays footwear icons based on category link titles or customizable theme preset blocks.

5. **100% Theme Customizer Ready**:
   - Easily enable/disable the Comet Mobile Drawer.
   - Customize header background color, tab text color, active indicator color, and custom menu blocks.

---

## 🛠️ Step-by-Step Configuration Guide

### 1. Access Theme Customizer
1. Log into your **Shopify Admin** panel.
2. Go to **Online Store** > **Themes**.
3. Next to your active theme, click **Customize**.

---

### 2. Configure Header & Mobile Menu Settings
1. In the left sidebar of the Theme Editor, click on **Header**.
2. Scroll down to the **Comet Mobile Header & Drawer** section.

| Setting Name | Type | Description & Recommended Values |
| :--- | :--- | :--- |
| **Enable Comet Mobile Drawer** | Checkbox | Check to enable Comet mobile header (Default: `Checked`). |
| **Header Background Color** | Color Picker | Background color of top drawer bar (Default: `#1d64f2` Comet Blue). |
| **Header Text & Icon Color** | Color Picker | Color of Close button, Search icon, and text (Default: `#ffffff`). |
| **Tab Navigation Background** | Color Picker | Background color of tab bar (Default: `#ffffff`). |
| **Tab Text Color** | Color Picker | Default text color for tab titles (Default: `#111111`). |
| **Active Tab & Accent Color**| Color Picker | Highlight color & underline indicator for active tab (Default: `#1d64f2`). |

---

### 3. Setup Custom Category Tabs (Men / Women / About Us)

Under **Comet Navigation Tabs** in the Header settings:

- **Tab 1 Title**: Enter `MEN` & Select **Tab 1 Menu** (e.g. `Men Menu`).
- **Tab 2 Title**: Enter `WOMEN` & Select **Tab 2 Menu** (e.g. `Women Menu`).
- **Tab 3 Title**: Enter `ABOUT US` & Select **Tab 3 Menu** (e.g. `Main Menu` or `About Us`).
- **Tab 4 Title** *(Optional)*: Enter additional tab name (e.g. `COLLECTIONS`).

---

### 4. Footwear Icon Presets & Custom Icons

The system **automatically** attaches footwear icons to menu links containing `BOOTS`, `CASUALS`, `FORMALS`, `LOAFERS`, `SANDALS`, `SLIPPERS`, `SNEAKERS`, or `SHOP ALL`.

If you wish to explicitly assign an icon or custom image to any menu item:

1. In Theme Customizer under **Header**, click **Add Block**.
2. Select **Mobile Menu Icon**.
3. Fill in the fields:
   - **Menu Item Title**: Type the exact title of the menu item (e.g. `BOOTS`, `LOAFERS`, `FORMALS`).
   - **Custom Icon Image** *(Optional)*: Upload your custom PNG/SVG icon.
   - **Or Select Icon Preset**: Choose from presets:
     - `Sneakers`
     - `Boots`
     - `Casual Shoes`
     - `Formal Shoes`
     - `Loafers`
     - `Sandals / Slippers`
     - `Shop All Arrow`
     - `Star`
     - `Fire / Hot`
     - `Gift`
   - **Badge Text** *(Optional)*: Add text like `NEW`, `HOT`, or `SALE`.

4. Click **Save**.

---

## 📁 File Structure Reference

| File Path | Description |
| :--- | :--- |
| `sections/header.liquid` | Header section file containing Comet schema settings & blocks. |
| `snippets/drawer-menu.liquid` | Main Liquid template rendering full-width header bar, tab switcher, and mobile drawer. |
| `snippets/comet-menu-item-render.liquid` | Sub-snippet handling footwear icon matching, SVG presets, badges, and dropdown links. |
| `assets/comet-mobile-header.css` | Stylesheet controlling 100% full-width drawer, tab indicator line, icons, and micro-animations. |
