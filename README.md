#   Percobaan 1

##  Soal

1.	Jelaskan perbedaan struktur dan mekanisme traversal antara Single Linked List dan Double Linked List!
2.	Perhatikan class Node, di dalamnya terdapat atribut next dan prev. Jelaskan fungsi masing-masing atribut tersebut pada proses traversal dan manipulasi node!
3.	Perhatikan konstruktor pada class DoubleLinkedList. Jelaskan fungsi konstruktor tersebut terhadap kondisi awal linked list!
4.	Perhatikan potongan kode berikut:

    ```java
        if (isEmpty()) {
            head = tail = newNode;
        }        
    ```
Mengapa head dan tail harus menunjuk node yang sama ketika linked list masih kosong?

5.	Modifikasi method print() agar menampilkan pesan "Linked List masih kosong" ketika tidak terdapat data pada linked list!
6.	Modifikasi kode program dengan menambahkan method printReverse() untuk menampilkan seluruh data pada Double Linked List secara terbalik, dimulai dari node tail menuju head!

---

##  Jawaban

1.  Perbedaan utamanya terletak pada arah penelusuran (traversal), di mana Single Linked List hanya bisa ditelusuri satu arah dari depan ke belakang karena setiap node hanya memiliki pointer next, sedangkan Double Linked List dapat ditelusuri secara dua arah (maju dan mundur) karena setiap node dilengkapi dengan pointer next dan prev.
2.  Pada proses traversal dan manipulasi node, atribut next berfungsi untuk menyimpan referensi atau alamat dari node berikutnya agar penelusuran bisa bergerak maju, sementara atribut prev berfungsi untuk menyimpan referensi dari node sebelumnya sehingga penelusuran bisa bergerak mundur dengan mudah.
3.  Konstruktor pada class DoubleLinkedList berfungsi untuk menginisialisasi kondisi awal objek saat pertama kali dibuat, yaitu dengan mendeklarasikan pointer head dan tail bernilai null untuk memastikan bahwa linked list berada dalam keadaan benar-benar kosong.
4.  Pointer head dan tail harus menunjuk ke node yang sama ketika linked list masih kosong karena node baru yang dimasukkan (newNode) merupakan satu-satunya node yang ada di dalam list tersebut, sehingga node itu bertindak sebagai elemen pertama (head) sekaligus elemen terakhir (tail).
5.  Untuk memodifikasi method print(), kita perlu menambahkan pengecekan kondisi list pada baris paling atas menggunakan blok kode if (isEmpty()) { System.out.println("Linked List masih kosong."); return; } agar program langsung menampilkan pesan dan berhenti mengeksekusi perulangan di bawahnya jika tidak ada data.
6.  Untuk menampilkan data secara terbalik, kita dapat menambahkan method public void printReverse() yang melakukan inisialisasi awal pada pointer bagian belakang dengan Node current = tail;, kemudian melakukan perulangan while (current != null) yang mencetak data dan bergerak mundur menggunakan perintah current = current.prev;.

---

#   Percobaan 2

##  Soal

---

##  Jawaban

---