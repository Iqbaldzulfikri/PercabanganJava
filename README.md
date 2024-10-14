public class percabangan1 {

    public static void main(String[] args) {
    
    // Loop untuk mencetak angka 1 sampai 6, tiga kali
    for (int i = 0; i < 3; i++) { // Mengulang sebanyak 3 kali

    for (int j = 1; j <= 6; j++) { // Mencetak angka 1 sampai 6
        System.out.print(j + " "); // Mencetak angka di baris yang sama
    }
    System.out.println(); // Pindah ke baris baru setelah mencetak 1 sampai 6
        }
    }
}


public class percabangan2{

    public static void main(String[] args) {
    
        // Loop untuk mencetak tiga baris
        for (int i = 1; i <= 3; i++) { // i akan menjadi 1, 2, dan 3
            for (int j = 1; j <= 6; j++) { // Loop untuk mencetak 6 angka
                // Menggunakan percabangan untuk menentukan angka yang dicetak
                if (j == 1) {
                    System.out.print(i + " "); // Cetak angka i untuk kolom pertama
                } else {
                    System.out.print((i + j - 1) + " "); // Cetak angka selanjutnya
                }
            }
            System.out.println(); // Pindah ke baris baru setelah mencetak angka
        }
    }
}


public class percabangan3 {

    public static void main(String[] args) {
    
        // Jumlah baris yang akan dicetak
        int rows = 6;

        // Loop untuk setiap baris
        for (int i = rows; i >= 1; i--) {
            // Loop untuk mencetak angka 1 sebanyak i kali
            for (int j = 1; j <= i; j++) {
                System.out.print("1 "); // Cetak angka 1
            }
            System.out.println(); // Pindah ke baris baru setelah mencetak angka
        }
    }
}


public class percabangan4 {

    public static void main(String[] args) {
    
        // Mengatur jumlah baris yang akan dicetak
        int rows = 3;

        // Loop untuk setiap baris
        for (int i = 1; i <= rows; i++) {
            // Loop untuk setiap kolom
            for (int j = 1; j <= 5; j++) {
                // Menggunakan percabangan untuk menentukan karakter yang dicetak
                if (i % 2 == 1) { // Baris ganjil (1 dan 3)
                    if (j % 2 == 1) { // Kolom ganjil
                        System.out.print("S "); // Cetak "S"
                    } else { // Kolom genap
                        System.out.print("0 "); // Cetak "0"
                    }
                } else { // Baris genap (2)
                    if (j % 2 == 1) { // Kolom ganjil
                        System.out.print("0 "); // Cetak "0"
                    } else { // Kolom genap
                        System.out.print("S "); // Cetak "S"
                    }
                }
            }
            System.out.println(); // Pindah ke baris baru setelah mencetak
        }
    }
}


public class percabangan5 {

    public static void main(String[] args) {
    
        // Jumlah baris yang akan dicetak
        int rows = 6;

        // Loop untuk setiap baris
        for (int i = 0; i < rows; i++) {
            // Mencetak bintang
            for (int j = 0; j < rows - i - 1; j++) {
                System.out.print("* "); // Cetak bintang
            }

            // Mencetak angka
            for (int k = rows - i - 1; k < rows; k++) {
                System.out.print(k + " "); // Cetak angka
            }

            System.out.println(); // Pindah ke baris baru setelah mencetak
        }
    }
}


public class percabangan6 {

    public static void main(String[] args) {
    
        // Menentukan jumlah elemen deret yang akan dicetak
        int n = 9;
        
        // Membuat array untuk menyimpan deret
        int[] sequence = new int[n];
        
        // Mengisi elemen pertama deret
        sequence[0] = 1; // Elemen pertama
        sequence[1] = 1; // Elemen kedua
        
        // Menghitung sisa elemen
        for (int i = 2; i < n; i++) {
            // Setiap elemen adalah jumlah dari tiga elemen sebelumnya
            sequence[i] = sequence[i - 1] + sequence[i - 2] + (i > 2 ? sequence[i - 3] : 0);
        }
        
        // Mencetak deret
        for (int i = 0; i < n; i++) {
            System.out.print(sequence[i] + " ");
        }
    }
}
