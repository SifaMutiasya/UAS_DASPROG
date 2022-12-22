# Ujian Akhir Semester 
<br>Mata Kuliah : Dasar Pemrograman
<br>Nama	: Sifa Mutiasya Hendayana Puteri
<br>NIM		: 1227050125
<br>Jurusan	: Teknik Informatika (http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Pada program ini dibuat untuk memenuhi Ujian Akhir Semester (UAS) Mata Kuliah Dasar Pemrograman.
Di dalam program ini terdapat dua soal yaitu :
1. Mengubah Mengubah baris jadi kolom dan kolom jadi baris (transpose).
Program pertama ini membuat array 2 dimensi yang diinputkan baris dan kolom serta nilainya lalu ditukarkan antara baris dan kolomnya.
2. Menampilkan bilangan yang habis dibagi 3,5 dan 7.
program kedua ini sama dengan program pertama membuat array 2 dimensi lalu mencari nilai yang habis dibagi 3, 5 dan 7.

## Source Code
```
#include <iostream>
using namespace std;
int main()
{
	cout<<endl<<"\t UAS DASAR PEMOGRAMAN"<<endl;
	cout<<"\t ____________________"<<endl<<endl;
	cout<<" ====================================="<<endl;
	cout<<" Nama  : Sifa Mutiasya Hendayana Puteri"<<endl;
	cout<<" NIM   : 1227050125"<<endl;
	cout<<" Kelas : IF-C"<<endl;
	cout<<" ====================================="<<endl<<endl;

cout<<endl<<" Soal UAS No 1\n Mengubah baris jadi kolom dan kolom jadi baris (transpose) "<<endl;
int ba,ko,total;
int angka[50][50];
//input banyaknya baris dan kolom 
cout<<" Input jumlah baris : ";
cin>>ba;
cout<<" Input jumlah Kolom : ";
	cin>>ko;

//isi nilai dari kolom yang 
cout<<endl;
for (int i=1; i<=ba; i++){
	for (int j=1; j<=ko; j++ ){
		cout<< " Baris ke "<<i<<" , Kolom ke "<<j<<" : ";
		cin>>angka[i][j];
	}
	cout<<endl;
}
//hasil baris dan kolom dari angka yang telah diinputkan
cout<<" Hasil baris dan kolom yang diinputkan"<<endl;
for (int i=1; i<=ba; i++){
	for (int j=1; j<=ko; j++){
		cout<<" "<<angka[i][j]<<" ";
	}
	cout<<endl;
}
//hasil pertukaran baris dan kolom
cout<<" Hasil pertukaran baris dan kolom : "<<endl;
for (int i=1; i<=ko; i++){
	for (int j=1; j<=ba; j++){
		cout<<" "<<angka[j][i]<<" ";
	}
	cout<<endl;
}
cout<<endl<<" Soal UAS NO 2\n Menampilkan bilangan yang habis dibagi 3, 5 dan 7"<<endl;
//input banyaknya baris dan kolom 
cout<<" Input jumlah baris : ";
cin>>ba;
cout<<" Input jumlah Kolom : ";
	cin>>ko;

//isi nilai dari kolom yang 
cout<<endl;
for (int i=1; i<=ba; i++){
	for (int j=1; j<=ko; j++ ){
	cout <<"("<<i<<","<<j<<") : ";
	cin>>angka[i][j];
	}
	cout<<endl;
}
cout << " Bilangan yang habis di bagi 3,5,7 adalah : "<<endl;
// Mencetak bilangan yang habis di bagi 3
for (int i = 1; i <= ko; i++){
	for (int j = 1; j <= ba; j++){
if (angka[i][j] % 3 == 0 && angka [i][j] % 5 == 0 && angka [i][j] %7 ==0){
//menampilkan bilangan yang habis dibagi 3,5 dan 7
cout << " Angka yang habis dibagi 3,5 dan 7 : "<<angka[i][j] <<endl; 
	}
	if (angka[i][j]%3==0 && angka[i][j]%5==0){
		cout<<" Angka yang habis dibagi 3 dan 5 : "<<angka[i][j]<<endl;
	}
	else if (angka[i][j]%5==0 && angka[i][j]%7==0){
		cout<<" Angka yang habis dibagi 5 dan 7 : "<<angka[i][j]<<endl;
	}
}
  return 0;
}
}
```
## Output

<br>         UAS DASAR PEMOGRAMAN
<br>         ____________________

 <br>=====================================
 <br>Nama  : Sifa Mutiasya Hendayana Puteri
 <br>NIM   : 1227050125
 <br>Kelas : IF-C
 <br>=====================================


 <br>Soal UAS No 1
 <br>Mengubah baris jadi kolom dan kolom jadi baris (transpose)
 <br>Input jumlah baris : 3
 <br>Input jumlah Kolom : 3

 <br>Baris ke 1 , Kolom ke 1 : 2
 <br>Baris ke 1 , Kolom ke 2 : 4
 <br>Baris ke 1 , Kolom ke 3 : 5

 <br>Baris ke 2 , Kolom ke 1 : 4
 <br>Baris ke 2 , Kolom ke 2 : 7
 <br>Baris ke 2 , Kolom ke 3 : 8

 <br>Baris ke 3 , Kolom ke 1 : 7
 <br>Baris ke 3 , Kolom ke 2 : 5
 <br>Baris ke 3 , Kolom ke 3 : 4

 <br>Hasil baris dan kolom yang diinputkan
 <br>2  4  5
 <br>4  7  8
 <br>7  5  4
 <br>Hasil pertukaran baris dan kolom :
 <br>2  4  7
 <br>4  7  5
 <br>5  8  4

 <br>Soal UAS NO 2
 <br>Menampilkan bilangan yang habis dibagi 3, 5 dan 7
 <br>Input jumlah baris : 2
 <br>Input jumlah Kolom : 2

<br>(1,1) : 105
<br>(1,2) : 457

<br>(2,1) : 340
<br>(2,2) : 430

 <br>Bilangan yang habis di bagi 3,5,7 adalah :
 <br>Angka yang habis dibagi 3,5 dan 7 : 105

<br>--------------------------------
