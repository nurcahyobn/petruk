# Perintah Kendali
- Dalam bab ini, Anda akan mempelajari berbagai perintah `seleksi` atau `percabangan`.
- Menerapkan dalam fungsi.

## Selection Statements 

C++ memiliki beberapa jenis `selection statements`: 

- `if` Statements, `if … else` statements, `nested if` statements 
- `switch` Statements 
- Conditional Expressions

## Perintah `if` 

```java
if (booleanExpression) { 
 statement(s); 
}
```

![if](/flowchar-if-simple.png)

Percabangan if merupakan percabangan yang hanya memiliki satu blok pilihan saat kondisi bernilai benar.

Coba perhatikan flowchart berikut ini:

![if](/flowchar-if-simple2.png)

Flowchart tersebut dapat kita baca seperti ini:

> “Jika total belanja lebih besar dari Rp 100.000, Maka tampilkan pesan Selamat, Anda dapat hadiah”

> Kalau dibawah Rp 100.000 bagaimana?

> Ya pesannya tidak akan ditampilkan.

Mari kita coba dalam program C++. Buatlah file bernama `if.cpp`, kemudian isi dengan kode berikut.



```cpp
#include <iostream>
using namespace std;

int main(){

    cout << "=== Program Pembayaran ===" << endl;
    unsigned int total_belanja;

    cout << "Masukan total belanja: ";
    cin >> total_belanja;

    // menggunakan percabangan if
    if(total_belanja > 100000){
        cout << "Selamat! anda dapat hadiah" << endl;
    }

    cout << "Terimakasih sudah berbelanja di toko kami" << endl;

    return 0;
}
```
