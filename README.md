# Pemrograman Terstruktur


### Pert-1: Pengantar

### Pert-2: Perulangan (*Looping*)

### Pert-3: [Menggunakan Fungsi (*Function*)](/fungsi.md)

### Pert-4: [Kendali perintah](/kendal.md)

### Pert-5: [Struct atau Record](/struct.md)

## Pert-6: Evaluasi dan Diskusi (Quis)

> Perulangan for `1 2 3 4 5`

```c++
#include <iostream>
 
using namespace std;
 
int main() {
    for (int i = 1; i <= 5; ++i) {
        cout << i << " ";
    }
}
```

> Fungsi dengan data `int` untuk penjumlahan

```c++
#include <iostream>

using namespace std;

//fungsi penjumlahan dengan tipe int
int Tambah (int a, int b){
    return (a + b);
}

int main() {
    int saldo_awal, setor, saldo;
    saldo_awal = 70000;
    
    cout << "saldo awal\t: Rp." << saldo_awal << endl;
    cout << "input setor\t: Rp.";
    cin  >> setor;
    
    cout << "total saldo\t: Rp." << Tambah (saldo_awal, setor);
}
```

> Struct atau Record `Tabungan Nasabah` dan hasil

namanasabah | saldo_awal | setor | fungsi `Tambah`
--- | --- | --- | --- | 
nurcahyo | 70000 | 25000 | 85000

> QUIS-1 struct `Pinjaman`

? | ? | ? | fungsi `Angsuran`
--- | --- | --- | --- | 
? | ? | ? | ?

