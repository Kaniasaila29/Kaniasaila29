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

		cout << "		      UJIAN AKHIR SEMESTER				"<<endl;
		cout << "==============================================================="<<endl;
		cout << "Nama : Kania Sailanul Anjani "<<endl;
		cout << "NIM  : 1227050064 "<<endl;
		cout << "==============================================================="<<endl;
		cout << "No.1 Mengubah baris jadi kolom dan kolom jadi baris (transpose)" << endl;
		cout << "==============================================================="<<endl;
		cout << "Masukkan jumlah baris matriks: ";
		cin >> m;
		cout << "Masukkan jumlah kolom matriks: ";
		cin >> n;
		
		cout<<endl;

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
		
		cout<<endl;

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
		cout << "====================================================="<<endl;
		cout << "No.2 Menampilkan bilangan yang habis dibagi 3,5,dan 7"<<endl;
		cout << "====================================================="<<endl;
		
		int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

		cout<<"Input jumlah baris: "; cin>>jumlahBaris;
		cout<<"Input jumlah kolom: "; cin>>jumlahKolom;
		cout << endl;

		for(i = 0; i < jumlahBaris; i++){
	      	for(j = 0; j < jumlahKolom; j++){
		cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
		cin >> arr[i][j];
		}
		cout << endl;
		}

	 	cout << "Hasil matriks: " << endl;

		for(i = 0; i < jumlahBaris ; i++){
		for(j = 0; j < jumlahKolom; j++){
		cout << arr[i][j] << " ";
		}
		cout << endl;
		}

		cout << "\nBilangan yang habis dibagi 3,5,dan 7: " << endl;

		for(i = 0; i < jumlahBaris ; i++){
		for(j = 0; j < jumlahKolom; j++){
	 	if(arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0){
		cout << arr[i][j] << " ";
		}
		}
		cout << endl;
		}
		
		cout << endl;
		return 0;
		}
		
## Output

			               UJIAN AKHIR SEMESTER
		===============================================================
		Nama : Kania Sailanul Anjani
		NIM  : 1227050064
		===============================================================
		No.1 Mengubah baris jadi kolom dan kolom jadi baris (transpose)
		===============================================================
		Masukkan jumlah baris matriks: 2
		Masukkan jumlah kolom matriks: 2

		Masukkan Nilai-Nilai Matriks
		Baris ke 1, Kolom ke 1 : 3
		Baris ke 1, Kolom ke 2 : 7
		Baris ke 2, Kolom ke 1 : 5
		Baris ke 2, Kolom ke 2 : 8

		Hasil dari matriks yang diinputkan :
		3       7
		5       8

		Hasil Transpose Matriks:
		3       5
		7       8

		=====================================================
		No.2 Menampilkan bilangan yang habis dibagi 3,5,dan 7
		=====================================================
		Input jumlah baris: 2
		Input jumlah kolom: 2

		Baris 1, kolom 1 = 3
		Baris 1, kolom 2 = 5

		Baris 2, kolom 1 = 7
		Baris 2, kolom 2 = 9

		Hasil matriks:
		3 5
		7 9

		Bilangan yang habis dibagi 3,5,dan 7:
		3 5
		7 9


		--------------------------------
		Process exited after 8.209 seconds with return value 0
		Press any key to continue . . .
