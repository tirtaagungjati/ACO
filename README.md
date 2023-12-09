# ACO
Penerapan Ant Colony Optimization Dalam Mencari Jalur Terpendek

Berikut List Jarak Yang Ada
distances = np.array([
    [0, 10, 175, 400, 500],  # Titik 0 Jarak Indonesia ke negara lainnya 
    [10, 0, 23, 350, 600],    # Titik 1 Jarak Singapura ke negara lainnya 
    [175, 23, 0, 400, 500],    # Titik 2 Jarak Malaysia ke negara lainnya 
    [400, 350, 400, 0, 800],    # Titik 3 Jarak Jepang ke negara lainnya 
    [500, 600, 500, 800, 0]    # Titik 4 Jarak Australia ke negara lainnya 
])

route = [
    (113.9213, -0.7893),  # Koordinat Indonesia Titik 0
    (103.8198, 1.3521),  # Koordinat Singapura Titik 1
    (101.9758, 4.2105),  # Koordinat Malaysia Titik 2
    (138.2529, 36.2048),  # Koordinat Jepang Titik 3
    (133.7751, -25.2744)   # Koordinat Australia Titik 4
]

Dengan Algoritma ACO didapatkan Hasil Rute Terpendek yaitu
Shortest path: [4, 0, 1, 2, 3]
Shortest distance: 933
Total distance via shortest path: 8281895.57 m

Dengan Gambar Sebagai Berikut:
![image](https://github.com/tirtaagungjati/ACO/blob/main/output_ACO.png)

Penjelasan Shortest Path: 
Dari Negara Australia (Titik 4) menuju Indonesia (Titik 0) setelah itu menuju ke Singapura (Titik 1) setelah itu menuju ke Malaysia (Titik 2) setelah itu menuju ke Jepang (Titik 3)
Penjelasan Shortest distance:
Dikarenakan jarak yang paling pendek yaitu : 500 + 10 + 23 + 400 = 933


Jika Dilihat Menghitung Manual Dengan Rute Terpanjang didapatkan
Rute terpanjang yang dihasilkan adalah [0, 3, 4, 1, 2]
Total jarak = Jarak dari Indonesia ke Jepang + Jarak dari Jepang ke Australia + Jarak dari Australia ke Singapura + Jarak dari Singapura ke Malaysia
Total jarak = 400 + 800 + 600 + 23
Total jarak = 1823

Maka Algoritma ACO ini sukses mencari Rute Terpendek