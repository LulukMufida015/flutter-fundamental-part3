# flutter_fundamental_3

- menerapkan jenis-jenis gesture
- menerapkan input widget dan controllernya
- menerapkan custom input dan FormField widget

## Praktikum 1: Menerapkan Gesture Detector

###  1. onTap

![Screenshoot onTap](images/gestureDetector_onTap.PNG)

Penjelasan Code : Pada kode program diatas terdapat child gestureDetector yang berisi nilai _incrementCounter yang artinya ketika gambar di-tap satu kali maka angka di bawah gambar akan terus bertambah.

### 2. onDoubleTap

![Screenshoot onDoubleTap](images/gestureDetector_onDoubleTap.PNG)

Penjelasan Code : Hal ini masih sama dengan nomor 1 namun mengubah gestureDetector menjadi onDoubleTap, sehingga angka akan berubah ketika di-tap 2x.

### 3. onLongPress

![Screnshoot onLongPress](images/gestureDetector_onLongPress.PNG)

Penjelasan Code : Hal ini masih sama dengan nomor 1 namun mengubah gestureDetector menjadi onLongPress, sehingga angka akan berubah ketika di-klik cukup panjang.

## Praktikum 2: Menerapkan Input Widget dan Forms

![Screenshoot input_widget_forms](images/input_widget_forms.PNG)

Penjelasan Code : Pada kode program tersebut langkah pertama yang dilakukan adalah membuat class FormContoh yang extends pada StatefulWidget sehingga perlu dibuatkan state di dalamnya. Kemudian langkah kedua yakni membuat class state-nya yang berisi variabel controller yang bertujuan untuk mengatur sebuah nilai dan terdapat variabel TextEditValue yang berisi "Initial Value" yang berfungsi untuk memberi nilai awal pada form tersebut. Lalu membuat variabel key yang bernilai GlobalKey yang bertujuan untuk menyimpan state dari suatu widget agar saat elemen tersebut dipindahkan ke tempat lain. Lalu membuat textValue yang berisi nilai string. Lalu Membuat initState dan juga setState. Pada build nilai yang dikembalikan adalah form, lalu membuat 2 textFormField dan juga validate yang dimana validate akan bertambah nilai true jika isi dari textFormField benar. Terakhir yakni mengubah pada bagian main dengan melakukan import dan juga pemanggilan class FormContoh.

## Praktikum 3: Menerapkan Custom Input dan FormField Widget

![Screenshoot customInput_formField](images/customInput_FormFieldWidget.PNG)

Penjelasan Code : Pada kode program di atas, langkah pertama kita membuat sebuah class VerificationCodeInput yang extends pada StatefulWidget yang terntunya harus membuat state di dalamnya. Kemudian membuat beberapa varibel dan juga constructor. Langkah kedua membuat class state-nya dan yang di-return adalah TexField yang memiliki controller dan juga input format yakni hanya berisi angka 0-9 dan diberi batasan hanya 6 angka. Lalu diatur juga untuk tata letaknya dan juga keyboard dibuat auto TextInputType agar memudahkan user. Langkah ketiga yakni membuat class VerificationCodeFormField yang extends pada FormField yang di dalamnya terdapat controller, constructor dan juga createState. Langkah keempat membuat class _VerificationCodeFormFieldState yang extends pada state yang kita buat pada langkah 3 yang berisi 3 hal yakni initState, reset dan controllerChange, dan juga dispose yang masing masing memiliki fungsi mengubah maupun menghapus. Langkah kelima menambahkan variabel controller pada main. Langkah terakhir yakni menambahkan kode program untuk membuat tampilan pada class main.