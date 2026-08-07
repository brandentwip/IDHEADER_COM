# Comet Mobile Header & Drawer Menu - User & Configuration Guide

Welcome to the **Comet Mobile Header & Drawer Menu** for your Shopify store! This feature replicates the mobile menu design of [WearComet](https://www.wearcomet.com/) with full-width drawer navigation, category tabs (e.g. `MEN`, `WOMEN`, `ABOUT US`), category icon matching, custom image uploads, customizable colors, and mobile responsiveness.

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

4. **Footwear Category Custom Icons (Global Category Settings)**:
   - Dedicated image upload settings for your key footwear categories:
     - 🥾 **BOOTS**
     - 👞 **CASUALS**
     - 👔 **FORMALS**
     - 👞 **LOAFERS**
     - 🩴 **SANDALS / SLIPPERS**
     - 👟 **SNEAKERS**
   - **Automatic Image Matching**: When you upload an icon image for a category in Theme Customizer settings, any menu item whose name matches that category (e.g. `BOOTS`, `CASUALS`) will automatically display your uploaded custom icon!
   - Default vector SVGs built-in if no image is uploaded.

5. **100% Theme Customizer Ready**:
   - Easily enable/disable the Comet Mobile Drawer.
   - Customize header background color, tab text color, active indicator color, category icons, and item-specific blocks.

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

### 3. Upload Category Custom Icons (Automatic Matching)

Under **Category Custom Icons** in Header section settings:

- **Boots Icon**: Upload your custom PNG/SVG for `BOOTS`.
- **Casual Shoes Icon**: Upload your custom PNG/SVG for `CASUALS`.
- **Formal Shoes Icon**: Upload your custom PNG/SVG for `FORMALS`.
- **Loafers Icon**: Upload your custom PNG/SVG for `LOAFERS`.
- **Sandals / Slippers Icon**: Upload your custom PNG/SVG for `SANDALS/SLIPPERS`.
- **Sneakers Icon**: Upload your custom PNG/SVG for `SNEAKERS`.

> [!TIP]
> Once an image is uploaded in these category settings, any menu link containing that category name will **automatically show your custom icon image**!

---

### 4. Custom Icon Blocks for Individual Items

If you want to assign a custom image or badge to an item that is NOT a main category name (e.g. `X LOWS` or `SPECIAL OFFER`):

1. Under **Header** in Theme Customizer, click **Add Block**.
2. Select **Mobile Menu Icon**.
3. Fill in the fields:
   - **Menu Item Title**: Type the exact title of the menu item (e.g. `X LOWS`).
   - **Custom Icon Image**: Upload your image.
   - **Badge Text** *(Optional)*: Add text like `NEW`, `HOT`, or `SALE`.
4. Click **Save**.

---

## 📁 File Structure Reference

| File Path | Description |
| :--- | :--- |
| `sections/header.liquid` | Contains Comet settings, category custom icon uploaders, and block definitions. |
| `snippets/drawer-menu.liquid` | Template rendering full-width header bar, tab switcher, and mobile drawer. |
| `snippets/comet-menu-item-render.liquid` | Sub-snippet handling category image matching, fallback SVGs, badges, and dropdown links. |
| `assets/comet-mobile-header.css` | Stylesheet controlling 100% full-width drawer, tab indicator line, icons, and micro-animations. |
