# Comet Mobile Header & Drawer Menu - User & Configuration Guide

Welcome to the **Comet Mobile Header & Drawer Menu** for your Shopify store! This feature replicates the mobile menu design of [WearComet](https://www.wearcomet.com/) with full-width drawer navigation, category tabs (e.g. `MEN`, `WOMEN`, `ABOUT US`), category custom icon uploads, tab-specific promo banner images, customizable colors, and mobile responsiveness.

---

## 🌟 Key Features

1. **Full Width Mobile Drawer Navigation**:
   - Spans 100% viewport width on mobile devices for an expansive, modern user experience.

2. **Top Header Bar inside Drawer**:
   - **Close Button `(X)`**: Instantly closes the drawer.
   - **Search Icon `(Magnifying Glass)`**: Quick link to the search page `/search`.
   - **Store Logo / Name**: Clean centered branding.

3. **Tabbed Category Navigation & Changing Bottom Banner Images**:
   - Switch between top-level categories (`MEN`, `WOMEN`, `ABOUT US`, etc.) smoothly.
   - **Dynamic Tab Banner Images**: Upload a separate bottom promotional banner image per tab (e.g. Men footwear banner for `MEN`, Women lifestyle banner for `WOMEN`). The banner image changes automatically when switching tabs!
   - Banner links: Make each banner image clickable to direct shoppers to a specific collection or product page.

4. **Footwear Category Custom Icons**:
   - Automatic Image Matching across all footwear categories:
     - 🥾 **BOOTS**
     - 👞 **CASUALS**
     - 👔 **FORMALS**
     - 👞 **LOAFERS**
     - 🩴 **SANDALS / SLIPPERS**
     - 👟 **SNEAKERS**
     - ➡️ **SHOP ALL**

---

## 🛠️ Step-by-Step Configuration Guide

### 1. Access Theme Customizer
1. Log into your **Shopify Admin** panel.
2. Go to **Online Store** > **Themes** > **Customize**.
3. In the left sidebar, click directly on **Header**.

---

### 2. Setting Up Tab Promo Banner Images (Men / Women)

Under **Comet Navigation Tabs** in the Header settings panel:

- **Tab 1 Title**: Enter `MEN`
  - **Tab 1 Menu**: Select your Men's Linklist menu.
  - **Tab 1 Bottom Promo Banner Image**: Upload your Men's promo banner image.
  - **Tab 1 Banner Link**: Enter target URL (e.g. `/collections/men`).

- **Tab 2 Title**: Enter `WOMEN`
  - **Tab 2 Menu**: Select your Women's Linklist menu.
  - **Tab 2 Bottom Promo Banner Image**: Upload your Women's promo banner image.
  - **Tab 2 Banner Link**: Enter target URL (e.g. `/collections/women`).

- **Tab 3 Title**: Enter `ABOUT US` (or custom title)
  - **Tab 3 Bottom Promo Banner Image**: Upload banner image for Tab 3.
  - **Tab 3 Banner Link**: Enter target URL.

---

### 3. Upload Category Custom Icons

Under **Category Custom Icons** in Header section settings:
- Upload images for **Boots Icon**, **Casual Shoes Icon**, **Formal Shoes Icon**, **Loafers Icon**, **Sandals / Slippers Icon**, **Sneakers Icon**.

---

## 📁 File Structure Reference

| File Path | Description |
| :--- | :--- |
| `sections/header.liquid` | Contains Comet settings, tab promo image pickers, category custom icon uploaders, and block definitions. |
| `snippets/drawer-menu.liquid` | Template rendering full-width header bar, tab switcher, menu lists, and changing tab promo banners. |
| `snippets/comet-menu-item-render.liquid` | Sub-snippet handling category image matching, fallback SVGs, badges, and dropdown links. |
| `assets/comet-mobile-header.css` | Stylesheet controlling 100% full-width drawer, tab indicator line, tab promo images, and micro-animations. |
