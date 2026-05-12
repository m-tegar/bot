# TODO - AI Cyber Pentest Control Platform

## Phase 1: Skeleton & Kontrak Sistem
- [x] Buat struktur folder: frontend, backend, worker, shared (sebagian)
- [x] Inisialisasi Next/Tailwind/Framer Motion/socket.io-client (sebagian)
- [x] Buat FastAPI app + endpoint health
- [x] Buat endpoint scan MVP + event WS contract (placeholder)
- [x] Buat worker loop placeholder

## Phase 2: Engines
- [ ] Implement XSS engine: crawling, parameter detection, reflection testing, payload injection, validation check
- [ ] Implement SQLi engine: parameter fuzzing, boolean-based detection, time-based detection, response comparison
- [ ] Implement Validation Engine (anti false positive): bukti payload + response snippet + signature match

## Phase 3: AI/SOC Report Generator
- [ ] Implement report generator: JSON report + HTML dashboard report + downloadable file
- [ ] Implement SOC-style AI analysis formatter (tanpa API call bila tidak ada key)

## Phase 4: Dashboard UI
- [ ] Implement halaman report viewer + download HTML
- [ ] Tambah tampilan validation evidence + payload used + snippet
- [ ] Integrasi event real scan (bukan placeholder)

## Phase 5: Validasi (harus ada error logs jelas)
- [ ] Pastikan backend bisa start (uvicorn) setelah dependency sukses
- [ ] Pastikan worker jalan
- [ ] Pastikan frontend build sukses
- [ ] Jalankan smoke test `GET /api/health`
- [ ] Tambahkan endpoint `GET /api/report/{scanId}` untuk testing

## Catatan kendala
- [ ] Selesaikan setup environment Python/MSVC agar `pydantic-core` install sukses di Windows (link.exe missing)

