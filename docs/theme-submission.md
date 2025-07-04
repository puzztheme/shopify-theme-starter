# 🌟 Shopify Theme Submission – Starter Theme Documentation

This document supports the submission of our custom Shopify Liquid theme to the Shopify Theme Store. It includes all required technical and design specifications as per [Shopify’s Partner Theme Requirements](https://shopify.dev/docs/themes/store/requirements).

---

## 📄 Theme Name

**Theme Name**: ModernPeak  
**Version**: 1.0.0  
**Author**: lofdevteam  
**Target Industries**: Lifestyle, Decor, Fashion, D2C Brands

---

## 🎨 Design Overview

**Design Philosophy**:  
Minimal, image-first theme optimized for high-conversion eCommerce stores. Prioritizes whitespace, fast-loading visuals, and mobile usability.

**Key Differentiators**:

- Blocks-first homepage (modular layout builder)
- Custom animated hero with CTA & dual buttons
- AJAX cart drawer + responsive header
- Alpine.js for lightweight interactivity
- Tailwind CSS + Vite setup for performance-focused styling

---

## 🧱 Technical Stack

| Layer        | Stack                              |
|-------------|-------------------------------------|
| CSS         | Tailwind CSS (purged via Vite)     |
| JS          | Alpine.js (v3+)                     |
| Build Tool  | Vite (builds to `assets/vite/`)     |
| Theme Engine| Shopify Liquid                      |
| CI/CD       | GitHub Actions (auto build)         |

---

## ✅ Shopify Compatibility

- [x] Online Store 2.0 (Section Everywhere)
- [x] Global Settings via `settings_schema.json`
- [x] Fully Responsive (Mobile-first)
- [x] Translatable via `locales/en.default.json`
- [x] Accessible: alt tags, ARIA roles, keyboard-friendly
- [x] AJAX Cart Drawer
- [x] Search & 404 templates
- [x] Cart Page and Cart Notes supported
- [x] Section schema includes `presets` and `blocks`

---

## 📂 Theme Structure

