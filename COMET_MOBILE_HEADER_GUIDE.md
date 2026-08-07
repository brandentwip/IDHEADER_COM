# Comet Mobile Header & Drawer Menu - User & Configuration Guide

Welcome to the **Comet Mobile Header & Drawer Menu** for your Shopify store! This feature replicates the mobile menu design of [WearComet](https://www.wearcomet.com/) with tabbed category navigation (e.g. `MEN`, `WOMEN`, `ABOUT US`), item icon support (shoe silhouettes, shop icons, custom uploads), customizable colors, and mobile-optimized responsiveness.

---

## 🌟 Key Features

1. **Top Header Bar inside Drawer**:
   - **Close Button `(X)`**: Instantly closes the drawer.
   - **Search Icon `(Magnifying Glass)`**: Quick link to the search page `/search`.
   - **Store Logo / Name**: Clean centered branding.

2. **Tabbed Navigation Bar**:
   - Switch between top-level categories (`MEN`, `WOMEN`, `ABOUT US`, etc.) smoothly.
   - Active tab indicator line with smooth transition effect.
   - Dynamic out-of-the-box fallback: automatically uses top-level Main Menu items if custom tabs are not configured.

3. **Menu Links & Icon Support**:
   - Bold uppercase typography (`NEW IN`, `SNEAKERS`, `THE VAULT`, `GIFTING GUIDE`).
   - Icon assignment per menu item (Preset sneaker silhouettes, Shop All arrows, Star, Fire, Gift, or custom uploaded PNG/SVG icons).
   - Optional badge tags (`NEW`, `SALE`, `HOT`).
   - Expandable sub-menus for sub-categories.

4. **100% Theme Customizer Ready**:
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

> [!TIP]
> **Automatic Mode**: If you leave the Tab fields blank, the system automatically uses your top-level items from your Shopify **Main Menu** as the tabs!

---

### 4. Adding Icons & Badges to Menu Items

You can attach icons and badges to specific menu items (e.g. `X LOWS`, `AERES`, `SHOP ALL`).

1. In Theme Customizer under **Header**, click **Add Block**.
2. Select **Mobile Menu Icon**.
3. Fill in the fields:
   - **Menu Item Title**: Type the **exact** menu item name (e.g., `X LOWS` or `SHOP ALL`).
   - **Custom Icon Image** *(Optional)*: Upload a small PNG/SVG icon.
   - **Or Select Icon Preset**: Choose from built-in presets:
     - `Sneaker Icon 1 (Low Top)`
     - `Sneaker Icon 2 (Runner)`
     - `Sneaker Icon 3 (Court)`
     - `Shop All Arrow`
     - `Star`
     - `Fire / Hot`
     - `Gift`
   - **Badge Text** *(Optional)*: Add text like `NEW`, `HOT`, or `SALE`.

4. Click **Save** in the top right corner.

---

## 📁 File Structure Reference

| File Path | Description |
| :--- | :--- |
| `sections/header.liquid` | Header section file containing Comet schema settings & blocks. |
| `snippets/drawer-menu.liquid` | Main Liquid template rendering header bar, tab switcher, and mobile drawer. |
| `snippets/comet-menu-item-render.liquid` | Sub-snippet handling icon matching, preset SVGs, badges, and dropdown links. |
| `assets/comet-mobile-header.css` | Stylesheet controlling drawer header, tab indicator line, icons, and micro-animations. |

---

## 💡 Troubleshooting & Notes

> [!NOTE]
> - **Mobile Display**: The Comet drawer header is styled for mobile screens (`medium-up--hide`), keeping your desktop header fully intact.
> - **Exact Matching**: When adding **Mobile Menu Icon** blocks, ensure the **Menu Item Title** matches the link title in your Shopify Navigation exactly (case-insensitive).
