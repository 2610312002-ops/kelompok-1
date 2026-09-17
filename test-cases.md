# Testing

## Test Case 1: Pembelian Tanpa Diskon (< Rp 50.000)

*Input:*  
- Barang 1: buku (Harga: 10000, Qty: 2) -> Subtotal: 20000  
- Tambah barang lagi?: n  
- Uang dibayar: 50000  

*Expected Output:*  
Total sebelum diskon : 20000  
Diskon (0%): 0  
Total akhir : 20000  
Uang dibayar : 50000  
Uang kembali : 30000  

*Actual Output:*  
Total sebelum diskon : 20000  
Diskon (0%): 0  
Total akhir : 20000  
Uang dibayar : 50000  
Uang kembali : 30000  

*Status:* PASS

---

## Test Case 2: Pembelian Diskon 5% (Rp 50.000 - Rp 99.000)

*Input:*  
- Barang 1: pulpen (Harga: 20000, Qty: 3) -> Subtotal: 60000  
- Tambah barang lagi?: n  
- Uang dibayar: 100000  

*Expected Output:*  
Total sebelum diskon : 60000  
Diskon (5%): 3000  
Total akhir : 57000  
Uang dibayar : 100000  
Uang kembali : 43000  

*Actual Output:*  
Total sebelum diskon : 60000  
Diskon (5%): 3000  
Total akhir : 57000  
Uang dibayar : 100000  
Uang kembali : 43000  

*Status:* PASS

---

## Test Case 3: Pembelian Diskon 10% (>= Rp 100.000)

*Input:*  
- Barang 1: sepatu (Harga: 150000, Qty: 1) -> Subtotal: 150000  
- Tambah barang lagi?: n  
- Uang dibayar: 200000  

*Expected Output:*  
Total sebelum diskon : 150000  
Diskon (10%): 15000  
Total akhir : 135000  
Uang dibayar : 200000  
Uang kembali : 65000  

*Actual Output:*  
Total sebelum diskon : 150000  
Diskon (10%): 15000  
Total akhir : 135000  
Uang dibayar : 200000  
Uang kembali : 65000  

*Status:* PASS

---

## Test Case 4: Multiple Items (Lebih dari 1 Barang)

*Input:*  
- Barang 1: pensil (Harga: 5000, Qty: 2) -> Subtotal: 10000  
- Tambah barang lagi?: y  
- Barang 2: map (Harga: 10000, Qty: 4) -> Subtotal: 40000  
- Tambah barang lagi?: n  
- Uang dibayar: 50000  

*Expected Output:*  
Total sebelum diskon : 50000  
Diskon (5%): 2500  
Total akhir : 47500  
Uang dibayar : 50000  
Uang kembali : 2500  

*Actual Output:*  
Total sebelum diskon : 50000  
Diskon (5%): 2500  
Total akhir : 47500  
Uang dibayar : 50000  
Uang kembali : 2500  

*Status:* PASS

---

## Test Case 5: Penanganan Uang Pembayaran Kurang

*Input:*  
- Barang 1: baju (Harga: 50000, Qty: 1) -> Subtotal: 50000  
- Tambah barang lagi?: n  
- Uang dibayar (1): 40000 (Kurang)  
- Uang dibayar (2): 50000 (Cukup)  

*Expected Output:*  
Uang pembayaran kurang! Silakan coba lagi.  
Uang dibayar : 50000  
Uang kembali : 2500  

*Actual Output:*  
Uang pembayaran kurang! Silakan coba lagi.  
Uang dibayar : 50000  
Uang kembali : 2500  

*Status:* PASS
