# Final Results — Qolbul Muzaki

## Portfolio Info
- **Nama:** Qolbul Muzaki
- **Repository:** d:/zaki/zaki-portofolio
- **Tech Stack:** HTML5 + CSS3
- **Design:** Neobrutalism, Mobile-first
- **Date:** May 5, 2026

---

## Screenshot: Desktop

[paste screenshot — all sections visible]

---

## Screenshot: Mobile

[paste screenshot — responsive, no horizontal scroll]

---

## What I Learned

1. **Semantic HTML5 Structure Matters**: Menggunakan elemen yang tepat seperti `header`, `nav`, `main`, `section`, `article`, dan `footer` bukan hanya untuk SEO, tapi juga membuat kode lebih readable, maintainable, dan accessible untuk screen readers. Zero non-semantic divs menunjukkan pemahaman mendalam tentang HTML semantik.

2. **CSS-Only Solutions untuk Mobile Interaction**: Hamburger menu bisa diimplementasikan tanpa JavaScript menggunakan checkbox input hidden dan label trigger dengan CSS selector `:checked`. Ini menunjukkan bahwa tidak semua interaksi butuh JavaScript—pemahaman CSS yang mendalam bisa menggantikan logic complexity.

3. **Mobile-First Approach Fundamental**: Mulai dari mobile (320px) membuat design yang lebih robust. Desktop versi jadi natural evolution, bukan afterthought. Ini juga meningkatkan performance karena mobile mendapat prioritas utama.

4. **Neobrutalism sebagai Design Philosophy**: Border tegas, shadow block, dan kontras kuat menciptakan karakter yang bold namun tetap minimalis. Design ini cocok untuk startup yang ingin terlihat inovatif dan tegas.

5. **RTCC-O Framework untuk Planning yang Sistematis**: Role, Task, Context, Constraints, Output yang jelas dari awal membuat execution lebih efisien. Setiap keputusan bisa di-justify dengan framework ini.

---

## Challenges & Solutions

**Challenge 1: Implementasi Hamburger Menu CSS-Only**
- **Deskripsi**: Membuat burger menu yang fungsional tanpa JavaScript, dengan ikon burger dan teks "Menu" yang centered di mobile.
- **Solution**: Menggunakan checkbox input (`nav-toggle`) yang di-hide dengan `opacity: 0`, label sebagai trigger (`nav-toggle-label`), dan pseudo-element `::before` untuk ikon burger. CSS selector `:checked` untuk mengontrol visibility nav-list. Hasilnya: clean, minimal, dan fully semantic.

**Challenge 2: Alignment Ikon Burger dan Teks**
- **Deskripsi**: Ikon burger dan teks "Menu" sulit di-align dengan sempurna, bisa terlihat janggal di mobile.
- **Solution**: Menggunakan flexbox dengan `align-items: center` dan `gap: 0.75rem`. Pseudo-element `::before` untuk ikon menggunakan `box-shadow` untuk garis-garis burger, dengan `transform: translateY()` untuk fine-tuning vertical alignment.

**Challenge 3: Zero Non-Semantic Divs**
- **Deskripsi**: Membuat layout yang kompleks tanpa menggunakan div wrapper—struktur harus tetap semantic.
- **Solution**: Menggunakan elemen yang tepat: `header`, `nav`, `main`, `section`, `article` untuk setiap blok konten. Grid dan flexbox pada CSS handle layout tanpa div helper. Hasilnya: struktur lebih jelas dan maintainable.

**Challenge 4: Responsive Spacing dan Typography**
- **Deskripsi**: Font dan spacing yang cocok di mobile tapi tidak terlihat terlalu besar di desktop.
- **Solution**: Menggunakan CSS `clamp()` function: `font-size: clamp(1.75rem, 3vw, 2.5rem)`. Media queries untuk padding dan gap yang berbeda antara mobile dan desktop. Consistent line-height (1.6) untuk readability.
