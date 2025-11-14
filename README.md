
---

# ✅ **Studi Kasus Lengkap: Program Penghitung Diskon**

## 📌 **Deskripsi Program**

Program meminta user memasukkan:

* Harga barang
* Persentase diskon

Lalu program akan menghitung dan menampilkan harga akhir setelah diskon menggunakan **function terpisah**.

---

# ✅ **Kode Java Lengkap**

```java
import java.util.Scanner;

public class PenghitungDiskon {

    // Function untuk menghitung harga setelah diskon
    static double hitungDiskon(double harga, double persenDiskon) {
        double potongan = harga * (persenDiskon / 100);
        return harga - potongan;
    }

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        // Input harga barang
        System.out.print("Masukkan harga barang: ");
        double harga = input.nextDouble();

        // Input persentase diskon
        System.out.print("Masukkan diskon (%): ");
        double diskon = input.nextDouble();

        // Memanggil function hitungDiskon
        double hargaSetelahDiskon = hitungDiskon(harga, diskon);

        // Output hasil
        System.out.println("-----------------------------");
        System.out.println("Harga awal          : " + harga);
        System.out.println("Diskon              : " + diskon + "%");
        System.out.println("Harga setelah diskon: " + hargaSetelahDiskon);
    }
}
```

---

# ✅ **Penjelasan Function**

```java
static double hitungDiskon(double harga, double persenDiskon)
```

### Fungsi ini:

* menerima **harga** dan **persenDiskon**
* menghitung potongan = harga × (diskon/100)
* mengembalikan harga final setelah diskon

---

# ✅ **Contoh Output**

```
Masukkan harga barang: 150000
Masukkan diskon (%): 25
-----------------------------
Harga awal          : 150000.0
Diskon              : 25.0%
Harga setelah diskon: 112500.0


