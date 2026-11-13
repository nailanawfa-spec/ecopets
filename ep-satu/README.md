# Eco-Pet — Pixel Eco-Pet Adventure App

Aplikasi pet pixel bertema lingkungan. Rawat pet-mu lewat aksi hijau harian.

**Stack:** Next.js + Payload CMS + Tailwind CSS (dibuat di Figma Make)

## Fitur
- Daftar dan Masuk dengan email + kata sandi (sesi aman lewat cookie)
- Pilih pet: kura-kura, kelinci, kucing, ular
- Level, XP, poin, token eco, streak harian, aksesori
- Aksi hijau: transportasi, sampah, energi, makanan, alam, edukasi
- Chat dengan pet, komunitas + leaderboard, pertemanan, diary foto
- Panel admin di `/admin`

## Cara pakai
**Lewat Figma Make (disarankan):** di Figma Make pilih Import dari GitHub / hubungkan repo ini.
Database dan backend disediakan Figma, jadi login dan sinkron data langsung jalan.
Folder `figma-config/` berisi konfigurasi Figma Make (nama aslinya `.figma`).

**Jalan di lokal:**
```bash
pnpm install
pnpm dev
```
Catatan: di luar Figma, backend memerlukan variabel `FIGMA_CONTENT_API_*`.
Untuk hosting sendiri, database perlu diganti (mis. Postgres) di `src/payload.config.ts`.

## Struktur singkat
- `src/app/(frontend)/` — tampilan app dan API (`api/app/route.ts`)
- `src/collections/` — data: users, activities, pet-messages, friendships, diary, dll.
- `src/lib/app-auth.ts` — login/sesi
- `figma-config/` — konfigurasi Figma Make
