# Install Guide (Windows)

## Masalah umum
- `pydantic-core` gagal build karena `link.exe` tidak ditemukan.
- Biasanya perlu MSVC Build Tools.

## Opsi paling simpel
1. Install **Build Tools for Visual Studio**
2. Pilih workload: **Desktop development with C++**
3. Pastikan komponen C++ build tools terpasang (supaya `link.exe` ada)

## Validasi setelah install
Jalankan:
```bat
where python
python --version
pip --version
cd backend
python -m venv .venv
.\.venv\Scripts\activate
pip install -r requirements.txt
```

