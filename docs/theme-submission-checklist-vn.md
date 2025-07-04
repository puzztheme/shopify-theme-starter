# ✅ Shopify Theme Development & Submission Checklist

## 1. 📦 Theme Structure

- [ ] `/templates/*.liquid` chỉ gọi `{% section 'main-*' %}`
- [ ] Trang chủ dùng `sections/main-home.liquid` với `blocks`
- [ ] Tất cả nội dung tĩnh (text, image...) đều qua `settings` hoặc `blocks`
- [ ] Có đủ các `templates`:
  - [ ] `index.liquid`
  - [ ] `product.liquid`
  - [ ] `collection.liquid`
  - [ ] `cart.liquid`
  - [ ] `search.liquid`
  - [ ] `404.liquid`
  - [ ] `page.contact.liquid`

## 2. 🎨 UI/UX & Design

- [ ] Design độc đáo, không trùng với theme public
- [ ] Mobile-first, responsive hoàn toàn
- [ ] Section homepage hỗ trợ block-based layout
- [ ] Tối ưu padding, typography, line-height
- [ ] Hỗ trợ alignment: left / center / right
- [ ] Hover, focus, CTA states có hiệu ứng rõ ràng
- [ ] Empty states rõ ràng (search, cart, collection empty...)

## 3. 🧱 Code & Performance

- [ ] Không dùng jQuery hoặc thư viện legacy
- [ ] Dùng Alpine.js nếu cần interaction (no overkill)
- [ ] Tailwind CSS tree-shaked và purge đúng content
- [ ] CSS final build < 200KB gzip
- [ ] Không gọi `all_products` trong vòng lặp
- [ ] Không hard-code sản phẩm, link, text

## 4. 🧩 Schema & Customizer

- [ ] Tất cả section đều có `{% schema %}`
- [ ] `presets` hoạt động trong theme editor
- [ ] Có `max_blocks` nếu dùng block-based
- [ ] Section `main-product`, `main-cart`, `main-home` hoạt động đầy đủ

## 5. 🌐 Translations (i18n)

- [ ] Tất cả text hiển thị dùng `{{ 'key' | t }}`
- [ ] `locales/en.default.json` đầy đủ các key
- [ ] Có thể dịch 100% sang tiếng Pháp / Đức / Nhật

## 6. 🔐 Accessibility (A11Y)

- [ ] Có `alt` cho mọi ảnh
- [ ] Dùng `aria-*` cho nút, icon, overlay
- [ ] Hỗ trợ điều hướng bàn phím (focusable menu, drawer)
- [ ] Dùng `role="dialog"` cho modal / cart-drawer

## 7. 🛒 Functional Pages

- [ ] Add to cart hoạt động (form POST hoặc AJAX)
- [ ] Cart page hiển thị item, subtotal, update qty
- [ ] Cart drawer hoạt động nếu có
- [ ] Quickview (optional) hoạt động đúng
- [ ] Search hiển thị kết quả (và có fallback nếu empty)

## 8. 🧪 Validation & Theme Check

- [ ] `theme-check` không có lỗi/blocker
- [ ] `shopify theme validate` pass tất cả kiểm tra
- [ ] Kiểm thử manual trong Shopify Theme Editor:
  - [ ] Add block, move block, remove block không lỗi
  - [ ] Mọi section đều render trong editor

## 9. 🚀 Submission Package

- [ ] Có `README.md` hướng dẫn dùng theme
- [ ] Có `config/settings_schema.json` chuẩn
- [ ] Có `config/settings_data.json` mẫu homepage layout
- [ ] Có ảnh screenshot `assets/theme-preview.png` (1440x900)
- [ ] Nén thành `theme.zip` chuẩn để upload

## 10. ⚠️ Optional But Recommended

- [ ] Sticky filter (collection page)
- [ ] Wishlist UI ready (even if not functional)
- [ ] Loader animation (spinner, fade)
- [ ] Performance: Lighthouse Mobile Score > 85

---
