# ✅ Shopify Theme Development & Submission Checklist

## 1. 📦 Theme Structure

- [ ] `/templates/*.liquid` for all `{% section 'main-*' %}`
- [ ] Homepage use `sections/main-home.liquid` with `blocks`
- [ ] All static content (text, image...) should use `settings` or `blocks`
- [ ] Includes `templates`:
  - [ ] `index.liquid`
  - [ ] `product.liquid`
  - [ ] `collection.liquid`
  - [ ] `cart.liquid`
  - [ ] `search.liquid`
  - [ ] `404.liquid`
  - [ ] `page.contact.liquid`

## 2. 🎨 UI/UX & Design

- [ ] Design should unique, not duplicate public theme
- [ ] Mobile-first, rull responsive
- [ ] Section homepage support block-based layout
- [ ] Optimize padding, typography, line-height
- [ ] Support alignment: left / center / right
- [ ] Hover, focus, CTA states: have obvious effect
- [ ] Empty states more clear (search, cart, collection empty...)

## 3. 🧱 Code & Performance

- [ ] Do not use jQuery or legacy libraries
- [ ] Use Alpine.js if need interaction (no overkill)
- [ ] Tailwind CSS tree-shaked and purge with right content
- [ ] CSS final build < 200KB gzip
- [ ] Dont call `all_products` in the loop
- [ ] Dont hard-code product, link, text

## 4. 🧩 Schema & Customizer

- [ ] All section should have `{% schema %}`
- [ ] `presets` is working in theme editor
- [ ] Have `max_blocks` if use block-based
- [ ] Section `main-product`, `main-cart`, `main-home` fully operational

## 5. 🌐 Translations (i18n)

- [ ] All text display used `{{ 'key' | t }}`
- [ ] `locales/en.default.json` full keys
- [ ] 100% translatable to French/German/Japanese

## 6. 🔐 Accessibility (A11Y)

- [ ] Have `alt` for all image
- [ ] Use `aria-*` for button, icon, overlay
- [ ] Keyboard navigation support (focusable menu, drawer)
- [ ] Use `role="dialog"` for modal / cart-drawer

## 7. 🛒 Functional Pages

- [ ] Add to cart work (form POST hoặc AJAX)
- [ ] Cart page display item, subtotal, update qty
- [ ] Cart drawer active if any
- [ ] Quickview (optional)function properly
- [ ] Search shows results (and has fallback if empty)

## 8. 🧪 Validation & Theme Check

- [ ] `theme-check` dont have error/blocker
- [ ] `shopify theme validate` pass all tests
- [ ] Test manual in Shopify Theme Editor:
  - [ ] Add block, move block, remove block dont error
  - [ ] All section have render in editor

## 9. 🚀 Submission Package

- [ ] Have `README.md` theme user guide
- [ ] Have `config/settings_schema.json` standard
- [ ] Have `config/settings_data.json` demo homepage layout
- [ ] Have image screenshot `assets/theme-preview.png` (1440x900)
- [ ] Nén thành `theme.zip` chuẩn để upload

## 10. ⚠️ Optional But Recommended

- [ ] Sticky filter (collection page)
- [ ] Wishlist UI ready (even if not functional)
- [ ] Loader animation (spinner, fade)
- [ ] Performance: Lighthouse Mobile Score > 85

---
