# Praktikum4

# Latihan
Implementasikan java code diagram class berikut:

![image](https://github.com/user-attachments/assets/100900ac-0997-40d4-9bd5-0d5b5baeb965)

# INPUT
# * Class Utama

![Screenshot 2024-10-29 103359](https://github.com/user-attachments/assets/47b094f1-0f6a-418d-b017-f001cbc4c2d3)

Penjelasan:
* public class Utama: Ini adalah definisi dari kelas utama dalam program.
* ublic static void main(String[] args): Metode main adalah titik masuk (entry point) untuk setiap aplikasi Java 
* Lingkaran lingkaran = new Lingkaran(7); membuat objek lingkaran dengan jari-jari 7.
* Segitiga segitiga = new Segitiga(5, 12); membuat objek segitiga dengan alas 5 dan tinggi 12.
* Persegi persegi = new Persegi(4); membuat objek persegi dengan panjang sisi 4.
* Program ini menggunakan System.out.println() untuk mencetak hasil perhitungan luas dan keliling untuk masing-masing objek.
* lingkaran.luas() dan lingkaran.keliling(): Menghitung luas dan keliling lingkaran.
* segitiga.luas() dan segitiga.keliling(): Menghitung luas dan keliling segitiga.
* persegi.luas() dan persegi.keliling(): Menghitung luas dan keliling persegi.

# Class Bangun Datar

![Screenshot 2024-10-29 103419](https://github.com/user-attachments/assets/4571ae05-d142-4259-b02d-53c02d45dc8f)

Penjelasan :
* abstract class BangunDatar: Ini mendefinisikan kelas BangunDatar sebagai kelas abstrak.
* public abstract float luas();: Ini adalah metode abstrak untuk menghitung luas yang harus diimplementasikan oleh semua kelas turunan.
* public abstract float keliling();: Ini adalah metode abstrak untuk menghitung keliling yang juga harus diimplementasikan oleh semua kelas turunan.

# class Lingkaran

![Screenshot 2024-10-29 103430](https://github.com/user-attachments/assets/19572364-4cc6-4357-bd41-786903d70250)

Penjelasan:
1. Pewarisan Kelas:
* Kelas Lingkaran merupakan turunan dari kelas abstrak BangunDatar, yang berarti
* kelas ini harus mengimplementasikan metode abstrak yang didefinisikan dalam BangunDatar, yaitu luas() dan keliling().

2. Atribut:
* private final int r;: Ini adalah atribut yang menyimpan nilai jari-jari lingkaran. Dideklarasikan sebagai private agar tidak dapat diakses langsung dari luar kelas. Kata kunci final menandakan bahwa nilai r tidak dapat diubah setelah diinisialisasi dalam konstruktor.

3. Konstruktor:
* public Lingkaran(int r): Konstruktor ini menerima parameter r untuk menginisialisasi atribut jari-jari. Kata kunci this digunakan untuk membedakan antara parameter r dan atribut kelas.

4. Metode luas():

@Override public float luas(): Metode ini mengimplementasikan rumus luas lingkaran dengan formula 𝜋𝑟2. Hasil perhitungan dikonversi menjadi tipe float sebelum dikembalikan.

5. Metode keliling():

@Override public float keliling(): Metode ini mengimplementasikan rumus keliling lingkaran dengan formula 2𝜋𝑟. Seperti metode luas(), hasilnya juga dikonversi menjadi tipe float.

# Class Segitiga

![Screenshot 2024-10-29 103455](https://github.com/user-attachments/assets/89a97b70-80b7-47f6-a8d3-88ae0abfb47a)

Penjelasan:

Kelas Segitiga menghitung luas dan keliling segitiga dengan atribut alas dan tinggi.

* Konstruktor: Inisialisasi alas dan tinggi untuk segitiga.
* Metode luas(): Menggunakan rumus luas = 1/2 × alas × tinggi

* Metode keliling(): Menghitung keliling dengan asumsi segitiga sama kaki, menggunakan teorema Pythagoras untuk mendapatkan panjang sisi miring:
  
  sisi miring = √(alas/2)2 + tinggi2
  
Keliling adalah alas + 2 × sisi miring
  


