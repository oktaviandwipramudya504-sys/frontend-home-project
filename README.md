# Resonance Trilogy - Landing Page Module

Selamat datang di repositori modul frontend **Resonance Trilogy**. Kode ini merupakan berkas *template* Jinja2 yang berfungsi sebagai modul halaman utama (*Hero Landing Page*) berestetika mewah (*luxury cinematic theme*) untuk platform web manajemen atau profil produksi milik Resonance Trilogy.

## Deskripsi Struktur Kode

Berkas ini mengintegrasikan komponen frontend modern yang dibungkus di dalam ekosistem backend Python berbasis kerangka kerja **Flask**:
- **Arsitektur Template:** Menggunakan pewarisan templat (Jinja2 Template Inheritance) `{% extends 'admin/layout.html' %}` untuk menjaga konsistensi komponen navigasi (*sidebar/navbar*).
- **Tipografi Sinematik:** Mengintegrasikan Google Fonts pilihan untuk membangun citra premium:
  - `Cinzel`: Digunakan untuk judul utama film/sinema agar terkesan megah.
  - `Cormorant Garamond`: Digunakan untuk deskripsi puitis berestetika klasik (*serif italic*).
  - `Montserrat`: Digunakan untuk label penjelas (*sub-heading*) yang modern dan bersih.
- **Desain Latar Belakang Video:** Menggunakan tag `<video>` interaktif berukuran penuh (*fullscreen 100vh*) yang memutar berkas `resonancetrilogy.mp4` secara otomatis (*autoplay*, *muted*, *looping*) dilapisi dengan *gradient overlay* gelap.

---

## Fitur Utama

1. **Luxury Gold & Dark Aesthetic:** Kustomisasi kelas CSS global yang memaksa elemen navbar bawaan mengadopsi warna emas mewah (`#dab01b`) agar serasi dengan konsep jenama (*branding*).
2. **Cinematic Animation System:** Efek animasi *fade-in slide-up* beruntun (`delay-1` hingga `delay-4`) menggunakan CSS Keyframes untuk memberikan kesan transisi panggung sinema saat halaman dimuat.
3. **Floating Interactive Bubbles:** Tombol melayang di pojok kanan bawah dengan efek animasi mengapung secara kontinu (*infinite floating loop*). Berfungsi sebagai pintasan integrasi langsung ke WhatsApp bisnis untuk dua divisi kritikal:
   - **Admin Productions** (Operasional & Produksi)
   - **Admin Finance** (Keuangan & Akuntansi)
4. **Fully Responsive Layout:** Optimalisasi media queries (`@media max-width: 768px`) untuk memastikan video latar belakang, tipografi raksasa, dan tombol aksi tetap proporsional saat diakses melalui perangkat seluler (smartphone).

---

##  Struktur Komponen Dokumen

```text
├── CSS Inclusions (Google Fonts Hub)
├── Custom Styles (<style> scoped block)
│   ├── Navbar Gold Override
│   ├── Fullscreen Video Wrapper & Dark Gradient Overlay
│   ├── Fonts Styling (Cinzel, Garamond, Montserrat)
│   ├── Keyframes Key-Animation (slideUpFade & float loops)
│   └── Mobile Responsiveness Adaptations
├── Header Semantic Container (<header class="hero-fullscreen">)
│   ├── Local Source Video Ingestion
│   └── Brand Text Header Group (Title, Divider, Slogans)
└── Floating CTA Buttons Window (<div class="bubble-container">)
    ├── WhatsApp Action: Admin Productions
    └── WhatsApp Action: Admin Finance
