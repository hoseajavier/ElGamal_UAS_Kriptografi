# ElGamal_UAS_Kriptografi

# Deskripsi
Algoritma ElGamal adalah algoritma kriptografi asimetris yang digunakan untuk enkripsi dan dekripsi data, serta untuk tanda tangan digital. Algoritma ini didasarkan pada prinsip Logaritma Diskrit dalam teori bilangan, yang membuatnya sulit dipecahkan dengan komputasi modern. Algoritma ini diperkenalkan oleh Tahar Elgamal pada tahun 1985.

# Komponen Utama Algoritma ElGamal
1. Kunci Publik dan Privat:
Kunci publik digunakan untuk enkripsi.
Kunci privat digunakan untuk dekripsi.

2. Bilangan Prima (p):
Sebuah bilangan prima besar digunakan sebagai basis operasi modular.

3. Generator (g):
Sebuah bilangan yang menjadi akar primitif modulo p, digunakan untuk menghasilkan kunci publik.

4. Pilih bilangan acak x (untuk private key) 
dengan 1 <= x <= p – 1

5. Hitung kunci publik y = g^x mod p. 

# Enkripsi
Mengambil nilai k secara acak, dengan k bernilai 
1 <= k <= p–1 (juga ada yang menulis sampai p-2)
Menghitung nilai C1 dan C2, yang mana : 
C1   = g^k mod p 
C2  = M.y^k mod p
Jadi, ciphertext C yang dikirimkan adalah satu pasangan dengan dua nilai C1 dan C2 (terpisah).

# Dekripsi
Menghitung nilai C1x , yang mana :
 	C1^x = (C1)^x mod p
Menghitung nilai M = C2(C1^x)^-1 mod p

Jadi, plaintext yg dikirimkan adalah satu huruf dari pasangan chipertext C1 dan C2 yaitu nilai M
