# Struct atau Record

1. Menjelaskan cara mendeklarasikan struct/record .
2. Menjelaskan cara menginisialisasi struct/record.
3. Menjelaskan cara mengakses elemen struct/record.
4. Menjelaskan perbedaan array dari struktur (array of struct).

Struct/Record adalah tipe terstruktur yang terdiri atas sejumlah elemen yang tipenya tidak harus sama.
Struct/Record  koleksi satuan data yang heterogen, yakni terdiri dari berbagai type: int, float, char, dan lainnya

Record yang berisi record lain dikenal sebagai field (elemen dalam suatu record).
Sejumlah elemen dalam record (field) dikenal dengan Array
Setiap field boleh berbeda tipe datanya.


* Tipe data record adalah tipe data khusus yang komponennya terdiri dari berbagai jenis tipe data lain. Sebuah record berisi beberapa variabel lain yang ‘dipaketkan’. Konsep struktur data seperti ini sedikit mirip dengan konsep object dalam bahasa pemrograman modern (walaupun di dalam pascal juga terdapat konsep tentang object).
* Record juga mirip dengan array, dimana kita bisa membuat sebuah variabel yang berisi berbagai element. Perbedaannya, record bisa menampung berbagai jenis tipe data, tidak hanya 1 tipe data seperti array.

```c++
struct <namatipe>
{
    <typedata1> <namavar1>; 
    <typedata2> <namavar2>;
    ...
};
```

Tabel : Mahasiswa
nama | usia
--- | ---
Agus |Salim
23 |22

* nama merupakan variabel  bertipe char atau string. 
* usia merupakan variabel  bertipe int.

```c++
// file: mahasiswa.cpp
#include <iostream>
#include <string.h>
using namespace std;

struct Mahasiswa {
    char nama[30];
    int usia;
};

int main(){
    Mahasiswa mhs1;

    // initialisi atau input data
    strcpy(mhs1.nama, "Agus");
    mhs1.usia = 23;

    // output
    cout << "\nRecord Data Mahasiswa\n";
    cout << mhs1.nama << " berusia " << mhs1.usia << " tahun\n";
    return 0;
}
```
