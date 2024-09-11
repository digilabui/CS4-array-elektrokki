---
title: Case Study 2 - Modular Programming

---

# Case Study 4 - Array
Pada praktikum modul 4 ini anda akan diminta untuk membuat program yang dapat melakukan invers matriks.


## Latar Belakang

Suatu hari zhavier diberi tugas oleh dosennya untuk melakukan invers matriks pada ukuran 3 x 3. Tetapi karena zhavier tahu bahwa kamu bisa melakukan programming, maka ia memintamu untuk membuat sebuah program yang dapat menyelesaikan tugas tersebut. Bantulah zhavier untuk menyelesaikannya. Good luck :+1: :+1: 

## Spesifikasi

Program dibuat dengan ketentuan sebagai berikut:

- Matriks sudah disediakan, jadi tidak perlu melakukan input matriks lagi pada program.
- Program boleh menggunakan function atau tidak.

## Isi Matrix

![image](https://hackmd.io/_uploads/Bk6GZXv3C.png)


    Kode : 
    ```
    float B[2][2] = {
        {2, 1, 1},
        {3, 2, 1},
        {1, 1, 2}
    };
    ``` 

## Rumus
- Rumus Umum
![image](https://hackmd.io/_uploads/HkU0mGw3R.png)


- Step Pengerjaan : 
    - Misal matriksnya adalah
    ![image](https://hackmd.io/_uploads/HJmIDzDnA.png)

    -    step 1, cari determinan
![image](https://hackmd.io/_uploads/SJ4wPGD20.png)


    -    step 2, cari koefesien matriks
![image](https://hackmd.io/_uploads/S17QrGwhA.png)

    -    step 3, cari adj matriks, dengan melakukan transpose pada koefesien matriks.
![image](https://hackmd.io/_uploads/H1z4HzvnA.png)


## Hint

Wah kelihatannya sulit sekali ya?? Eitss, tapi tunggu dulu, aku akan membantu kamu untuk menyelesaikan tugas tersebut. Aku akan membantumu dengan memberikanmu kode untuk mencari determinan dari matriks 3 x 3. Jangan lupa pada TP terdapat kode transpose matrix juga yang dapat digunakan pada CS ini. Semangat !!!

**Kode Koef Matrix :**
```
int determinant3x3(int matrix[3][3]) {
    int det;
    
    det = matrix[0][0] * (matrix[1][1] * matrix[2][2] - matrix[1][2] * matrix[2][1])
        - matrix[0][1] * (matrix[1][0] * matrix[2][2] - matrix[1][2] * matrix[2][0])
        + matrix[0][2] * (matrix[1][0] * matrix[2][1] - matrix[1][1] * matrix[2][0]);

    return det;
}

```

## Contoh Output

```
Matrix awal :
2 1 1
3 2 1
1 1 2

Invers Matrix :
1.5 -0.5 -0.5
-2.5 1.5 0.5
0.5 -0.5 0.5
```