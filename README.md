# Riza Aditya — Portfolio Web (Static & Interactive)

Versi statis interaktif dari portofolio Riza Aditya, dioptimalkan untuk hosting gratis di **Cloudflare Pages**, **Vercel**, atau **GitHub Pages**.

## Fitur Interaktif (Vanilla JavaScript):
1. **Smooth Page Transitions**: Perpindahan halaman mulus tanpa layar berkedip/reload (PJAX Client-side Router).
2. **Interactive Project Modal**: Klik kartu proyek pada menu Portfolio untuk melihat detail, screenshot, tag, dan link aksi dalam popup modal.
3. **Animated Category Filter**: Filter kategori proyek (All, Mobile Apps, Academic, System Design, Videografi) dengan transisi visual halus.
4. **Click-to-Copy with Toast**: Klik pada kartu Email atau WhatsApp di halaman Contact untuk langsung menyalin ke clipboard dengan notifikasi toast.
5. **Responsive**: Layout adaptif untuk Desktop dan Mobile.

---

## Cara Deploy ke Cloudflare Pages (100% Gratis Selamanya)

### Langkah 1: Push ke GitHub
Buka terminal di dalam folder `web_porto_static`:
```bash
git init
git add .
git commit -m "feat: portfolio static release"
git branch -M main
git remote add origin https://github.com/Riza2803/portfolio-static.git # Sesuaikan dengan nama repo Anda
git push -u origin main
```

### Langkah 2: Hubungkan ke Cloudflare Pages
1. Buka [dash.cloudflare.com](https://dash.cloudflare.com/) (Daftar/Login gratis).
2. Di menu kiri, pilih **Workers & Pages** $\rightarrow$ **Create application** $\rightarrow$ **Pages** $\rightarrow$ **Connect to Git**.
3. Pilih repositori GitHub Anda (`portfolio-static`).
4. Pada **Build settings**:
   - **Framework preset**: `None`
   - **Build command**: *(Kosongkan)*
   - **Build output directory**: `/` *(atau kosongkan / titik `.`)*
5. Klik **Save and Deploy**.

Dalam ~20 detik, website Anda sudah aktif di domain gratis, misalnya `https://portfolio-static.pages.dev`.
