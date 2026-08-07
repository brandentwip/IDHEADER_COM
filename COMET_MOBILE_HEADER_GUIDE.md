# Comet Mobile Header & Drawer Menu - User & Configuration Guide

Welcome to the **Comet Mobile Header & Drawer Menu** for your Shopify store! This feature replicates the mobile menu design of [WearComet](https://www.wearcomet.com/) with full-width drawer navigation, category tabs (e.g. `MEN`, `WOMEN`, `ABOUT US`), category custom icon uploads, customizable colors, and mobile responsiveness.

---

## 📍 How to Find & Upload Custom Category Icons in Theme Customizer

There are **2 EASY WAYS** to add custom category icons in your Shopify Theme Customizer:

### Method A: Under Section Settings (Global Uploads)
1. Go to **Shopify Admin** > **Online Store** > **Themes** > **Customize**.
2. On the left sidebar, click directly on the section title **Header**.
3. Scroll down in the left settings panel to **Category Custom Icons**.
4. You will see image uploaders for:
   - **Boots Icon**
   - **Casual Shoes Icon**
   - **Formal Shoes Icon**
   - **Loafers Icon**
   - **Sandals / Slippers Icon**
   - **Sneakers Icon**
5. Upload your custom icon image next to any category. Any menu item containing that category name will **automatically display your uploaded custom icon**!

---

### Method B: Via "+ Add block" (Block Uploads)
1. Click on **Header** in the left sidebar of Theme Customizer.
2. Click **+ Add block**.
3. Select **Category Custom Icon**.
4. Select your category (`SNEAKERS`, `BOOTS`, `CASUALS`, `FORMALS`, `LOAFERS`, `SANDALS`, `SHOP ALL`) or type a custom category title.
5. Upload your **Category Icon Image** and click **Save**.

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

4. **Footwear Category Custom Icons**:
   - Automatic Image Matching across all footwear categories:
     - 🥾 **BOOTS**
     - 👞 **CASUALS**
     - 👔 **FORMALS**
     - 👞 **LOAFERS**
     - 🩴 **SANDALS / SLIPPERS**
     - 👟 **SNEAKERS**
     - ➡️ **SHOP ALL**
   - Fallback SVGs built-in if no image is uploaded.

---

## 📁 File Structure Reference

| File Path | Description |
| :--- | :--- |
| `sections/header.liquid` | Contains Comet settings, category custom icon uploaders, and block definitions. |
| `snippets/drawer-menu.liquid` | Template rendering full-width header bar, tab switcher, and mobile drawer. |
| `snippets/comet-menu-item-render.liquid` | Sub-snippet handling category image matching, fallback SVGs, badges, and dropdown links. |
| `assets/comet-mobile-header.css` | Stylesheet controlling 100% full-width drawer, tab indicator line, icons, and micro-animations. |
