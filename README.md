## Ujian Akhir Semester 
<br> Mata Kuliah : Dasar Pemrograman
<br> Nama        : Kania Sailanul Anjani
<br> NIM         : 1227050064
<br> Jurusan     : [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum

Matriks adalah suatu susunan bilangan real atau bilangan kompleks (atau elemen-elemen) yang disusun dalam baris dan kolom sehingga membentuk jajaran persegi panjang. Suatu matriks diberi nama dengan menggunakan huruf kapital seperti A, B, C, dan seterusnya, sedangkan anggotanya dinyatakan dengan huruf kecil.
Transpose matriks adalah matriks baru yang diperoleh dengan cara menukar elemen-elemen baris menjadi elemen kolom atau sebaliknya.

## Source Code

		#include<iostream>
		using namespace std;


		int main()
		{
		int m, n;

		cout << "UAS"<<endl;
		cout << "===="<<endl;
		cout << "Nama : Kania Sailanul Anjani "<<endl;
		cout << "NIM  : 1227050064 "<<endl;
		cout << "======================================"<<endl<<endl<<endl;
		//mengubah baris jadi kolom dan kolom jadi baris (tranpose)//
		cout << "No.1 Mengubah baris jadi kolom dan kolom jadi baris (transpose)" << endl;
		cout << "==============================================================="<<endl;
		cout << "Masukkan jumlah baris matriks: ";
		cin >> m;
		cout << "Masukkan jumlah kolom matriks: ";
		cin >> n;

		int matriks[m][n], transpose[n][m];

		cout << "Masukkan Nilai-Nilai Matriks\n";
		for (int i = 0; i < m; i++)
		{
			for (int j = 0; j < n; j++)
			{
				cout <<"Baris ke "<<i+1<<", Kolom ke "<<j+1<<" : ";
				cin  >> matriks[i][j];
			}
		}

		cout << "Hasil dari matriks yang diinputkan :\n";
		for (int i = 0; i < m; i++)
		{
			for (int j = 0; j < n; j++)
			{
				cout << matriks[i][j] << "\t";
			}
			cout << endl;
		}
		cout << endl;

		for (int i = 0; i < m; i++)
		{
			for (int j = 0; j < n; j++)
			{
				transpose[j][i] = matriks[i][j];
			}
		}

		cout << "Hasil Transpose Matriks: \n";
		for (int i = 0; i < n; i++)
		{
			for (int j = 0; j < m; j++)
			{
				cout << transpose[i][j] << "\t";
			}
			cout << endl;
		}
		cout <<endl;
		//menampilkan bilangan yang habis dibagi 3,5,dan 7//
		cout << "No.2 Menampilkan bilangan yang habis dibagi 3, 5 dan 7" << endl;
		cout << "==============================================================="<<endl;
		cout << "Masukkan jumlah baris matriks: ";
		cin >> m;
		cout << "Masukkan jumlah kolom matriks: ";
		cin >> n;

		cout << "Masukkan Nilai-Nilai\n";
		for (int i = 0; i < m; i++)
		{
			for (int j = 0; j < n; j++)
			{
				cout <<"("<<i+1<<","<<j+1<<") : ";
				cin  >> matriks[i][j];
			}
		}
		cout << endl;

		bool cek = true;
		cout << "Nilai yang tidak bisa dibagi 3, 5, 7 yaitu :";
		for (int i = 0; i < m; i++)
		{
			for (int j = 0; j < n; j++)
			{
				if (matriks[i][j]%3!=0 && matriks[i][j]%5!=0 && matriks[i][j]%7!=0)
				{
					cout << " " << matriks[i][j];
					cek = false;
				}
			}
		}
		if (cek)
		{
			cout << " Nilai yang anda input bisa dibagi 3, 5 dan 7" <<endl;
		}
		return 0;

		}

## Output

UAS
====
Nama : Kania Sailanul Anjani
NIM  : 1227050064
======================================
No.1 Mengubah baris jadi kolom dan kolom jadi baris (transpose)
===============================================================
Masukkan jumlah baris matriks: 4
Masukkan jumlah kolom matriks: 3
Masukkan Nilai-Nilai Matriks
Baris ke 1, Kolom ke 1 : 5
Baris ke 1, Kolom ke 2 : 6
Baris ke 1, Kolom ke 3 : 7
Baris ke 2, Kolom ke 1 : 8
Baris ke 2, Kolom ke 2 : 4
Baris ke 2, Kolom ke 3 : 5
Baris ke 3, Kolom ke 1 : 3
Baris ke 3, Kolom ke 2 : 2
Baris ke 3, Kolom ke 3 : 1
Baris ke 4, Kolom ke 1 : 5
Baris ke 4, Kolom ke 2 : 7
Baris ke 4, Kolom ke 3 : 9
Hasil dari matriks yang diinputkan :
5       6       7
8       4       5
3       2       1
5       7       9

Hasil Transpose Matriks:
5       8       3       5
6       4       2       7
7       5       1       9

No.2 Menampilkan bilangan yang habis dibagi 3, 5 dan 7
===============================================================
Masukkan jumlah baris matriks: 4
Masukkan jumlah kolom matriks: 3
Masukkan Nilai-Nilai
(1,1) : 5
(1,2) : 7
(1,3) : 8
(2,1) : 9
(2,2) : 4
(2,3) : 3
(3,1) : 5
(3,2) : 9
(3,3) : 7
(4,1) : 2
(4,2) : 1
(4,3) : 6

Nilai yang tidak bisa dibagi 3, 5, 7 yaitu : 8 4 2 1
--------------------------------
Process exited after 21.84 seconds with return value 0
Press any key to continue . . .
