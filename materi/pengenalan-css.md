CSS adalah kependekan dari Cascading Style Sheet. CSS merupakan kumpulan kode-kode yang bertujuan untuk menghias dan mengatur gaya tampilan/layout halaman web supaya lebih elegan dan menarik. CSS adalah sebuah teknologi internet yang direkomendasikan oleh World Wide Web Consortium atau W3C pada tahun 1996. Awalnya, CSS dikembangkan di SGML pada tahun 1970, dan terus dikembangkan hingga saat ini. CSS telah mendukung banyak bahasa markup seperti HTML, XHTML, XML, SVG (Scalable Vector Graphics) dan Mozilla XUL (XML User Interface Language).

Pada desember 1996, W3C memperkenalkan Level 1 spesifikasi CSS atau juga dikenal CSS1 yang mendukung format, warna font teks, dan lain-lain. Kemudian, Mei 1998, W3C menerbitkan CSS2 yang di dalamnya diatur fungsi peletakan elemen. Dan sekarang, W3C telah memperbaiki dan meningkatkan Kemampuan CSS2 ke  CSS3.

CSS digunakan oleh web programmer dan juga blogger untuk menentukan warna, tata letak font, dan semua aspek lain dari presentasi dokumen di situs mereka. Saat ini, hampir tidak ada situs web yang dibangun tanpa kode css.

Sebagai blogger, Anda juga harus tahu apa itu CSS dan bagaimana menggunakannya agar mudah untuk merancang blog anda. Kode CSS membuat pembaca blog kita menjadi nyaman dan betah berlama-lama di blog kita sehingga pageviews situs kitapun meningkat. Namun, itu semua tergantung bagaimana kita menggunakannya sehingga bisa memikat pengunjung. Untuk itulah serial tutorial ini dibuat 🙂 .

PENGENALAN DASAR
Cascading Style Sheet terdiri dari Selektor, deklarasi, Properti dan Nilai. Seperti pada HTML, PHP dan bahasa pemrograman lainnya, CSS juga memiliki aturan yang menulis itu sendiri.
Contoh penulisan kode css :

Body {background-color: white;}
"Body" adalah Selektor,
"{ }" adalah deklarasi, 
"background-color" adalah properti dan 
"white" adalah nilai. 
Maksud dari kode diatas adalah mengatur warna latar belakang (background color) dari tag "Body" sebuah halaman web.

CARA-CARA PENGGUNAAN CSS
Untuk latihan penggunaan CSS, langkah pertama yang harus anda lakukan adalah membuat file  dengan menggunakan Software kode editor seperti Notepad, lalu namai file dengan format ?.html?. Lalu praktekkanlah cara-cara berikut ini. Ada 3 cara untuk menggunakan kode CSS di situs Anda.

1. CSS sebagai atribut/elemen/bagian dari tag HTML.
<div style="padding: 5px 20px;"

"Div" adalah tag html/Mark up yang dihiasi oleh kode css. kode cssnya adalah style ="padding: 5px 20px;". Cara ini biasanya dipakai jika kode cssnya sedikit.

2. CSS dalam tag <style type='text/css'> (Kode CSS) </ style>.

Kode css terletak antara tag 'style' yang biasanya diletakkan dibawah elemen <title></title>
Dengan cara ini anda harus menentukan nama selektor. 

<style type='text/css'>
	table{
		padding:5px;
	}
</ style>

3. CSS sebagai file terpisah.

<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/jstree/3.2.1/themes/default/style.min.css" />

Kode diatas adalah kode html untuk memanggil kode css yang terpisah. Kode itu biasanya diletakkan dibawah elemen <title></title> pada sebuah file html. Dalam cara 3 ini, kode css berada pada file .css yang dibuat dengan cara yang sama yaitu dengan sofware notepad, namun diberi format .css.

Untuk Latihan cara 3 ini silahkan anda buat folder. Dalam folder itu anda buat lagi file .html, misalnya latihan.html . Lalu buat file css-nya misalnya style.css.

Dalam file latihan.html, silahkan ketikkan kode dibawah ini :

<html>
<head>
<title>Latihan</title>
<link rel='stylesheet' href='style.css' type='text/css'/>
</head>
<body>
<div class='download'>
<a href="#">Download</a>
</div>
</body>
<html>

 
Simpan, lalu buka di browser. File .html anda belum dihias karena kita belum menambahkan kode css kedalam file style.css. Jadi, silahkan masukkan kode seperti dibawah ini, tentu anda bisa merubah-rubahnya :

.download {
padding:5px 20px;
background:#000;
border:1px solid auto;
text-transform:uppercase;
font-size:20px;
}
setelah itu simpan, lalu refresh file latihan.html yang sedang dibuka di browser

Selamat mencoba 🙂 .

Keterangan :
Cara 1 dan 2 sebagian besar digunakan dalam blog blogspot/blogger. Sedangkan, Cara 3  biasanya digunakan dalam situs web berbasis wordpress ataupun yang lainnya, karena membutuhkan ruang untuk menyimpan file css.

Jika menggunakan cara2 dan 3, Anda harus melengkapi tag html yang akan anda hias dengan atribut ?id? atau ?class?. Ini adalah  2 cara untuk penamaan selektor pada kode css. Jika menggunakan atribut 'id' (misal: <div id='download'></div>), maka selektor dalam kode cssnya adalah sebagai berikut :

#download {
Properti:nilai;
}
Sedangkan, jika menggunakan atribut 'class' (misal:<div class='download'></div>), maka selektor dalam kode cssnya adalah sebagai berikut :

.download {
Properti:nilai;
}
Dengan kata lain, hanya dibedakan dengan tanda '# dan '.' .

Nah, lalu jika anda ingin menghias tag tertentu dalam file html, misalnya seluruh tag h1 yang ada, Maka anda dapat menuliskan selektornya tanpa menggunakan tanda apapun. Seperti ini :

h1 {
properti:nilai;
}