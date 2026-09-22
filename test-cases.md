# Testing

## Test Case 1: Pembelian Single Item Tanpa Diskon

**Input:**
- Nama barang: `buku`
- Harga barang: `10000`
- Jumlah barang: `2`
- Tambah barang lagi?: `n`
- Uang dibayar: `50000`

**Expected Output:**
- Total sebelum diskon: Rp 20000
- Diskon (0%): Rp 0
- Total akhir: Rp 20000
- Uang kembali: Rp 30000

**Actual Output:**
- Total sebelum diskon: Rp 20000
- Diskon (0%): 0
- Total akhir: Rp 20000
- Uang kembali: Rp 30000

**Status:** PASS

---

## Test Case 2: Pembelian Single Item Dengan Diskon 5%

**Input:**
- Nama barang: `pulpen`
- Harga barang: `20000`
- Jumlah barang: `3`
- Tambah barang lagi?: `n`
- Uang dibayar: `100000`

**Expected Output:**
- Total sebelum diskon: Rp 60000
- Diskon (5%): Rp 3000
- Total akhir: Rp 57000
- Uang kembali: Rp 43000

**Actual Output:**
- Total sebelum diskon: Rp 60000
- Diskon (5%): 3000
- Total akhir: Rp 57000
- Uang kembali: Rp 43000

**Status:** PASS

---

## Test Case 3: Pembelian Single Item Dengan Diskon 10%

**Input:**
- Nama barang: `sepatu`
- Harga barang: `150000`
- Jumlah barang: `1`
- Tambah barang lagi?: `n`
- Uang dibayar: `200000`

**Expected Output:**
- Total sebelum diskon: Rp 150000
- Diskon (10%): Rp 15000
- Total akhir: Rp 135000
- Uang kembali: Rp 65000

**Actual Output:**
- Total sebelum diskon: Rp 150000
- Diskon (10%): 15000
- Total akhir: Rp 135000
- Uang kembali: Rp 65000

**Status:** PASS

---

## Test Case 4: Pembelian Multiple Items

**Input:**
- Barang 1: `pensil`, Harga: `5000`, Jumlah: `2`
- Tambah barang lagi?: `y`
- Barang 2: `map`, Harga: `10000`, Jumlah: `4`
- Tambah barang lagi?: `n`
- Uang dibayar: `50000`

**Expected Output:**
- Total sebelum diskon: Rp 50000
- Diskon (5%): Rp 2500
- Total akhir: Rp 47500
- Uang kembali: Rp 2500

**Actual Output:**
- Total sebelum diskon: Rp 50000
- Diskon (5%): 2500
- Total akhir: Rp 47500
- Uang kembali: Rp 2500

**Status:** PASS

---

## Test Case 5: Pembayaran Kurang (Validasi Input Uang)

**Input:**
- Nama barang: `baju`
- Harga barang: `50000`
- Jumlah barang: `1`
- Tambah barang lagi?: `n`
- Uang dibayar (1): `40000`
- Uang dibayar (2): `50000`

**Expected Output:**
- Menampilkan pesan error "Uang pembayaran kurang! Silakan coba lagi."
- Meminta input ulang uang pembayaran
- Uang kembali: Rp 2500

**Actual Output:**
- Menampilkan pesan "Uang pembayaran kurang! Silakan coba lagi."
- Menerima input `50000` dan menampilkan Uang kembali: Rp 2500

**Status:** PASS
