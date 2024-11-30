# Kikiyan-Himmatal-Ulya_23030630013_MatB

# Final Projek APLIKOM
Nama  :Kikiyan Himmatal Ulya


NIM   :23030630013


Kelas :Matematika B


# EMT untuk Perhitungan Aljabar

Pada notebook ini Anda belajar menggunakan EMT untuk melakukan
berbagai perhitungan terkait dengan materi atau topik dalam Aljabar.

## Contoh pertama
Menyederhanakan bentuk aljabar:
$$6x^{-3}y^5\times -7x^2y^{-9}$$

$$6\*x^(-3)\*y^5\*-7\*x^2\*y^(-9)$$

$$-\frac{42}{x\,y^4}##Menjabarkan:

$$(6x^{-3}+y^5)(-7x^2-y^{-9})

$$\>$&showev('expand((6\*x^(-3)+y^5)\*(-7\*x^2-y^(-9))))

$${\it expand}\left(\left(-\frac{1}{y^9}-7\,x^2\right)\,\left(y^5+
 \frac{6}{x^3}\right)\right)=-7\,x^2\,y^5-\frac{1}{y^4}-\frac{6}{x^3
 \,y^9}-\frac{42}{x}$$## Baris Perintah

Baris perintah Euler terdiri dari satu atau beberapa perintah Euler
diikuti dengan titik koma ";" atau koma ",". Titik koma mencegah
pencetakan hasil. Koma setelah perintah terakhir dapat dihilangkan.


Baris perintah berikut hanya akan mencetak hasil ekspresi, bukan
penugasan atau perintah format.


\>r:=2; h:=4; pi\*r^2\*h/3


    16.7551608191

Perintah harus dipisahkan dengan kosong. Baris perintah berikut
mencetak dua hasilnya.


\>pi\*2\*r\*h, %+2\*pi\*r\*h // Ingat tanda % menyatakan hasil perhitungan terakhir sebelumnya


    50.2654824574
    100.530964915

Baris perintah dijalankan dalam urutan pengguna menekan return. Jadi
Anda mendapatkan nilai baru setiap kali Anda mengeksekusi baris kedua.


\>x := 1;

\>x := cos(x) // nilai cosinus (x dalam radian)


    0.540302305868

\>x := cos(x)


    0.857553215846

Jika dua garis dihubungkan dengan "..." Kedua baris akan selalu
dijalankan secara bersamaan.


\>x := 1.5; ...  
\>   x := (x+2/x)/2, x := (x+2/x)/2, x := (x+2/x)/2, 


    1.41666666667
    1.41421568627
    1.41421356237

Ini juga merupakan cara yang baik untuk menyebarkan perintah panjang
ke dua baris atau lebih. Anda dapat menekan Ctrl+Return untuk membagi
baris menjadi dua pada posisi kursor saat ini, atau Ctlr+Back untuk
menggabungkan baris.


Untuk melipat semua multi-baris, tekan Ctrl+L. Kemudian baris
berikutnya hanya akan terlihat, jika salah satunya memiliki fokus.
Untuk melipat satu multi-baris, mulailah baris pertama dengan "%+ ".


\>%+ x=4+5; ...  
\>    // This line will not be visible once the cursor is off the line


Garis yang dimulai dengan %% akan sama sekali tidak terlihat.


    81

Euler mendukung loop dalam baris perintah, selama mereka masuk ke
dalam satu baris tunggal atau multi-baris. Dalam program, pembatasan
ini tidak berlaku, tentu saja. Untuk informasi lebih lanjut,
konsultasikan dengan pengantar berikut.


\>x=1; for i=1 to 5; x := (x+2/x)/2, end; // menghitung akar 2


    1.5
    1.41666666667
    1.41421568627
    1.41421356237
    1.41421356237

Tidak apa-apa untuk menggunakan multi-baris. Pastikan baris diakhiri
dengan " ...".


\>x := 1.5; // comments go here before the ...  
\>   repeat xnew:=(x+2/x)/2; until xnew~=x; ...  
\>      x := xnew; ...  
\>   end; ...  
\>   x,


    1.41421356237

Struktur bersyarat juga berfungsi.


\>if E^pi\>pi^E; then "Thought so!", endif;


    Thought so!

Saat Anda menjalankan perintah, kursor dapat berada di posisi mana pun
di baris perintah. Anda dapat kembali ke perintah sebelumnya atau
melompat ke perintah berikutnya dengan tombol panah. Atau Anda dapat
mengklik bagian komentar di atas perintah untuk membuka perintah.


Saat Anda menggerakkan kursor di sepanjang garis, pasangan tanda
kurung atau tanda kurung pembuka dan penutup akan disorot. Juga,
perhatikan baris status. Setelah tanda kurung pembuka fungsi sqrt(),
baris status akan menampilkan teks bantuan untuk fungsi tersebut.
Jalankan perintah dengan tombol return.


\>sqrt(sin(10°)/cos(20°))


    0.429875017772

Untuk melihat bantuan untuk perintah terbaru, buka jendela bantuan
dengan F1. Di sana, Anda dapat memasukkan teks untuk dicari. Pada
baris kosong, bantuan untuk jendela bantuan akan ditampilkan. Anda
dapat menekan escape untuk menghapus baris, atau untuk menutup jendela
bantuan.


Anda dapat mengklik dua kali pada perintah apa pun untuk membuka
bantuan untuk perintah ini. Coba klik dua kali perintah exp di bawah
ini di baris perintah.


\>exp(log(2.5))


    2.5

Anda juga dapat menyalin dan menempelkan di Euler. Gunakan Ctrl-C dan
Ctrl-V untuk ini. Untuk menandai teks, seret mouse atau gunakan shift
bersama dengan tombol kursor apa pun. Selain itu, Anda dapat menyalin
tanda kurung yang disorot.


## Sintaks Dasar

Euler tahu fungsi matematika yang biasa. Seperti yang telah Anda lihat
di atas, fungsi trigonometri bekerja dalam radian atau derajat. Untuk
mengonversi ke derajat, tambahkan simbol derajat (dengan tombol F7) ke
nilai, atau gunakan fungsi rad(x). Fungsi akar kuadrat disebut sqrt
dalam Euler. Tentu saja, x^(1/2) juga dimungkinkan.


Untuk mengatur variabel, gunakan "=" atau ":=". Demi kejelasan,
pengantar ini menggunakan bentuk yang terakhir. Ruang tidak masalah.
Tetapi ruang di antara perintah diharapkan.


Beberapa perintah dalam satu baris dipisahkan dengan "," atau ";".
Titik koma menekan output perintah. Di akhir baris perintah, ","
diasumsikan, jika ";" hilang.


\>g:=9.81; t:=2.5; 1/2\*g\*t^2


    30.65625

EMT menggunakan sintaks pemrograman untuk ekspresi. Untuk masuk


lateks: e^2 cdot left( frac{1}{3+4 log(0.6)}+frac{1}{7} right)


Anda harus menetapkan tanda kurung yang benar dan menggunakan / untuk
pecahan. Perhatikan tanda kurung yang disorot untuk mendapatkan
bantuan. Perhatikan bahwa konstanta Euler e bernama E di EMT.


\>E^2\*(1/(3+4\*log(0.6))+1/7)


    8.77908249441

Untuk menghitung ekspresi rumit seperti


lateks: left(frac{frac17 + frac18 + 2}{frac13 + frac12}right)^2 pi


Anda harus memasukkannya dalam bentuk baris.


\>((1/7 + 1/8 + 2) / (1/3 + 1/2))^2 \* pi


    23.2671801626

Letakkan tanda kurung dengan hati-hati di sekitar sub-ekspresi yang
perlu dihitung terlebih dahulu. EMT membantu Anda dengan menyoroti
ekspresi yang diselesaikan oleh braket penutup. Anda juga harus
memasukkan nama "pi" untuk huruf Yunani pi.


Hasil perhitungan ini adalah angka floating point. Secara default
dicetak dengan akurasi sekitar 12 digit. Di baris perintah berikut,
kita juga mempelajari bagaimana kita dapat merujuk ke hasil sebelumnya
dalam baris yang sama.


\>1/3+1/7, fraction %


    0.47619047619
    10/21

Perintah Euler dapat berupa ekspresi atau perintah primitif. Ekspresi
dibuat dari operator dan fungsi. Jika perlu, itu harus berisi tanda
kurung untuk memaksa urutan eksekusi yang benar. Jika diragukan,
memasang braket adalah ide yang bagus. Perhatikan bahwa EMT
menunjukkan tanda kurung pembuka dan penutup saat mengedit baris
perintah.


\>(cos(pi/4)+1)^3\*(sin(pi/4)+1)^2


    14.4978445072

Operator numerik Euler meliputi


  + unary atau operator plus  
  - unary atau operator minus  
  *, /  
  . produk matriks  
  a^b daya untuk positif a atau bilangan bulat b (a**b juga berfungsi)  
  n! operator faktorial  

dan masih banyak lagi.


Berikut adalah beberapa fungsi yang mungkin Anda butuhkan. Ada banyak
lagi.


  sin,cos,tan,atan,asin,acos,rad,deg  
  log,exp,log10,sqrt,logbase  
  bin,logbin,logfac,mod,lantai,ceil,bulat,abs,tanda  
  conj,re,im,arg,conj,nyata,kompleks  
  beta,betai,gamma,complexgamma,ellrf,ellf,ellrd,elle  
  bitand, bitor, bitxor, bitnot  

Beberapa perintah memiliki alias, mis. Untuk log.


\>ln(E^2), arctan(tan(0.5))


    2
    0.5

\>sin(30°)


    0.5

Pastikan untuk menggunakan tanda kurung (tanda kurung bundar), setiap
kali ada keraguan tentang urutan eksekusi! Berikut ini tidak sama
dengan (2^3)^4, yang merupakan default untuk 2^3^4 di EMT (beberapa
sistem numerik melakukannya dengan cara lain).


\>2^3^4, (2^3)^4, 2^(3^4)


    2.41785163923e+24
    4096
    2.41785163923e+24

## Bilangan Real (Asli)

Tipe data utama dalam Euler adalah bilangan real. Real
direpresentasikan dalam format IEEE dengan akurasi sekitar 16 digit
desimal.


\>longest 1/3


         0.3333333333333333 

Representasi ganda internal membutuhkan 8 byte.


\>printdual(1/3)


    1.0101010101010101010101010101010101010101010101010101*2^-2

\>printhex(1/3)


    5.5555555555554*16^-1

## String

String dalam Euler didefinisikan dengan "...".


\>"A string can contain anything."


    A string can contain anything.

String dapat digabungkan dengan | atau dengan +. Ini juga berfungsi
dengan angka, yang dikonversi menjadi string dalam kasus ini.


\>"The area of the circle with radius " + 2 + " cm is " + pi\*4 + " cm^2."


    The area of the circle with radius 2 cm is 12.5663706144 cm^2.

Fungsi print juga mengonversi angka menjadi string. Ini dapat
mengambil sejumlah digit dan sejumlah tempat (0 untuk output padat),
dan secara optimal satu unit.


\>"Golden Ratio : " + print((1+sqrt(5))/2,5,0)


    Golden Ratio : 1.61803

Ada string khusus none, yang tidak dicetak. Itu dikembalikan oleh
beberapa fungsi, ketika hasilnya tidak masalah. (Ini dikembalikan
secara otomatis, jika fungsi tidak memiliki pernyataan return.)


\>none


Untuk mengonversi string menjadi angka, cukup evaluasi itu. Ini juga
berfungsi untuk ekspresi (lihat di bawah).


\>"1234.5"()


    1234.5

Untuk mendefinisikan vektor string, gunakan notasi vektor [...]


\>v:=["affe","charlie","bravo"]


    affe
    charlie
    bravo

Vektor string kosong dilambangkan dengan [none]. Vektor string dapat
digabungkan.


\>w:=[none]; w|v|v


    affe
    charlie
    bravo
    affe
    charlie
    bravo

String dapat berisi karakter Unicode. Secara internal, string ini
berisi kode UTF-8. Untuk menghasilkan string seperti itu, gunakan
u"..." dan salah satu entitas HTML.


String Unicode dapat digabungkan seperti string lainnya.


\>u"&alpha; = " + 45 + u"&deg;" // pdfLaTeX mungkin gagal menampilkan secara benar


    α = 45°

I


Dalam komentar, entitas yang sama seperti a, ß dll dapat digunakan.
Ini mungkin alternatif cepat untuk Lateks. (Detail lebih lanjut
tentang komentar di bawah).


Ada beberapa fungsi untuk membuat atau menganalisis string unicode.
Fungsi strtochar() akan mengenali string Unicode, dan menerjemahkannya
dengan benar.


\>v=strtochar(u"&Auml; is a German letter")


    [196,  32,  105,  115,  32,  97,  32,  71,  101,  114,  109,  97,  110,
    32,  108,  101,  116,  116,  101,  114]

Hasilnya adalah vektor angka Unicode. Fungsi kebalikannya adalah
chartoutf().


\>v[1]=strtochar(u"&Uuml;")[1]; chartoutf(v)


    Ü is a German letter

Fungsi utf() dapat menerjemahkan string dengan entitas dalam variabel
ke dalam string Unicode.


\>s="We have &alpha;=&beta;."; utf(s) // pdfLaTeX mungkin gagal menampilkan secara benar


    We have α=β.

Dimungkinkan juga untuk menggunakan entitas numerik.


\>u"&#196;hnliches"


    Ähnliches

## Nilai Boolean

Nilai Boolean direpresentasikan dengan 1=benar atau 0=salah dalam
Euler. String dapat dibandingkan, seperti angka.


\>2<1, "apel"<"banana"


    0
    1

"and" adalah operator "&amp;&amp;" dan "or" adalah operator "||", seperti
dalam bahasa C. (Kata "and" dan "or" hanya dapat digunakan dalam
kondisi untuk "if".)


\>2<E && E<3


    1

Operator Boolean mematuhi aturan bahasa matriks.


\>(1:10)\>5, nonzeros(%)


    [0,  0,  0,  0,  0,  1,  1,  1,  1,  1]
    [6,  7,  8,  9,  10]

Anda dapat menggunakan fungsi nonzeros() untuk mengekstrak elemen
tertentu dari vektor. Dalam contoh, kita menggunakan isprime(n)
bersyarat.


\>N=2|3:2:99 // N berisi elemen 2 dan bilangan2 ganjil dari 3 s.d. 99


    [2,  3,  5,  7,  9,  11,  13,  15,  17,  19,  21,  23,  25,  27,  29,
    31,  33,  35,  37,  39,  41,  43,  45,  47,  49,  51,  53,  55,  57,
    59,  61,  63,  65,  67,  69,  71,  73,  75,  77,  79,  81,  83,  85,
    87,  89,  91,  93,  95,  97,  99]

\>N[nonzeros(isprime(N))] //pilih anggota2 N yang prima


    [2,  3,  5,  7,  11,  13,  17,  19,  23,  29,  31,  37,  41,  43,  47,
    53,  59,  61,  67,  71,  73,  79,  83,  89,  97]

## Format Keluaran

Format keluaran default EMT mencetak 12 digit. Untuk memastikan bahwa
kami melihat default, kami mengatur ulang formatnya.


\>defformat; pi


    3.14159265359

Internally, EMT uses the IEEE standard for double numbers with about
16 decimal digits. To see the full number of digits, use the command
"longestformat", or we use the operator "longest" to display the
result in the longest format.


Secara internal, EMT menggunakan standar IEEE untuk angka ganda dengan
sekitar 16 digit desimal. Untuk melihat jumlah digit penuh, gunakan
perintah "longestformat", atau kami menggunakan operator "longest"
untuk menampilkan hasilnya dalam format longest.


\>longest pi


          3.141592653589793 

Berikut adalah representasi heksadesimal internal dari bilangan ganda.


\>printhex(pi)


    3.243F6A8885A30*16^0

Format keluaran dapat diubah secara permanen dengan perintah format.


\>format(12,5); 1/3, pi, sin(1)


        0.33333 
        3.14159 
        0.84147 

Defaultnya adalah format(12).


\>format(12); 1/3


    0.333333333333

Fungsi seperti "shortestformat", "shortformat", "longformat" bekerja
untuk vektor dengan cara berikut.


\>shortestformat; random(3,8)


      0.66    0.2   0.89   0.28   0.53   0.31   0.44    0.3 
      0.28   0.88   0.27    0.7   0.22   0.45   0.31   0.91 
      0.19   0.46  0.095    0.6   0.43   0.73   0.47   0.32 

Format default untuk skalar adalah format(12). Tapi ini bisa diubah.


\>setscalarformat(5); pi


    3.1416

Fungsi "longestformat" juga mengatur format skalar.


\>longestformat; pi


    3.141592653589793

Sebagai referensi, berikut adalah daftar format keluaran yang paling
penting.


shortestformat shortformat longformat, longestformat


 format(length,digits) goodformat(length)


 fracformat(length)


 defformat


Akurasi internal EMT adalah sekitar 16 tempat desimal, yang merupakan
standar IEEE. Angka disimpan dalam format internal ini.


Tetapi format keluaran EMT dapat diatur dengan cara yang fleksibel.


\>longestformat; pi,


    3.141592653589793

\>format(10,5); pi


      3.14159 

Defaultnya adalah defformat().


\>defformat; // default


Ada operator pendek yang hanya mencetak satu nilai. Operator "longest"
akan mencetak semua digit yang valid dari suatu angka.


\>longest pi^2/2


          4.934802200544679 

Ada juga operator pendek untuk mencetak hasil dalam format pecahan.
Kami telah menggunakannya di atas.


\>fraction 1+1/2+1/3+1/4


    25/12

Karena format internal menggunakan cara biner untuk menyimpan angka,
nilai 0,1 tidak akan direpresentasikan dengan tepat. Kesalahan
bertambah sedikit, seperti yang Anda lihat dalam perhitungan berikut.


\>longest 0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1-1


     -1.110223024625157e-16 

Tetapi dengan "longformat" default Anda tidak akan melihat hal ini.
Untuk kenyamanan, output dari angka yang sangat kecil adalah 0.


\>0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1-1


    0

# Ekspresi

String atau nama dapat digunakan untuk menyimpan ekspresi matematika,
yang dapat dievaluasi oleh EMT. Untuk ini, gunakan tanda kurung
setelah ekspresi. Jika Anda bermaksud menggunakan string sebagai
ekspresi, gunakan konvensi untuk menamakannya "fx" atau "fxy" dll.
Ekspresi lebih diutamakan daripada fungsi.


Variabel global dapat digunakan dalam evaluasi.


\>r:=2; fx:="pi\*r^2"; longest fx()


          12.56637061435917 

Parameter ditetapkan ke x, y, dan z dalam urutan itu. Parameter
tambahan dapat ditambahkan menggunakan parameter yang ditetapkan.


\>fx:="a\*sin(x)^2"; fx(5,a=-1)


    -0.919535764538

Perhatikan bahwa ekspresi akan selalu menggunakan variabel global,
bahkan jika ada variabel dalam fungsi dengan nama yang sama. (Jika
tidak, evaluasi ekspresi dalam fungsi dapat memberikan hasil yang
sangat membingungkan bagi pengguna yang memanggil fungsi tersebut.)


\>at:=4; function f(expr,x,at) := expr(x); ...  
\>   f("at\*x^2",3,5) // computes 4\*3^2 not 5\*3^2


    36

Jika Anda ingin menggunakan nilai lain untuk "at" daripada nilai
global, Anda perlu menambahkan "at=value".


\>at:=4; function f(expr,x,a) := expr(x,at=a); ...  
\>   f("at\*x^2",3,5)


    45

Untuk referensi, kami berkomentar bahwa koleksi panggilan (dibahas di
tempat lain) dapat berisi ekspresi. Jadi kita bisa membuat contoh di
atas sebagai berikut.


\>at:=4; function f(expr,x) := expr(x); ...  
\>   f({{"at\*x^2",at=5}},3)


    45

Ekspresi dalam x sering digunakan seperti fungsi.


Perhatikan bahwa mendefinisikan fungsi dengan nama yang sama seperti
ekspresi simbolik global menghapus variabel ini untuk menghindari
kebingungan antara ekspresi simbolik dan fungsi.


\>f &= 5\*x;

\>function f(x) := 6\*x;

\>f(2)


    12

Dengan cara konvensi, ekspresi simbolik atau numerik harus diberi nama
fx, fxy dll. Skema penamaan ini tidak boleh digunakan untuk fungsi.


\>fx &= diff(x^x,x); $&fx


$$x^{x}\,\left(\log x+1\right)$$Bentuk khusus dari ekspresi memungkinkan variabel apa pun sebagai
parameter tanpa nama untuk evaluasi ekspresi, bukan hanya "x", "y"
dll. Untuk ini, mulai ekspresi dengan "@(variabel) ...".


\>"@(a,b) a^2+b^2", %(4,5)


    @(a,b) a^2+b^2
    41

Ini memungkinkan untuk memanipulasi ekspresi dalam variabel lain untuk
fungsi EMT yang membutuhkan ekspresi dalam "x".


Cara paling dasar untuk mendefinisikan fungsi sederhana adalah dengan
menyimpan rumusnya dalam ekspresi simbolis atau numerik. Jika variabel
utama adalah x, ekspresi dapat dievaluasi seperti fungsi.


Seperti yang Anda lihat dalam contoh berikut, variabel global terlihat
selama evaluasi.


\>fx &= x^3-a\*x;  ...  
\>   a=1.2; fx(0.5)


    -0.475

Semua variabel lain dalam ekspresi dapat ditentukan dalam evaluasi
menggunakan parameter yang ditetapkan.


\>fx(0.5,a=1.1)


    -0.425

Sebuah ekspresi tidak perlu simbolis. Ini diperlukan, jika ekspresi
berisi fungsi, yang hanya diketahui di kernel numerik, bukan di
Maxima.


# Matematika Simbolik

EMT melakukan matematika simbolis dengan bantuan Maxima. Untuk
detailnya, mulailah dengan tutorial berikut, atau telusuri referensi
untuk Maxima. Para ahli di Maxima harus mencatat bahwa ada perbedaan
sintaks antara sintaks asli Maxima dan sintaks default ekspresi
simbolik di EMT.


Matematika simbolik terintegrasi dengan mulus ke dalam Euler dengan &amp;.
Ekspresi apa pun yang dimulai dengan &amp; adalah ekspresi simbolis. Itu
dievaluasi dan dicetak oleh Maxima.


Pertama-tama, Maxima memiliki aritmatika "tak terbatas" yang dapat
menangani angka yang sangat besar.


\>$&44!


$$2658271574788448768043625811014615890319638528000000000$$Dengan cara ini, Anda dapat menghitung hasil yang besar dengan tepat.
Mari kita hitung


lateks: C(44,10) = \frac{44!}{34! \cdot 10!}


\>$& 44!/(34!\*10!) // nilai C(44,10)


$$2481256778$$Tentu saja, Maxima memiliki fungsi yang lebih efisien untuk ini
(seperti halnya bagian numerik dari EMT).


\>$binomial(44,10) //menghitung C(44,10) menggunakan fungsi binomial()


$$2481256778$$Untuk mempelajari lebih lanjut tentang fungsi tertentu klik dua kali
di atasnya. Misalnya, coba klik dua kali pada "&amp;binomial" di baris
perintah sebelumnya. Ini membuka dokumentasi Maxima seperti yang
disediakan oleh penulis program itu.


Anda akan belajar bahwa yang berikut ini juga berfungsi.


$$C(x,3)=\frac{x!}{(x-3)!3!}=\frac{(x-2)(x-1)x}{6}$$\>$binomial(x,3) // C(x,3)


$$\frac{\left(x-2\right)\,\left(x-1\right)\,x}{6}$$Jika Anda ingin mengganti x dengan nilai tertentu, gunakan "with".


\>$&binomial(x,3) with x=10 // substitusi x=10 ke C(x,3)


$$120$$Dengan begitu Anda dapat menggunakan solusi persamaan dalam persamaan
lain.


Ekspresi simbolik dicetak oleh Maxima dalam bentuk 2D. Alasan untuk
ini adalah bendera simbolis khusus dalam string.


Seperti yang akan Anda lihat pada contoh sebelumnya dan berikut, jika
Anda telah menginstal LaTeX, Anda dapat mencetak ekspresi simbolis
dengan Lateks. Jika tidak, perintah berikut akan mengeluarkan pesan
kesalahan.


Untuk mencetak ekspresi simbolis dengan LaTeX, gunakan $ di depan &amp;
(atau Anda dapat menghilangkan &amp;) sebelum perintah. Jangan menjalankan
perintah Maxima dengan $, jika Anda tidak menginstal LaTeX.


\>$(3+x)/(x^2+1)


$$\frac{x+3}{x^2+1}$$Ekspresi simbolik diuraikan oleh Euler. Jika Anda membutuhkan sintaks
yang kompleks dalam satu ekspresi, Anda dapat menyertakan ekspresi
dalam "...". Untuk menggunakan lebih dari ekspresi sederhana adalah
mungkin, tetapi sangat tidak disarankan.


\>&"v := 5; v^2"


    
                                      25
    

Untuk kelengkapan, kami menyatakan bahwa ekspresi simbolik dapat
digunakan dalam program, tetapi perlu diapit dalam tanda kutip. Selain
itu, jauh lebih efektif untuk memanggil Maxima pada waktu kompilasi
jika memungkinkan.


\>$&expand((1+x)^4), $&factor(diff(%,x)) // diff: turunan, factor: faktor


$$x^4+4\,x^3+6\,x^2+4\,x+1$$$$4\,\left(x+1\right)^3$$Sekali lagi, % mengacu pada hasil sebelumnya.


Untuk mempermudah, kami menyimpan solusi ke variabel simbolik.
Variabel simbolik didefinisikan dengan "&amp;=".


\>fx &= (x+1)/(x^4+1); $&fx


$$\frac{x+1}{x^4+1}$$Ekspresi simbolik dapat digunakan dalam ekspresi simbolik lainnya.


\>$&factor(diff(fx,x))


$$\frac{-3\,x^4-4\,x^3+1}{\left(x^4+1\right)^2}$$Masukan langsung dari perintah Maxima juga tersedia. Mulai baris
perintah dengan "::". Sintaks Maxima disesuaikan dengan sintaks EMT
(disebut "mode kompatibilitas").


\>&factor(20!)


    
                             2432902008176640000
    

\>::: factor(10!)


    
                                   8  4  2
                                  2  3  5  7
    

\>:: factor(20!)


    
                            18  8  4  2
                           2   3  5  7  11 13 17 19
    

Jika Anda ahli dalam Maxima, Anda mungkin ingin menggunakan sintaks
asli Maxima. Anda dapat melakukannya dengan ":::".


\>::: av:g$ av^2;


    
                                       2
                                      g
    

\>fx &= x^3\*exp(x), $fx


    
                                     3  x
                                    x  E
    

$$x^3\,e^{x}$$Variabel tersebut dapat digunakan dalam ekspresi simbolik lainnya.
Perhatikan, bahwa dalam perintah berikut sisi kanan &amp;= dievaluasi
sebelum penugasan ke Fx.


\>&(fx with x=5), $%, &float(%)


    
                                         5
                                    125 E
    

$$125\,e^5$$    
                              18551.64488782208
    

\>fx(5)


    18551.6448878

Untuk evaluasi ekspresi dengan nilai variabel tertentu, Anda dapat
menggunakan operator "with".


Baris perintah berikut juga menunjukkan bahwa Maxima dapat
mengevaluasi ekspresi secara numerik dengan float().


\>&(fx with x=10)-(fx with x=5), &float(%)


    
                                    10        5
                              1000 E   - 125 E
    
    
                             2.20079141499189e+7
    

\>$factor(diff(fx,x,2))


$$x\,\left(x^2+6\,x+6\right)\,e^{x}$$Untuk mendapatkan kode Lateks untuk ekspresi, Anda dapat menggunakan
perintah tex.


\>tex(fx)


    x^3\,e^{x}

Ekspresi simbolik dapat dievaluasi seperti ekspresi numerik.


\>fx(0.5)


    0.206090158838

Dalam ekspresi simbolis, ini tidak berfungsi, karena Maxima tidak
mendukungnya. Sebagai gantinya, gunakan sintaks "with" (bentuk yang
lebih bagus dari perintah at(...) dari Maxima).


\>$&fx with x=1/2


$$\frac{\sqrt{e}}{8}$$Penugasan juga bisa bersifat simbolis.


\>$&fx with x=1+t


$$\left(t+1\right)^3\,e^{t+1}$$Perintah solve memecahkan ekspresi simbolik untuk variabel di Maxima.
Hasilnya adalah vektor solusi.


\>$&solve(x^2+x=4,x)


$$\left[ x=\frac{-\sqrt{17}-1}{2} , x=\frac{\sqrt{17}-1}{2} \right] $$Bandingkan dengan perintah numerik "selesaikan" di Euler, yang
membutuhkan nilai awal, dan secara opsional nilai target.


\>solve("x^2+x",1,y=4)


    1.56155281281

Nilai numerik dari solusi simbolik dapat dihitung dengan evaluasi
hasil simbolis. Euler akan membaca tugas x= dll. Jika Anda tidak
memerlukan hasil numerik untuk perhitungan lebih lanjut, Anda juga
dapat membiarkan Maxima menemukan nilai numerik.


\>sol &= solve(x^2+2\*x=4,x); $&sol, sol(), $&float(sol)


$$\left[ x=-\sqrt{5}-1 , x=\sqrt{5}-1 \right] $$    [-3.23607,  1.23607]

$$\left[ x=-3.23606797749979 , x=1.23606797749979 \right] $$Untuk mendapatkan solusi simbolis tertentu, seseorang dapat
menggunakan "with" dan index.


\>$&solve(x^2+x=1,x), x2 &= x with %[2]; $&x2


$$\left[ x=\frac{-\sqrt{5}-1}{2} , x=\frac{\sqrt{5}-1}{2} \right] $$$$\frac{\sqrt{5}-1}{2}$$Untuk menyelesaikan sistem persamaan, gunakan vektor persamaan.
Hasilnya adalah vektor solusi.


\>sol &= solve([x+y=3,x^2+y^2=5],[x,y]); $&sol, $&x\*y with sol[1]


$$\left[ \left[ x=2 , y=1 \right]  , \left[ x=1 , y=2 \right] 
  \right] $$$$2$$Ekspresi simbolis dapat memiliki bendera, yang menunjukkan perlakuan
khusus di Maxima. Beberapa flag dapat digunakan sebagai perintah juga,
yang lain tidak. Bendera ditambahkan dengan "|" (bentuk yang lebih
bagus dari "ev(...,flags)")


\>$& diff((x^3-1)/(x+1),x) //turunan bentuk pecahan


$$\frac{3\,x^2}{x+1}-\frac{x^3-1}{\left(x+1\right)^2}$$\>$& diff((x^3-1)/(x+1),x) | ratsimp //menyederhanakan pecahan


$$\frac{2\,x^3+3\,x^2+1}{x^2+2\,x+1}$$\>$&factor(%)


$$\frac{2\,x^3+3\,x^2+1}{\left(x+1\right)^2}$$# Fungsi

Dalam EMT, fungsi adalah program yang didefinisikan dengan perintah
"function". Ini bisa berupa fungsi satu baris atau fungsi multibaris.


Fungsi satu baris dapat berupa numerik atau simbolis. Fungsi satu
baris numerik didefinisikan oleh ":=".


\>function f(x) := x\*sqrt(x^2+1)


Untuk gambaran umum, kami menunjukkan semua kemungkinan definisi untuk
fungsi satu baris. Suatu fungsi dapat dievaluasi sama seperti fungsi
Euler bawaan lainnya.


\>f(2)


    4.472135955

Fungsi ini akan bekerja untuk vektor juga, dengan mematuhi bahasa
matriks Euler, karena ekspresi yang digunakan dalam fungsi
divektorkan.


\>f(0:0.1:1)


    [0,  0.100499,  0.203961,  0.313209,  0.430813,  0.559017,  0.699714,
    0.854459,  1.0245,  1.21083,  1.41421]

Fungsi dapat diplot. Alih-alih ekspresi, kita hanya perlu memberikan
nama fungsi.


Berbeda dengan ekspresi simbolik atau numerik, nama fungsi harus
diberikan dalam string.


\>solve("f",1,y=1)


    0.786151377757

Secara default, jika Anda perlu menimpa fungsi bawaan, Anda harus
menambahkan kata kunci "menimpa". Menimpa fungsi bawaan berbahaya dan
dapat menyebabkan masalah untuk fungsi lain tergantung pada fungsi
tersebut.


Anda masih dapat memanggil fungsi bawaan sebagai "_...", jika itu
adalah fungsi di inti Euler.


\>function overwrite sin (x) := \_sin(x°) // redine sine in degrees

\>sin(45)


    0.707106781187

Lebih baik kita menghapus redefinisi sin ini.


\>forget sin; sin(pi/4)


    0.707106781187

## Parameter Default

Fungsi numerik dapat memiliki parameter default.


\>function f(x,a=1) := a\*x^2


Menghilangkan parameter ini menggunakan nilai default.


\>f(4)


    16

Menyetelnya akan menimpa nilai default.


\>f(4,5)


    80

Parameter yang ditetapkan menimpanya juga. Ini digunakan oleh banyak
fungsi Euler seperti plot2d, plot3d.


\>f(4,a=1)


    16

Jika suatu variabel bukan parameter, itu harus global. Fungsi satu
baris dapat melihat variabel global.


\>function f(x) := a\*x^2

\>a=6; f(2)


    24

Tetapi parameter yang ditetapkan menimpa nilai global.


Jika argumen tidak ada dalam daftar parameter yang telah ditentukan
sebelumnya, argumen tersebut harus dideklarasikan dengan ":="!


\>f(2,a:=5)


    20

Fungsi simbolis didefinisikan dengan "&amp;=". Mereka didefinisikan dalam
Euler dan Maxima, dan bekerja di kedua dunia. Ekspresi yang
mendefinisikan dijalankan melalui Maxima sebelum definisi.


\>function g(x) &= x^3-x\*exp(-x); $&g(x)


$$x^3-x\,e^ {- x }$$Fungsi simbolik dapat digunakan dalam ekspresi simbolik.


\>$&diff(g(x),x), $&% with x=4/3


$$x\,e^ {- x }-e^ {- x }+3\,x^2$$$$\frac{e^ {- \frac{4}{3} }}{3}+\frac{16}{3}$$Mereka juga dapat digunakan dalam ekspresi numerik. Tentu saja, ini
hanya akan berfungsi jika EMT dapat menginterpretasikan semua yang ada
di dalam fungsi tersebut.


\>g(5+g(1))


    178.635099908

Mereka dapat digunakan untuk mendefinisikan fungsi atau ekspresi
simbolik lainnya.


\>function G(x) &= factor(integrate(g(x),x)); $&G(c) // integrate: mengintegralkan


$$\frac{e^ {- c }\,\left(c^4\,e^{c}+4\,c+4\right)}{4}$$\>solve(&g(x),0.5)


    0.703467422498

Berikut ini juga berfungsi, karena Euler menggunakan ekspresi simbolis
dalam fungsi g, jika tidak menemukan variabel simbolik g, dan jika ada
fungsi simbolis g.


\>solve(&g,0.5)


    0.703467422498

\>function P(x,n) &= (2\*x-1)^n; $&P(x,n)


$$\left(2\,x-1\right)^{n}$$\>function Q(x,n) &= (x+2)^n; $&Q(x,n)


$$\left(x+2\right)^{n}$$\>$&P(x,4), $&expand(%)


$$\left(2\,x-1\right)^4$$$$16\,x^4-32\,x^3+24\,x^2-8\,x+1$$\>P(3,4)


    625

\>$&P(x,4)+ Q(x,3), $&expand(%)


$$\left(2\,x-1\right)^4+\left(x+2\right)^3$$$$16\,x^4-31\,x^3+30\,x^2+4\,x+9$$\>$&P(x,4)-Q(x,3), $&expand(%), $&factor(%)


$$\left(2\,x-1\right)^4-\left(x+2\right)^3$$$$16\,x^4-33\,x^3+18\,x^2-20\,x-7$$$$16\,x^4-33\,x^3+18\,x^2-20\,x-7$$\>$&P(x,4)\*Q(x,3), $&expand(%), $&factor(%)


$$\left(x+2\right)^3\,\left(2\,x-1\right)^4$$$$16\,x^7+64\,x^6+24\,x^5-120\,x^4-15\,x^3+102\,x^2-52\,x+8$$$$\left(x+2\right)^3\,\left(2\,x-1\right)^4$$\>$&P(x,4)/Q(x,1), $&expand(%), $&factor(%)


$$\frac{\left(2\,x-1\right)^4}{x+2}$$$$\frac{16\,x^4}{x+2}-\frac{32\,x^3}{x+2}+\frac{24\,x^2}{x+2}-\frac{8
 \,x}{x+2}+\frac{1}{x+2}$$$$\frac{\left(2\,x-1\right)^4}{x+2}$$\>function f(x) &= x^3-x; $&f(x)


$$x^3-x$$Dengan &amp;= fungsinya simbolis, dan dapat digunakan dalam ekspresi
simbolik lainnya.


\>$&integrate(f(x),x)


$$\frac{x^4}{4}-\frac{x^2}{2}$$Dengan := fungsinya numerik. Contoh yang baik adalah integral tak
tentu seperti


$$f(x) = \int_1^x t^t \, dt,$$yang tidak dapat dinilai secara simbolis.


Jika kita mendefinisikan kembali fungsi dengan kata kunci "peta" dapat
digunakan untuk vektor x. Secara internal, fungsi dipanggil untuk
semua nilai x satu kali, dan hasilnya disimpan dalam vektor.


\>function map f(x) := integrate("x^x",1,x)

\>f(0:0.5:2)


    [-0.783431,  -0.410816,  0,  0.676863,  2.05045]

Fungsi dapat memiliki nilai default untuk parameter.


\>function mylog (x,base=10) := ln(x)/ln(base);


Sekarang fungsi dapat dipanggil dengan atau tanpa parameter "base".


\>mylog(100), mylog(2^6.7,2)


    2
    6.7

Selain itu, dimungkinkan untuk menggunakan parameter yang ditetapkan.


\>mylog(E^2,base=E)


    2

Seringkali, kita ingin menggunakan fungsi untuk vektor di satu tempat,
dan untuk elemen individual di tempat lain. Ini dimungkinkan dengan
parameter vektor.


\>function f([a,b]) &= a^2+b^2-a\*b+b; $&f(a,b), $&f(x,y)


$$b^2-a\,b+b+a^2$$$$y^2-x\,y+y+x^2$$Fungsi simbolik seperti itu dapat digunakan untuk variabel simbolik.


Tetapi fungsinya juga dapat digunakan untuk vektor numerik.


\>v=[3,4]; f(v)


    17

Ada juga fungsi simbolis murni, yang tidak dapat digunakan secara
numerik.


\>function lapl(expr,x,y) &&= diff(expr,x,2)+diff(expr,y,2)//turunan parsial kedua


    
                     diff(expr, y, 2) + diff(expr, x, 2)
    

\>$&realpart((x+I\*y)^4), $&lapl(%,x,y)


$$y^4-6\,x^2\,y^2+x^4$$$$0$$Tetapi tentu saja, mereka dapat digunakan dalam ekspresi simbolik atau
dalam definisi fungsi simbolik.


\>function f(x,y) &= factor(lapl((x+y^2)^5,x,y)); $&f(x,y)


$$10\,\left(y^2+x\right)^3\,\left(9\,y^2+x+2\right)$$Untuk meringkas


* 
&amp;= mendefinisikan fungsi simbolis,

* 
:= mendefinisikan fungsi numerik,

* 
&amp;&amp;= mendefinisikan fungsi simbolis murni.


# Memecahkan Ekspresi

Ekspresi dapat diselesaikan secara numerik dan simbolis.


Untuk menyelesaikan ekspresi sederhana dari satu variabel, kita dapat
menggunakan fungsi solve(). Perlu nilai awal untuk memulai pencarian.
Secara internal, solve() menggunakan metode secant.


\>solve("x^2-2",1)


    1.41421356237

Ini juga berfungsi untuk ekspresi simbolis. Ambil fungsi berikut.


\>$&solve(x^2=2,x)


$$\left[ x=-\sqrt{2} , x=\sqrt{2} \right] $$\>$&solve(x^2-2,x)


$$\left[ x=-\sqrt{2} , x=\sqrt{2} \right] $$\>$&solve(a\*x^2+b\*x+c=0,x)


$$\left[ x=\frac{-\sqrt{b^2-4\,a\,c}-b}{2\,a} , x=\frac{\sqrt{b^2-4\,
 a\,c}-b}{2\,a} \right] $$\>$&solve([a\*x+b\*y=c,d\*x+e\*y=f],[x,y])


$$\left[ \left[ x=-\frac{c\,e}{b\,\left(d-5\right)-a\,e} , y=\frac{c
 \,\left(d-5\right)}{b\,\left(d-5\right)-a\,e} \right]  \right] $$\>px &= 4\*x^8+x^7-x^4-x; $&px


$$4\,x^8+x^7-x^4-x$$Sekarang kita mencari titik, di mana polinomialnya adalah 2. Dalam
solve(), nilai target default y=0 dapat diubah dengan variabel yang
ditetapkan.


Kami menggunakan y=2 dan memeriksa dengan mengevaluasi polinomial pada
hasil sebelumnya.


\>solve(px,1,y=2), px(%)


    0.966715594851
    2

Memecahkan ekspresi simbolis dalam bentuk simbolis mengembalikan
daftar solusi. Kami menggunakan pemecah simbolik solve() yang
disediakan oleh Maxima.


\>sol &= solve(x^2-x-1,x); $&sol


$$\left[ x=\frac{1-\sqrt{5}}{2} , x=\frac{\sqrt{5}+1}{2} \right] $$Cara termudah untuk mendapatkan nilai numerik adalah dengan
mengevaluasi solusi secara numerik seperti ekspresi.


\>longest sol()


        -0.6180339887498949       1.618033988749895 

Untuk menggunakan solusi secara simbolis dalam ekspresi lain, cara
termudah adalah "with".


\>$&x^2 with sol[1], $&expand(x^2-x-1 with sol[2])


$$\frac{\left(\sqrt{5}-1\right)^2}{4}$$$$0$$Memecahkan sistem persamaan secara simbolis dapat dilakukan dengan
vektor persamaan dan solver simbolis solve(). Jawabannya adalah daftar
daftar persamaan.


\>$&solve([x+y=2,x^3+2\*y+x=4],[x,y])


$$\left[ \left[ x=-1 , y=3 \right]  , \left[ x=1 , y=1 \right]  , 
 \left[ x=0 , y=2 \right]  \right] $$Fungsi f() dapat melihat variabel global. Namun seringkali kita ingin
menggunakan parameter lokal.


lateks: a^x-x^a = 0.1


dengan a=3.


\>function f(x,a) := x^a-a^x;


Salah satu cara untuk meneruskan parameter tambahan ke f() adalah
dengan menggunakan daftar dengan nama fungsi dan parameter (sebaliknya
adalah parameter titik koma).


\>solve({{"f",3}},2,y=0.1)


    2.54116291558

Ini juga bekerja dengan ekspresi. Tapi kemudian, elemen daftar bernama
harus digunakan. (Lebih lanjut tentang daftar di tutorial tentang
sintaks EMT).


\>solve({{"x^a-a^x",a=3}},2,y=0.1)


    2.54116291558

# Menyelesaikan Pertidaksamaan

Untuk menyelesaikan pertidaksamaan, EMT tidak akan dapat melakukannya,
melainkan dengan bantuan Maxima, artinya secara eksak (simbolik).
Perintah Maxima yang digunakan adalah fourier_elim(), yang harus
dipanggil dengan perintah "load(fourier_elim)" terlebih dahulu.


\>&load(fourier\_elim)


    
            C:/Program Files/Euler x64/maxima/share/maxima/5.35.1/share/f\
    ourier_elim/fourier_elim.lisp
    

\>$&fourier\_elim([x^2 - 1\>0],[x]) // x^2-1 \> 0


$$\left[ 1<x \right] \lor \left[ x<-1 \right] $$\>$&fourier\_elim([x^2 - 1<0],[x]) // x^2-1 < 0


$$\left[ -1<x , x<1 \right] $$\>$&fourier\_elim([x^2 - 1 # 0],[x]) // x^-1 <\> 0


$$\left[ -1<x , x<1 \right] \lor \left[ 1<x \right] \lor \left[ x<-1
  \right] $$\>$&fourier\_elim([x # 6],[x])


$$\left[ x<6 \right] \lor \left[ 6<x \right] $$\>$&fourier\_elim([x < 1, x \> 1],[x]) // tidak memiliki penyelesaian


$${\it emptyset}$$\>$&fourier\_elim([minf < x, x < inf],[x]) // solusinya R


$${\it universalset}$$\>$&fourier\_elim([x^3 - 1 \> 0],[x])


$$\left[ 1<x , x^2+x+1>0 \right] \lor \left[ x<1 , -x^2-x-1>0
  \right] $$\>$&fourier\_elim([cos(x) < 1/2],[x]) // ??? gagal


$$\left[ 1-2\,\cos x>0 \right] $$\>$&fourier\_elim([y-x < 5, x - y < 7, 10 < y],[x,y]) // sistem pertidaksamaan


$$\left[ y-5<x , x<y+7 , 10<y \right] $$\>$&fourier\_elim([y-x < 5, x - y < 7, 10 < y],[y,x])


$$\left[ {\it max}\left(10 , x-7\right)<y , y<x+5 , 5<x \right] $$\>$&fourier\_elim((x + y < 5) and (x - y \>8),[x,y])


$$\left[ y+8<x , x<5-y , y<-\frac{3}{2} \right] $$\>$&fourier\_elim(((x + y < 5) and x < 1) or  (x - y \>8),[x,y])


$$\left[ y+8<x \right] \lor \left[ x<{\it min}\left(1 , 5-y\right)
  \right] $$\>&fourier\_elim([max(x,y) \> 6, x # 8, abs(y-1) \> 12],[x,y])


    
            [6 &lt; x, x &lt; 8, y &lt; - 11] or [8 &lt; x, y &lt; - 11]
     or [x &lt; 8, 13 &lt; y] or [x = y, 13 &lt; y] or [8 &lt; x, x &lt; y, 13 &lt; y]
     or [y &lt; x, 13 &lt; y]
    

\>$&fourier\_elim([(x+6)/(x-9) <= 6],[x])


$$\left[ x=12 \right] \lor \left[ 12<x \right] \lor \left[ x<9
  \right] $$# Bahasa Matriks

Dokumentasi inti EMT berisi diskusi terperinci tentang bahasa matriks
Euler.


Vektor dan matriks dimasukkan dengan tanda kurung siku, elemen
dipisahkan dengan koma, baris dipisahkan dengan titik koma.


\>A=[1,2;3,4]


                1             2 
                3             4 

Produk matriks dilambangkan dengan titik.


\>b=[3;4]


                3 
                4 

\>b' // transpose b


    [3,  4]

\>inv(A) //inverse A


               -2             1 
              1.5          -0.5 

\>A.b //perkalian matriks


               11 
               25 

\>A.inv(A)


                1             0 
                0             1 

Poin utama dari bahasa matriks adalah bahwa semua fungsi dan operator
bekerja elemen untuk elemen.


\>A.A


                7            10 
               15            22 

\>A^2 //perpangkatan elemen2 A


                1             4 
                9            16 

\>A.A.A


               37            54 
               81           118 

\>power(A,3) //perpangkatan matriks


               37            54 
               81           118 

\>A/A //pembagian elemen-elemen matriks yang seletak


                1             1 
                1             1 

\>A/b //pembagian elemen2 A oleh elemen2 b kolom demi kolom (karena b vektor kolom)


         0.333333      0.666667 
             0.75             1 

\>A\\b // hasilkali invers A dan b, A^(-1)b 


               -2 
              2.5 

\>inv(A).b


               -2 
              2.5 

\>A\\A   //A^(-1)A


                1             0 
                0             1 

\>inv(A).A


                1             0 
                0             1 

\>A\*A //perkalin elemen-elemen matriks seletak


                1             4 
                9            16 

Ini bukan produk matriks, tetapi perkalian elemen demi elemen. Hal
yang sama berlaku untuk vektor.


\>b^2 // perpangkatan elemen-elemen matriks/vektor


                9 
               16 

Jika salah satu operan adalah vektor atau skalar, itu diperluas secara
alami.


\>2\*A


                2             4 
                6             8 

Misalnya, jika operan adalah vektor kolom, elemennya diterapkan ke
semua baris A.


\>[1,2]\*A


                1             4 
                3             8 

Jika itu adalah vektor baris, itu diterapkan ke semua kolom A.


\>A\*[2,3]


                2             6 
                6            12 

Seseorang dapat membayangkan perkalian ini seolah-olah vektor baris v
telah digandakan untuk membentuk matriks dengan ukuran yang sama
dengan A.


\>dup([1,2],2) // dup: menduplikasi/menggandakan vektor [1,2] sebanyak 2 kali (baris)


                1             2 
                1             2 

\>A\*dup([1,2],2) 


                1             4 
                3             8 

Ini juga berlaku untuk dua vektor di mana satu adalah vektor baris dan
yang lainnya adalah vektor kolom. Kami menghitung i*j untuk i,j dari 1
hingga 5. Caranya adalah dengan mengalikan 1:5 dengan transposnya.
Bahasa matriks Euler secara otomatis menghasilkan tabel nilai.


\>(1:5)\*(1:5)' // hasilkali elemen-elemen vektor baris dan vektor kolom


                1             2             3             4             5 
                2             4             6             8            10 
                3             6             9            12            15 
                4             8            12            16            20 
                5            10            15            20            25 

Sekali lagi, ingat bahwa ini bukan produk matriks!


\>(1:5).(1:5)' // hasilkali vektor baris dan vektor kolom


    55

\>sum((1:5)\*(1:5)) // sama hasilnya


    55

Bahkan operator seperti &lt; atau == bekerja dengan cara yang sama.


\>(1:10)<6 // menguji elemen-elemen yang kurang dari 6


    [1,  1,  1,  1,  1,  0,  0,  0,  0,  0]

Misalnya, kita dapat menghitung jumlah elemen yang memenuhi kondisi
tertentu dengan fungsi sum().


\>sum((1:10)<6) // banyak elemen yang kurang dari 6


    5

Euler memiliki operator perbandingan, seperti "==", yang memeriksa
kesetaraan.


Kami mendapatkan vektor 0 dan 1, di mana 1 berarti benar.


\>t=(1:10)^2; t==25 //menguji elemen2 t yang sama dengan 25 (hanya ada 1)


    [0,  0,  0,  0,  1,  0,  0,  0,  0,  0]

Dari vektor seperti itu, "nonzeros" memilih elemen bukan nol.


Dalam hal ini, kami mendapatkan indeks semua elemen lebih besar dari
50.


\>nonzeros(t\>50) //indeks elemen2 t yang lebih besar daripada 50


    [8,  9,  10]

Tentu saja, kita dapat menggunakan vektor indeks ini untuk mendapatkan
nilai yang sesuai dalam t.


\>t[nonzeros(t\>50)] //elemen2 t yang lebih besar daripada 50


    [64,  81,  100]

Sebagai contoh, mari kita cari semua kuadrat dari angka 1 hingga 1000,
yaitu 5 modulo 11 dan 3 modulo 13.


\>t=1:1000; nonzeros(mod(t^2,11)==5 && mod(t^2,13)==3)


    [4,  48,  95,  139,  147,  191,  238,  282,  290,  334,  381,  425,
    433,  477,  524,  568,  576,  620,  667,  711,  719,  763,  810,  854,
    862,  906,  953,  997]

EMT tidak sepenuhnya efektif untuk perhitungan bilangan bulat. Ini
menggunakan titik mengambang presisi ganda secara internal. Namun,
seringkali sangat berguna.


Kita dapat memeriksa keutamaan. Mari kita cari tahu, berapa banyak
kuadrat ditambah 1 adalah bilangan prima.


\>t=1:1000; length(nonzeros(isprime(t^2+1)))


    112

Fungsi bukan nol() hanya berfungsi untuk vektor. Untuk matriks, ada
mnonzeros().


\>seed(2); A=random(3,4)


         0.765761      0.401188      0.406347      0.267829 
          0.13673      0.390567      0.495975      0.952814 
         0.548138      0.006085      0.444255      0.539246 

Ini mengembalikan indeks elemen, yang bukan nol.


\>k=mnonzeros(A<0.4) //indeks elemen2 A yang kurang dari 0,4


                1             4 
                2             1 
                2             2 
                3             2 

Indeks ini dapat digunakan untuk mengatur elemen ke beberapa nilai.


\>mset(A,k,0) //mengganti elemen2 suatu matriks pada indeks tertentu


         0.765761      0.401188      0.406347             0 
                0             0      0.495975      0.952814 
         0.548138             0      0.444255      0.539246 

Fungsi mset() juga dapat mengatur elemen pada indeks ke entri dari
beberapa matriks lainnya.


\>mset(A,k,-random(size(A)))


         0.765761      0.401188      0.406347     -0.126917 
        -0.122404     -0.691673      0.495975      0.952814 
         0.548138     -0.483902      0.444255      0.539246 

Dan dimungkinkan untuk mendapatkan elemen dalam vektor.


\>mget(A,k)


    [0.267829,  0.13673,  0.390567,  0.006085]

Fungsi lain yang berguna adalah ekstrem, yang mengembalikan nilai
minimal dan maksimal di setiap baris matriks dan posisinya.


\>ex=extrema(A)


         0.267829             4      0.765761             1 
          0.13673             1      0.952814             4 
         0.006085             2      0.548138             1 

Kita dapat menggunakan ini untuk mengekstrak nilai maksimal di setiap
baris.


\>ex[,3]'


    [0.765761,  0.952814,  0.548138]

Ini, tentu saja, sama dengan fungsi max().


\>max(A)'


    [0.765761,  0.952814,  0.548138]

Tetapi dengan mget(), kita dapat mengekstrak indeks dan menggunakan
informasi ini untuk mengekstrak elemen pada posisi yang sama dari
matriks lain.


\>j=(1:rows(A))'|ex[,4], mget(-A,j)


                1             1 
                2             4 
                3             1 
    [-0.765761,  -0.952814,  -0.548138]

# Fungsi Matriks Lainnya (Membangun Matriks)

Untuk membangun matriks, kita dapat menumpuk satu matriks di atas yang
lain. Jika keduanya tidak memiliki jumlah kolom yang sama, kolom yang
lebih pendek akan diisi dengan 0.


\>v=1:3; v\_v


                1             2             3 
                1             2             3 

Demikian juga, kita dapat melampirkan matriks ke yang lain secara
berdampingan, jika keduanya memiliki jumlah baris yang sama.


\>A=random(3,4); A|v'


         0.032444     0.0534171      0.595713      0.564454             1 
          0.83916      0.175552      0.396988       0.83514             2 
        0.0257573      0.658585      0.629832      0.770895             3 

Jika mereka tidak memiliki jumlah baris yang sama, matriks yang lebih
pendek diisi dengan 0.


Ada pengecualian untuk aturan ini. Bilangan real yang dilampirkan pada
matriks akan digunakan sebagai kolom yang diisi dengan bilangan real
tersebut.


\>A|1


         0.032444     0.0534171      0.595713      0.564454             1 
          0.83916      0.175552      0.396988       0.83514             1 
        0.0257573      0.658585      0.629832      0.770895             1 

Dimungkinkan untuk membuat matriks vektor baris dan kolom.


\>[v;v]


                1             2             3 
                1             2             3 

\>[v',v']


                1             1 
                2             2 
                3             3 

Tujuan utama dari ini adalah untuk menafsirkan vektor ekspresi untuk
vektor kolom.


\>"[x,x^2]"(v')


                1             1 
                2             4 
                3             9 

Untuk mendapatkan ukuran A, kita dapat menggunakan fungsi berikut.


\>C=zeros(2,4); rows(C), cols(C), size(C), length(C)


    2
    4
    [2,  4]
    4

Untuk vektor, ada panjang().


\>length(2:10)


    9

Ada banyak fungsi lain, yang menghasilkan matriks.


\>ones(2,2)


                1             1 
                1             1 

Ini juga dapat digunakan dengan satu parameter. Untuk mendapatkan
vektor dengan angka selain 1, gunakan yang berikut ini.


\>ones(5)\*6


    [6,  6,  6,  6,  6]

Juga matriks bilangan acak dapat dihasilkan dengan acak (uniform
distribution) atau normal (Gauß distribution).


\>random(2,2)


          0.66566      0.831835 
            0.977      0.544258 

Berikut adalah fungsi lain yang berguna, yang merestrukturisasi elemen
matriks menjadi matriks lain.


\>redim(1:9,3,3) // menyusun elemen2 1, 2, 3, ..., 9 ke bentuk matriks 3x3


                1             2             3 
                4             5             6 
                7             8             9 

Dengan fungsi berikut, kita dapat menggunakan ini dan fungsi dup untuk
menulis fungsi rep(), yang mengulang vektor n kali.


\>function rep(v,n) := redim(dup(v,n),1,n\*cols(v))


Mari kita uji.


\>rep(1:3,5)


    [1,  2,  3,  1,  2,  3,  1,  2,  3,  1,  2,  3,  1,  2,  3]

Fungsi multdup() menduplikasi elemen vektor.


\>multdup(1:3,5), multdup(1:3,[2,3,2])


    [1,  1,  1,  1,  1,  2,  2,  2,  2,  2,  3,  3,  3,  3,  3]
    [1,  1,  2,  2,  2,  3,  3]

Fungsi flipx() dan flipy() mengembalikan urutan baris atau kolom
matriks. Yaitu, fungsi flipx() membalik secara horizontal.


\>flipx(1:5) //membalik elemen2 vektor baris


    [5,  4,  3,  2,  1]

Untuk rotasi, Euler memiliki rotleft() dan rotright().


\>rotleft(1:5) // memutar elemen2 vektor baris


    [2,  3,  4,  5,  1]

Sebuah fungsi khusus adalah drop(v,i), yang menghilangkan elemen
dengan indeks di i dari vektor v.


\>drop(10:20,3)


    [10,  11,  13,  14,  15,  16,  17,  18,  19,  20]

Perhatikan bahwa vektor i di drop(v,i) mengacu pada indeks elemen di
v, bukan nilai elemen. Jika Anda ingin menghapus elemen, Anda harus
menemukan elemennya terlebih dahulu. Fungsi indexof(v,x) dapat
digunakan untuk mencari elemen x dalam vektor terurut v.


\>v=primes(50), i=indexof(v,10:20), drop(v,i)


    [2,  3,  5,  7,  11,  13,  17,  19,  23,  29,  31,  37,  41,  43,  47]
    [0,  5,  0,  6,  0,  0,  0,  7,  0,  8,  0]
    [2,  3,  5,  7,  23,  29,  31,  37,  41,  43,  47]

Seperti yang Anda lihat, tidak ada salahnya untuk memasukkan indeks di
luar rentang (seperti 0), indeks ganda, atau indeks yang tidak
diurutkan.


\>drop(1:10,shuffle([0,0,5,5,7,12,12]))


    [1,  2,  3,  4,  6,  8,  9,  10]

Ada beberapa fungsi khusus untuk mengatur diagonal atau untuk
menghasilkan matriks diagonal.


Kita mulai dengan matriks identitas.


\>A=id(5) // matriks identitas 5x5


                1             0             0             0             0 
                0             1             0             0             0 
                0             0             1             0             0 
                0             0             0             1             0 
                0             0             0             0             1 

Kemudian kita atur diagonal bawah (-1) menjadi 1:4.


\>setdiag(A,-1,1:4) //mengganti diagonal di bawah diagonal utama


                1             0             0             0             0 
                1             1             0             0             0 
                0             2             1             0             0 
                0             0             3             1             0 
                0             0             0             4             1 

Perhatikan bahwa kami tidak mengubah matriks A. Kami mendapatkan
matriks baru sebagai hasil dari setdiag().


Berikut adalah fungsi, yang mengembalikan matriks tri-diagonal.


\>function tridiag (n,a,b,c) := setdiag(setdiag(b\*id(n),1,c),-1,a); ...  
\>   tridiag(5,1,2,3)


                2             3             0             0             0 
                1             2             3             0             0 
                0             1             2             3             0 
                0             0             1             2             3 
                0             0             0             1             2 

Diagonal suatu matriks juga dapat diekstraksi dari matriks tersebut.
Untuk mendemonstrasikan ini, kami merestrukturisasi vektor 1:9 menjadi
matriks 3x3.


\>A=redim(1:9,3,3)


                1             2             3 
                4             5             6 
                7             8             9 

Sekarang kita dapat mengekstrak diagonal.


\>d=getdiag(A,0)


    [1,  5,  9]

Misalnya. Kita dapat membagi matriks dengan diagonalnya. Bahasa
matriks memperhatikan bahwa vektor kolom d diterapkan ke matriks baris
demi baris.


\>fraction A/d'


            1         2         3 
          4/5         1       6/5 
          7/9       8/9         1 

# Vektorisasi

Hampir semua fungsi di Euler juga berfungsi untuk input matriks dan
vektor, kapan pun ini masuk akal.


Misalnya, fungsi sqrt() menghitung akar kuadrat dari semua elemen
vektor atau matriks.


\>sqrt(1:3)


    [1,  1.41421,  1.73205]

Jadi Anda dapat dengan mudah membuat tabel nilai. Ini adalah salah
satu cara untuk memplot suatu fungsi (alternatifnya menggunakan
ekspresi).


\>x=1:0.01:5; y=log(x)/x^2; // terlalu panjang untuk ditampikan


Dengan ini dan operator titik dua a:delta:b, vektor nilai fungsi dapat
dihasilkan dengan mudah.


Pada contoh berikut, kita membangkitkan vektor nilai t[i] dengan spasi
0,1 dari -1 hingga 1. Kemudian kita membangkitkan vektor nilai fungsi


lateks: s = t^3-t


\>t=-1:0.1:1; s=t^3-t


    [0,  0.171,  0.288,  0.357,  0.384,  0.375,  0.336,  0.273,  0.192,
    0.099,  0,  -0.099,  -0.192,  -0.273,  -0.336,  -0.375,  -0.384,
    -0.357,  -0.288,  -0.171,  0]

EMT memperluas operator untuk skalar, vektor, dan matriks dengan cara
yang jelas.


Misalnya, vektor kolom dikalikan vektor baris menjadi matriks, jika
operator diterapkan. Berikut ini, v' adalah vektor yang
ditransposisikan (vektor kolom).


\>shortest (1:5)\*(1:5)'


         1      2      3      4      5 
         2      4      6      8     10 
         3      6      9     12     15 
         4      8     12     16     20 
         5     10     15     20     25 

Perhatikan, bahwa ini sangat berbeda dari produk matriks. Produk
matriks dilambangkan dengan titik "." di EMT.


\>(1:5).(1:5)'


    55

Secara default, vektor baris dicetak dalam format yang ringkas.


\>[1,2,3,4]


    [1,  2,  3,  4]

Untuk matriks operator khusus . menunjukkan perkalian matriks, dan A'
menunjukkan transpos. Matriks 1x1 dapat digunakan seperti bilangan
real.


\>v:=[1,2]; v.v', %^2


    5
    25

Untuk mentranspos matriks kita menggunakan apostrof.


\>v=1:4; v'


                1 
                2 
                3 
                4 

Jadi kita dapat menghitung matriks A kali vektor b.


\>A=[1,2,3,4;5,6,7,8]; A.v'


               30 
               70 

Perhatikan bahwa v masih merupakan vektor baris. Jadi v'.v berbeda
dari v.v'.


\>v'.v


                1             2             3             4 
                2             4             6             8 
                3             6             9            12 
                4             8            12            16 

v.v' menghitung norma v kuadrat untuk vektor baris v. Hasilnya adalah
vektor 1x1, yang bekerja seperti bilangan real.


\>v.v'


    30

Ada juga fungsi norma (bersama dengan banyak fungsi lain dari Aljabar
Linier).


\>norm(v)^2


    30

Operator dan fungsi mematuhi bahasa matriks Euler.


Berikut ringkasan aturannya.


* 
Fungsi yang diterapkan ke vektor atau matriks diterapkan ke setiap
* elemen.


* 
Operator yang beroperasi pada dua matriks dengan ukuran yang sama
* diterapkan berpasangan ke elemen matriks.


* 
Jika kedua matriks memiliki dimensi yang berbeda, keduanya diperluas
* dengan cara yang masuk akal, sehingga memiliki ukuran yang sama.


Misalnya, nilai skalar kali vektor mengalikan nilai dengan setiap
elemen vektor. Atau matriks kali vektor (dengan *, bukan .) memperluas
vektor ke ukuran matriks dengan menduplikasinya.


Berikut ini adalah kasus sederhana dengan operator ^.


\>[1,2,3]^2


    [1,  4,  9]

Berikut adalah kasus yang lebih rumit. Vektor baris dikalikan dengan
vektor kolom mengembang keduanya dengan menduplikasi.


\>v:=[1,2,3]; v\*v'


                1             2             3 
                2             4             6 
                3             6             9 

Perhatikan bahwa produk skalar menggunakan produk matriks, bukan *!


\>v.v'


    14

Ada banyak fungsi matriks. Kami memberikan daftar singkat. Anda harus
berkonsultasi dengan dokumentasi untuk informasi lebih lanjut tentang
perintah ini.


   sum,prod menghitung jumlah dan produk dari baris  
   cumsum,cumprod melakukan hal yang sama secara kumulatif  
   menghitung nilai ekstrem dari setiap baris  
   extrema mengembalikan vektor dengan informasi ekstrim  
   diag(A,i) mengembalikan diagonal ke-i  
   setdiag(A,i,v) mengatur diagonal ke-i  
   id(n) matriks identitas  
   det(A) penentu  
   charpoly(A) polinomial karakteristik  
   nilai eigen(A) nilai eigen  

\>v\*v, sum(v\*v), cumsum(v\*v)


    [1,  4,  9]
    14
    [1,  5,  14]

Operator : menghasilkan vektor baris spasi yang sama, opsional dengan
ukuran langkah.


\>1:4, 1:2:10


    [1,  2,  3,  4]
    [1,  3,  5,  7,  9]

Untuk menggabungkan matriks dan vektor ada operator "|" dan "_".


\>[1,2,3]|[4,5], [1,2,3]\_1


    [1,  2,  3,  4,  5]
                1             2             3 
                1             1             1 

Unsur-unsur matriks disebut dengan "A[i,j]".


\>A:=[1,2,3;4,5,6;7,8,9]; A[2,3]


    6

Untuk vektor baris atau kolom, v[i] adalah elemen ke-i dari vektor.
Untuk matriks, ini mengembalikan baris ke-i lengkap dari matriks.


\>v:=[2,4,6,8]; v[3], A[3]


    6
    [7,  8,  9]

Indeks juga bisa menjadi vektor baris dari indeks. : menunjukkan semua
indeks.


\>v[1:2], A[:,2]


    [2,  4]
                2 
                5 
                8 

Bentuk singkat untuk : adalah menghilangkan indeks sepenuhnya.


\>A[,2:3]


                2             3 
                5             6 
                8             9 

Untuk tujuan vektorisasi, elemen matriks dapat diakses seolah-olah
mereka adalah vektor.


\>A{4}


    4

Matriks juga dapat diratakan, menggunakan fungsi redim(). Ini
diimplementasikan dalam fungsi flatten().


\>redim(A,1,prod(size(A))), flatten(A)


    [1,  2,  3,  4,  5,  6,  7,  8,  9]
    [1,  2,  3,  4,  5,  6,  7,  8,  9]

Untuk menggunakan matriks untuk tabel, mari kita reset ke format
default, dan menghitung tabel nilai sinus dan kosinus. Perhatikan
bahwa sudut dalam radian secara default.


\>defformat; w=0°:45°:360°; w=w'; deg(w)


                0 
               45 
               90 
              135 
              180 
              225 
              270 
              315 
              360 

Sekarang kita menambahkan kolom ke matriks.


\>M = deg(w)|w|cos(w)|sin(w)


                0             0             1             0 
               45      0.785398      0.707107      0.707107 
               90        1.5708             0             1 
              135       2.35619     -0.707107      0.707107 
              180       3.14159            -1             0 
              225       3.92699     -0.707107     -0.707107 
              270       4.71239             0            -1 
              315       5.49779      0.707107     -0.707107 
              360       6.28319             1             0 

Dengan menggunakan bahasa matriks, kita dapat menghasilkan beberapa
tabel dari beberapa fungsi sekaligus.


Dalam contoh berikut, kita menghitung t[j]^i untuk i dari 1 hingga n.
Kami mendapatkan matriks, di mana setiap baris adalah tabel t^i untuk
satu i. Yaitu, matriks memiliki elemen lateks: a_{i,j} = t_j^i, \quad
1 \le j \le 101, \quad 1 \le i \le n


Fungsi yang tidak berfungsi untuk input vektor harus "divektorkan".
Ini dapat dicapai dengan kata kunci "peta" dalam definisi fungsi.
Kemudian fungsi tersebut akan dievaluasi untuk setiap elemen dari
parameter vektor.


Integrasi numerik terintegrasi() hanya berfungsi untuk batas interval
skalar. Jadi kita perlu membuat vektor.


\>function map f(x) := integrate("x^x",1,x)


Kata kunci "peta" membuat vektor fungsi. Fungsinya sekarang akan
bekerja


untuk vektor bilangan.


\>f([1:5])


    [0,  2.05045,  13.7251,  113.336,  1241.03]

# Sub-Matriks dan Matriks-Elemen

Untuk mengakses elemen matriks, gunakan notasi braket.


\>A=[1,2,3;4,5,6;7,8,9], A[2,2]


                1             2             3 
                4             5             6 
                7             8             9 
    5

Kita dapat mengakses satu baris matriks yang lengkap.


\>A[2]


    [4,  5,  6]

Dalam kasus vektor baris atau kolom, ini mengembalikan elemen vektor.


\>v=1:3; v[2]


    2

Untuk memastikan, Anda mendapatkan baris pertama untuk matriks 1xn dan
mxn, tentukan semua kolom menggunakan indeks kedua kosong.


\>A[2,]


    [4,  5,  6]

Jika indeks adalah vektor indeks, Euler akan mengembalikan baris
matriks yang sesuai.


Di sini kita ingin baris pertama dan kedua dari A.


\>A[[1,2]]


                1             2             3 
                4             5             6 

Kita bahkan dapat menyusun ulang A menggunakan vektor indeks.
Tepatnya, kami tidak mengubah A di sini, tetapi menghitung versi A
yang disusun ulang.


\>A[[3,2,1]]


                7             8             9 
                4             5             6 
                1             2             3 

Trik indeks bekerja dengan kolom juga.


Contoh ini memilih semua baris A dan kolom kedua dan ketiga.


\>A[1:3,2:3]


                2             3 
                5             6 
                8             9 

Untuk singkatan ":" menunjukkan semua indeks baris atau kolom.


\>A[:,3]


                3 
                6 
                9 

Atau, biarkan indeks pertama kosong.


\>A[,2:3]


                2             3 
                5             6 
                8             9 

Kita juga bisa mendapatkan baris terakhir dari A.


\>A[-1]


    [7,  8,  9]

Sekarang mari kita ubah elemen A dengan menetapkan submatriks A ke
beberapa nilai. Ini sebenarnya mengubah matriks A yang disimpan.


\>A[1,1]=4


                4             2             3 
                4             5             6 
                7             8             9 

Kami juga dapat menetapkan nilai ke baris A.


\>A[1]=[-1,-1,-1]


               -1            -1            -1 
                4             5             6 
                7             8             9 

Kami bahkan dapat menetapkan sub-matriks jika memiliki ukuran yang
tepat.


\>A[1:2,1:2]=[5,6;7,8]


                5             6            -1 
                7             8             6 
                7             8             9 

Selain itu, beberapa jalan pintas diperbolehkan.


\>A[1:2,1:2]=0


                0             0            -1 
                0             0             6 
                7             8             9 

Peringatan: Indeks di luar batas mengembalikan matriks kosong, atau
pesan kesalahan, tergantung pada pengaturan sistem. Standarnya adalah
pesan kesalahan. Ingat, bagaimanapun, bahwa indeks negatif dapat
digunakan untuk mengakses elemen matriks yang dihitung dari akhir.


\>A[4]


    Row index 4 out of bounds!
    Error in:
    A[4] ...
        ^

# Menyortir dan Mengacak

Fungsi sort() mengurutkan vektor baris.


\>sort([5,6,4,8,1,9])


    [1,  4,  5,  6,  8,  9]

Seringkali perlu untuk mengetahui indeks dari vektor yang diurutkan
dalam vektor aslinya. Ini dapat digunakan untuk menyusun ulang vektor
lain dengan cara yang sama.


Mari kita mengocok vektor.


\>v=shuffle(1:10)


    [4,  5,  10,  6,  8,  9,  1,  7,  2,  3]

Indeks berisi urutan yang tepat dari v.


\>{vs,ind}=sort(v); v[ind]


    [1,  2,  3,  4,  5,  6,  7,  8,  9,  10]

Ini bekerja untuk vektor string juga.


\>s=["a","d","e","a","aa","e"]


    a
    d
    e
    a
    aa
    e

\>{ss,ind}=sort(s); ss


    a
    a
    aa
    d
    e
    e

Seperti yang Anda lihat, posisi entri ganda agak acak.


\>ind


    [4,  1,  5,  2,  6,  3]

Fungsi unik mengembalikan daftar elemen unik vektor yang diurutkan.


\>intrandom(1,10,10), unique(%)


    [4,  4,  9,  2,  6,  5,  10,  6,  5,  1]
    [1,  2,  4,  5,  6,  9,  10]

Ini bekerja untuk vektor string juga.


\>unique(s)


    a
    aa
    d
    e

# Aljabar linier

EMT memiliki banyak fungsi untuk menyelesaikan sistem linier, sistem
sparse, atau masalah regresi.


Untuk sistem linier Ax=b, Anda dapat menggunakan algoritma Gauss,
matriks invers atau kecocokan linier. Operator A\b menggunakan versi
algoritma Gauss.


\>A=[1,2;3,4]; b=[5;6]; A\\b


               -4 
              4.5 

Untuk contoh lain, kami membuat matriks 200x200 dan jumlah barisnya.
Kemudian kita selesaikan Ax=b menggunakan matriks invers. Kami
mengukur kesalahan sebagai deviasi maksimal semua elemen dari 1, yang
tentu saja merupakan solusi yang benar.


\>A=normal(200,200); b=sum(A); longest totalmax(abs(inv(A).b-1))


      8.790745908981989e-13 

Jika sistem tidak memiliki solusi, kecocokan linier meminimalkan norma
kesalahan Ax-b.


\>A=[1,2,3;4,5,6;7,8,9]


                1             2             3 
                4             5             6 
                7             8             9 

Determinan matriks ini adalah 0.


\>det(A)


    0

# Matriks Simbolik

Maxima memiliki matriks simbolis. Tentu saja, Maxima dapat digunakan
untuk masalah aljabar linier sederhana seperti itu. Kita dapat
mendefinisikan matriks untuk Euler dan Maxima dengan &amp;:=, dan kemudian
menggunakannya dalam ekspresi simbolis. Bentuk [...] biasa untuk
mendefinisikan matriks dapat digunakan di Euler untuk mendefinisikan
matriks simbolik.


\>A &= [a,1,1;1,a,1;1,1,a]; $A


$$\begin{pmatrix}a & 1 & 1 \\ 1 & a & 1 \\ 1 & 1 & a \\ \end{pmatrix}$$\>$&det(A), $&factor(%)


$$a\,\left(a^2-1\right)-2\,a+2$$$$\left(a-1\right)^2\,\left(a+2\right)$$\>$&invert(A) with a=0


$$\begin{pmatrix}-\frac{1}{2} & \frac{1}{2} & \frac{1}{2} \\ \frac{1
 }{2} & -\frac{1}{2} & \frac{1}{2} \\ \frac{1}{2} & \frac{1}{2} & -
 \frac{1}{2} \\ \end{pmatrix}$$\>A &= [1,a;b,2]; $A


$$\begin{pmatrix}1 & a \\ b & 2 \\ \end{pmatrix}$$Seperti semua variabel simbolik, matriks ini dapat digunakan dalam
ekspresi simbolik lainnya.


\>$&det(A-x\*ident(2)), $&solve(%,x)


$$\left(1-x\right)\,\left(2-x\right)-a\,b$$$$\left[ x=\frac{3-\sqrt{4\,a\,b+1}}{2} , x=\frac{\sqrt{4\,a\,b+1}+3
 }{2} \right] $$Nilai eigen juga dapat dihitung secara otomatis. Hasilnya adalah
vektor dengan dua vektor nilai eigen dan multiplisitas.


\>$&eigenvalues([a,1;1,a])


$$\left[ \left[ a-1 , a+1 \right]  , \left[ 1 , 1 \right]  \right] $$Untuk mengekstrak vektor eigen tertentu perlu pengindeksan yang
cermat.


\>$&eigenvectors([a,1;1,a]), &%[2][1][1]


$$\left[ \left[ \left[ a-1 , a+1 \right]  , \left[ 1 , 1 \right] 
  \right]  , \left[ \left[ \left[ 1 , -1 \right]  \right]  , \left[ 
 \left[ 1 , 1 \right]  \right]  \right]  \right] $$    
                                   [1, - 1]
    

Matriks simbolik dapat dievaluasi dalam Euler secara numerik seperti
ekspresi simbolik lainnya.


\>A(a=4,b=5)


                1             4 
                5             2 

Dalam ekspresi simbolik, gunakan dengan.


\>$&A with [a=4,b=5]


$$\begin{pmatrix}1 & 4 \\ 5 & 2 \\ \end{pmatrix}$$Akses ke baris matriks simbolik bekerja seperti halnya dengan matriks
numerik.


\>$&A[1]


$$\left[ 1 , a \right] $$A symbolic expression can contain an assignment. And that changes the
matrix A.


\>&A[1,1]:=t+1; $&A


$$\begin{pmatrix}t+1 & a \\ b & 2 \\ \end{pmatrix}$$Ada fungsi simbolik di Maxima untuk membuat vektor dan matriks. Untuk
ini, lihat dokumentasi Maxima atau tutorial tentang Maxima di EMT.


\>v &= makelist(1/(i+j),i,1,3); $v


$$\left[ \frac{1}{j+1} , \frac{1}{j+2} , \frac{1}{j+3} \right] $$\>B &:= [1,2;3,4]; $B, $&invert(B)


$$\begin{pmatrix}1 & 2 \\ 3 & 4 \\ \end{pmatrix}$$$$\begin{pmatrix}-2 & 1 \\ \frac{3}{2} & -\frac{1}{2} \\ 
 \end{pmatrix}$$Hasilnya dapat dievaluasi secara numerik dalam Euler. Untuk informasi
lebih lanjut tentang Maxima, lihat pengantar Maxima.


\>$&invert(B)()


               -2             1 
              1.5          -0.5 

Euler juga memiliki fungsi xinv() yang kuat, yang membuat upaya lebih
besar dan mendapatkan hasil yang lebih tepat.


Perhatikan, bahwa dengan &amp;:= matriks B telah didefinisikan sebagai
simbolik dalam ekspresi simbolik dan sebagai numerik dalam ekspresi
numerik. Jadi kita bisa menggunakannya di sini.


\>longest B.xinv(B)


                          1                       0 
                          0                       1 

Misalnya. nilai eigen dari A dapat dihitung secara numerik.


\>A=[1,2,3;4,5,6;7,8,9]; real(eigenvalues(A))


    [16.1168,  -1.11684,  0]

Atau secara simbolis. Lihat tutorial tentang Maxima untuk detailnya.


\>$&eigenvalues(@A)


$$\left[ \left[ \frac{15-3\,\sqrt{33}}{2} , \frac{3\,\sqrt{33}+15}{2}
  , 0 \right]  , \left[ 1 , 1 , 1 \right]  \right] $$# Nilai Numerik dalam Ekspresi simbolis

Ekspresi simbolis hanyalah string yang berisi ekspresi. Jika kita
ingin mendefinisikan nilai baik untuk ekspresi simbolik maupun
ekspresi numerik, kita harus menggunakan "&amp;:=".


\>A &:= [1,pi;4,5]


                1       3.14159 
                4             5 

Masih ada perbedaan antara bentuk numerik dan simbolik. Saat
mentransfer matriks ke bentuk simbolis, pendekatan fraksional untuk
real akan digunakan.


\>$&A


$$\begin{pmatrix}1 & \frac{1146408}{364913} \\ 4 & 5 \\ \end{pmatrix}$$Untuk menghindarinya, ada fungsi "mxmset(variable)".


\>mxmset(A); $&A


$$\begin{pmatrix}1 & 3.141592653589793 \\ 4 & 5 \\ \end{pmatrix}$$Maxima juga dapat menghitung dengan angka floating point, dan bahkan
dengan angka floating besar dengan 32 digit. Namun, evaluasinya jauh
lebih lambat.


\>$&bfloat(sqrt(2)), $&float(sqrt(2))


$$1.4142135623730950488016887242097_B \times 10^{0}$$$$1.414213562373095$$Ketepatan angka floating point besar dapat diubah.


\>&fpprec:=100; &bfloat(pi)


    
            3.14159265358979323846264338327950288419716939937510582097494\
    4592307816406286208998628034825342117068b0
    

Variabel numerik dapat digunakan dalam ekspresi simbolis apa pun
menggunakan "@var".


Perhatikan bahwa ini hanya diperlukan, jika variabel telah
didefinisikan dengan ":=" atau "=" sebagai variabel numerik.


\>B:=[1,pi;3,4]; $&det(@B)


$$-5.424777960769379$$# Demo - Suku Bunga

Di bawah ini, kami menggunakan Euler Math Toolbox (EMT) untuk
perhitungan suku bunga. Kami melakukannya secara numerik dan simbolis
untuk menunjukkan kepada Anda bagaimana Euler dapat digunakan untuk
memecahkan masalah kehidupan nyata.


Asumsikan Anda memiliki modal awal 5000 (katakanlah dalam dolar).


\>K=5000


    5000

Sekarang kita asumsikan tingkat bunga 3% per tahun. Mari kita
tambahkan satu tarif sederhana dan hitung hasilnya.


\>K\*1.03


    5150

Euler akan memahami sintaks berikut juga.


\>K+K\*3%


    5150

Tetapi lebih mudah menggunakan faktornya


\>q=1+3%, K\*q


    1.03
    5150

Selama 10 tahun, kita cukup mengalikan faktornya dan mendapatkan nilai
akhir dengan suku bunga majemuk.


\>K\*q^10


    6719.58189672

Untuk tujuan kita, kita dapat mengatur format menjadi 2 digit setelah
titik desimal.


\>format(12,2); K\*q^10


        6719.58 

Mari kita cetak yang dibulatkan menjadi 2 digit dalam kalimat lengkap.


\>"Starting from " + K + "$ you get " + round(K\*q^10,2) + "$."


    Starting from 5000$ you get 6719.58$.

Bagaimana jika kita ingin mengetahui hasil antara dari tahun 1 sampai
tahun 9? Untuk ini, bahasa matriks Euler sangat membantu. Anda tidak
harus menulis loop, tetapi cukup masukkan


\>K\*q^(0:10)


    Real 1 x 11 matrix
    
        5000.00     5150.00     5304.50     5463.64     ...

Bagaimana keajaiban ini bekerja? Pertama ekspresi 0:10 mengembalikan
vektor bilangan bulat.


\>short 0:10


    [0,  1,  2,  3,  4,  5,  6,  7,  8,  9,  10]

Kemudian semua operator dan fungsi dalam Euler dapat diterapkan pada
elemen vektor untuk elemen. Jadi


\>short q^(0:10)


    [1,  1.03,  1.0609,  1.0927,  1.1255,  1.1593,  1.1941,  1.2299,
    1.2668,  1.3048,  1.3439]

adalah vektor faktor q^0 sampai q^10. Ini dikalikan dengan K, dan kami
mendapatkan vektor nilai.


\>VK=K\*q^(0:10);


Tentu saja, cara realistis untuk menghitung suku bunga ini adalah
dengan membulatkan ke sen terdekat setelah setiap tahun. Mari kita
tambahkan fungsi untuk ini.


\>function oneyear (K) := round(K\*q,2)


Mari kita bandingkan dua hasil, dengan dan tanpa pembulatan.


\>longest oneyear(1234.57), longest 1234.57\*q


                    1271.61 
                  1271.6071 

Sekarang tidak ada rumus sederhana untuk tahun ke-n, dan kita harus
mengulang selama bertahun-tahun. Euler memberikan banyak solusi untuk
ini.


Cara termudah adalah iterasi fungsi, yang mengulangi fungsi tertentu
beberapa kali.


\>VKr=iterate("oneyear",5000,10)


    Real 1 x 11 matrix
    
        5000.00     5150.00     5304.50     5463.64     ...

Kami dapat mencetaknya dengan cara yang ramah, menggunakan format kami
dengan tempat desimal tetap.


\>VKr'


        5000.00 
        5150.00 
        5304.50 
        5463.64 
        5627.55 
        5796.38 
        5970.27 
        6149.38 
        6333.86 
        6523.88 
        6719.60 

Untuk mendapatkan elemen tertentu dari vektor, kami menggunakan indeks
dalam tanda kurung siku.


\>VKr[2], VKr[1:3]


        5150.00 
        5000.00     5150.00     5304.50 

Anehnya, kita juga bisa menggunakan vektor indeks. Ingat bahwa 1:3
menghasilkan vektor [1,2,3].


Mari kita bandingkan elemen terakhir dari nilai yang dibulatkan dengan
nilai penuh.


\>VKr[-1], VK[-1]


        6719.60 
        6719.58 

Perbedaannya sangat kecil.


# Memecahkan Persamaan

Sekarang kita mengambil fungsi yang lebih maju, yang menambahkan
tingkat uang tertentu setiap tahun.


\>function onepay (K) := K\*q+R


Kita tidak perlu menentukan q atau R untuk definisi fungsi. Hanya jika
kita menjalankan perintah, kita harus mendefinisikan nilai-nilai ini.
Kami memilih R=200.


\>R=200; iterate("onepay",5000,10)


    Real 1 x 11 matrix
    
        5000.00     5350.00     5710.50     6081.82     ...

Bagaimana jika kita menghapus jumlah yang sama setiap tahun?


\>R=-200; iterate("onepay",5000,10)


    Real 1 x 11 matrix
    
        5000.00     4950.00     4898.50     4845.45     ...

Kami melihat bahwa uang berkurang. Jelas, jika kita hanya mendapatkan
150 bunga di tahun pertama, tetapi menghapus 200, kita kehilangan uang
setiap tahun.


Bagaimana kita bisa menentukan berapa tahun uang itu akan bertahan?
Kita harus menulis loop untuk ini. Cara termudah adalah dengan iterasi
cukup lama.


\>VKR=iterate("onepay",5000,50)


    Real 1 x 51 matrix
    
        5000.00     4950.00     4898.50     4845.45     ...

Dengan menggunakan bahasa matriks, kita dapat menentukan nilai negatif
pertama dengan cara berikut.


\>min(nonzeros(VKR<0))


          48.00 

Alasan untuk ini adalah bahwa bukan nol(VKR&lt;0) mengembalikan vektor
indeks i, di mana VKR[i]&lt;0, dan min menghitung indeks minimal.


Karena vektor selalu dimulai dengan indeks 1, jawabannya adalah 47
tahun.


Fungsi iterate() memiliki satu trik lagi. Itu bisa mengambil kondisi
akhir sebagai argumen. Kemudian akan mengembalikan nilai dan jumlah
iterasi.


\>{x,n}=iterate("onepay",5000,till="x<0"); x, n,


         -19.83 
          47.00 

Mari kita coba menjawab pertanyaan yang lebih ambigu. Asumsikan kita
tahu bahwa nilainya adalah 0 setelah 50 tahun. Apa yang akan menjadi
tingkat bunga?


Ini adalah pertanyaan yang hanya bisa dijawab dengan angka. Di bawah
ini, kita akan mendapatkan formula yang diperlukan. Kemudian Anda akan
melihat bahwa tidak ada formula yang mudah untuk tingkat bunga. Tapi
untuk saat ini, kami bertujuan untuk solusi numerik.


Langkah pertama adalah mendefinisikan fungsi yang melakukan iterasi
sebanyak n kali. Kami menambahkan semua parameter ke fungsi ini.


\>function f(K,R,P,n) := iterate("x\*(1+P/100)+R",K,n;P,R)[-1]


Iterasinya sama seperti di atas


Tapi kami tidak lagi menggunakan nilai global R dalam ekspresi kami.
Fungsi seperti iterate() memiliki trik khusus di Euler. Anda dapat
meneruskan nilai variabel dalam ekspresi sebagai parameter titik koma.
Dalam hal ini P dan R.


Selain itu, kami hanya tertarik pada nilai terakhir. Jadi kita ambil
indeks [-1].


Mari kita coba tes.


\>f(5000,-200,3,47)


         -19.83 

Sekarang kita bisa menyelesaikan masalah kita.


\>solve("f(5000,-200,x,50)",3)


           3.15 

Rutin memecahkan memecahkan ekspresi=0 untuk variabel x. Jawabannya
adalah 3,15% per tahun. Kami mengambil nilai awal 3% untuk algoritma.
Fungsi solve() selalu membutuhkan nilai awal.


Kita dapat menggunakan fungsi yang sama untuk menyelesaikan pertanyaan
berikut: Berapa banyak yang dapat kita keluarkan per tahun sehingga
modal awal habis setelah 20 tahun dengan asumsi tingkat bunga 3% per
tahun.


\>solve("f(5000,x,3,20)",-200)


        -336.08 

Perhatikan bahwa Anda tidak dapat memecahkan jumlah tahun, karena
fungsi kami mengasumsikan n sebagai nilai integer.


## Solusi Simbolik untuk Masalah Suku Bunga

Kita dapat menggunakan bagian simbolik dari Euler untuk mempelajari
masalah tersebut. Pertama kita mendefinisikan fungsi onepay() kita
secara simbolis.


\>function op(K) &= K\*q+R; $&op(K)


$$R+q\,K$$Kita sekarang dapat mengulangi ini.


\>$&op(op(op(op(K)))), $&expand(%)


$$q\,\left(q\,\left(q\,\left(R+q\,K\right)+R\right)+R\right)+R$$$$q^3\,R+q^2\,R+q\,R+R+q^4\,K$$Kami melihat sebuah pola. Setelah n periode yang kita miliki


lateks: K_n = q^n K + R (1+q+\ldots+q^{n-1}) = q^n K +
\frac{q^n-1}{q-1} R


Rumusnya adalah rumus untuk jumlah geometri, yang diketahui Maxima.


\>&sum(q^k,k,0,n-1); $& % = ev(%,simpsum)


$$\sum_{k=0}^{n-1}{q^{k}}=\frac{q^{n}-1}{q-1}$$Ini agak rumit. Jumlahnya dievaluasi dengan bendera "simpsum" untuk
menguranginya menjadi hasil bagi.


Mari kita membuat fungsi untuk ini.


\>function fs(K,R,P,n) &= (1+P/100)^n\*K + ((1+P/100)^n-1)/(P/100)\*R; $&fs(K,R,P,n)


$$\frac{100\,\left(\left(\frac{P}{100}+1\right)^{n}-1\right)\,R}{P}+K
 \,\left(\frac{P}{100}+1\right)^{n}$$Fungsi tersebut melakukan hal yang sama seperti fungsi f kita
sebelumnya. Tapi itu lebih efektif.


\>longest f(5000,-200,3,47), longest fs(5000,-200,3,47)


         -19.82504734650985 
         -19.82504734652684 

Kita sekarang dapat menggunakannya untuk menanyakan waktu n. Kapan
modal kita habis? Dugaan awal kami adalah 30 tahun.


\>solve("fs(5000,-330,3,x)",30)


          20.51 

Jawaban ini mengatakan bahwa itu akan menjadi negatif setelah 21
tahun.


Kita juga dapat menggunakan sisi simbolis Euler untuk menghitung
formula pembayaran.


Asumsikan kita mendapatkan pinjaman sebesar K, dan membayar n
pembayaran sebesar R (dimulai setelah tahun pertama) meninggalkan sisa
hutang sebesar Kn (pada saat pembayaran terakhir). Rumus untuk ini
jelas


\>equ &= fs(K,R,P,n)=Kn; $&equ


$$\frac{100\,\left(\left(\frac{P}{100}+1\right)^{n}-1\right)\,R}{P}+K
 \,\left(\frac{P}{100}+1\right)^{n}={\it Kn}$$Biasanya rumus ini diberikan dalam bentuk


$$i = \frac{P}{100}$$\>equ &= (equ with P=100\*i); $&equ


$$\frac{\left(\left(i+1\right)^{n}-1\right)\,R}{i}+\left(i+1\right)^{
 n}\,K={\it Kn}$$Kita dapat memecahkan tingkat R secara simbolis.


\>$&solve(equ,R)


$$\left[ R=\frac{i\,{\it Kn}-i\,\left(i+1\right)^{n}\,K}{\left(i+1
 \right)^{n}-1} \right] $$Seperti yang Anda lihat dari rumus, fungsi ini mengembalikan kesalahan
titik mengambang untuk i=0. Euler tetap merencanakannya.


Tentu saja, kami memiliki batas berikut.


\>$&limit(R(5000,0,x,10),x,0)


$$\lim_{x\rightarrow 0}{R\left(5000 , 0 , x , 10\right)}$$Jelas, tanpa bunga kita harus membayar kembali 10 tarif 500.


Persamaan juga dapat diselesaikan untuk n. Kelihatannya lebih bagus,
jika kita menerapkan beberapa penyederhanaan untuk itu.


\>fn &= solve(equ,n) | ratsimp; $&fn


$$\left[ n=\frac{\log \left(\frac{R+i\,{\it Kn}}{R+i\,K}\right)}{
 \log \left(i+1\right)} \right] $$---



CONTOH SOAL ALJABAR ** EXERCISE SET R.2


1. Sederhanakan bentuk eksponen berikut!


$$\left( \frac {24a^{10}b^{-8}c^7}{12a^6b^{-3}c^5} \right)^{-5}$$Penyelesaian :


\>$&((24\*a^10\*b^(-8)\*c^7) / (12\*a^6\*b^(-3)\*c^5))^(-5)


$$\frac{b^{25}}{32\,a^{20}\,c^{10}}$$2. Sederhanakan bentuk eksponen berikut!


$$\left( \frac {125p^{12}q^{-14}r^{22}}{25p^8q^6r^{-15}} \right)^{-4}$$Penyelesaian :


\>$& ((125\*p^12\*q^-14\*r^22) / (25\*p^8\*q^6\*r^-15))^(-4)


$$\frac{q^{80}}{625\,p^{16}\,r^{148}}$$3. Hitunglah operasi matematika di bawah ini!


$$\frac{[4(8-6)^2+4](3-2\cdot8)}{2^2(2^3+5)}$$Penyelesaian :


\>$&((4\*(8-6)^2+4)\*(3-2\*8))/(2^2\*(2^3+5))


$$-5$$## EXERCISE SET R.3

1.Selesaikan operasi matematika di bawah ini!


$$(3a^2)(-7a^4)$$Penyelesaian :


\>$&(3\*a^2)\*(-7\*a^4)


$$-21\,a^6$$2.Selesaikan operasi matematika di bawah ini!


$$(2x+3y+z-7)+(4x-2y-z+8)+(-3x+y-2z-4)$$Penyelesaian :


\>$&(2\*x+3\*y+z-7)+(4\*x-2\*y-z+8)+(-3\*x+y-2\*z-4)


$$-2\,z+2\,y+3\,x-3$$3. Asumsikan bahwa semua eksponen adalah bilangan asli.


Carilah hasil di bawah ini!


$$(a^n+b^n)(a^n-b^n)$$Penyelesaian :


\>$&expand((a^n+b^n)\*(a\*n-b^n))


$$a^{n+1}\,n+a\,b^{n}\,n-b^{2\,n}-a^{n}\,b^{n}$$4. Asumsikan bahwa semua eksponen adalah bilangan asli.


Carilah hasil di bawah ini!


$$(a^n+b^n)^2$$Penyelesaian :


\>$&expand((a^n+b^n)^2)


$$b^{2\,n}+2\,a^{n}\,b^{n}+a^{2\,n}$$5. Hasil dari


$$(2a-3b)(2a-b)$$Penyelesaian:


\>$&expand((2\*a-3\*b)\*(2\*a-b))


$$3\,b^2-8\,a\,b+4\,a^2$$## EXERCISE SET R.4

1.Hitunglah faktor dari :


$$x^3-4x^2+5x-20$$Penyelesaian :


\>$&factor(x^3-4\*x^2+5\*x-20)


$$\left(x-4\right)\,\left(x^2+5\right)$$2.Hitunglah faktor dari :


$$125a - 8a^4$$Penyelesaian :


\>$&factor(125\*a-8\*a^4)


$$-a\,\left(2\,a-5\right)\,\left(4\,a^2+10\,a+25\right)$$ 3. Carilah Faktor dari soal di bawah ini!  

$$m^6+8m^3-20$$Penyelesaian :


\>$&factor(m^6+8\*m^3-20)


$$\left(m^3-2\right)\,\left(m^3+10\right)$$ 4. Carilah Faktor dari soal di bawah ini!  

$$16a^7b+54ab^7$$Penyelesaian :


\>$&factor(16\*a^7\*b+54\*a\*b^7)


$$2\,a\,b\,\left(3\,b^2+2\,a^2\right)\,\left(9\,b^4-6\,a^2\,b^2+4\,a^
 4\right)$$5. Carilah Faktor dari soal di bawah ini!


$$p-64p^4$$Penyelesaian :


\>$&factor(p-64\*p^4)


$$-p\,\left(4\,p-1\right)\,\left(16\,p^2+4\,p+1\right)$$## EXERCISE SET R.5

1. Tentukan nilai z dari persamaan berikut!


$$z^2=144$$Penyelesaian:


\>$&solve(z^2=144)


$$\left[ z=-12 , z=12 \right] $$2. Tentukan nilai x dari persamaan berikut!


$$2x^2-20=0$$Penyelesaian:


\>$&solve(2\*x^2-20=0)


$$\left[ x=-\sqrt{10} , x=\sqrt{10} \right] $$3. Tentukan nilai y dari persamaan berikut!


$$9y^2+15y+4=0$$Penyelesaian:


\>$&solve(9\*y^2+15\*y+4=0)


$$\left[ y=-\frac{4}{3} , y=-\frac{1}{3} \right] $$4. Selesaika soal i bawah ini!


$$3[5-3(4-t)]-2=5[3(5t-4)+8]-26$$Penyelesaian:


\>$&solve(3\*(5-3\*(4-t))-2=5\*(3\*(5\*t-4)+8)-26)


$$\left[ t=\frac{23}{66} \right] $$5. Selesaika soal i bawah ini!


$$3x^3+6x^2-27x-54=0$$Penyelesaian:


\>$&solve(3\*x^3+6\*x^2-27\*x-54=0)


$$\left[ x=-3 , x=-2 , x=3 \right] $$## EXERCISE SET R.6

1.Selesaikan operasi matematika di bawah ini!


$$\left( \frac{x^2-4}{x^2-4x+4}\right)$$Penyelesaian:


\>$&solve((x^2-4)/(x^2-4\*x+4))


$$\left[ x=-2 \right] $$2.Selesaikan operasi matematika di bawah ini!


$$ \frac{3}{x+2}+ \frac{2}{x^2-4}$$Penyelesaian:


\>$&solve(3/(x+2)+2/(x^2-4))


$$\left[ x=\frac{4}{3} \right] $$3.Selesaikan operasi matematika di bawah ini!


$$\frac{7}{12y}- \frac{1}{12y}$$Penyelesaian :


\>$&solve((7/12\*y)-(1/12\*y))


$$\left[ y=0 \right] $$4.Selesaikan operasi matematika di bawah ini!


$$\frac{x}{2x-3y}- \frac{y}{3y-2x}$$Penyelesaian :


\>$&solve(x/(2\*x)-(3\*y))-(y/(3\*y)-(2\*x))


$$\left[ y+2\,x-\frac{1}{3}=2\,x-\frac{1}{6} \right] $$5.Selesaikan operasi matematika di bawah ini!


$$\frac{a-a^-1}{a+a^-1}$$

Penyelesaian :


\>$&solve((a-a^(-1))/(a+a^(-1)))


$$\left[ a=-1 , a=1 \right] $$# CONTOH SOAL ALJABAR LAINNYA ** Bilangan Real (Asli)

1. Tentukan nilai real dari


$$\frac{2}{7}$$Penyelesaian


\>longest 2/7


         0.2857142857142857 

\>printdual(2/7)


    1.0010010010010010010010010010010010010010010010010010*2^-2

\>printhex(2/7)


    4.9249249249248*16^-1

2. Tentukan nilai real dari


$$\frac{12}{27}$$Penyelesaian


\>longest 12/27


         0.4444444444444444 

\>printdual (12/27)


    1.1100011100011100011100011100011100011100011100011100*2^-2

\>printhex (12/27)


    7.1C71C71C71C70*16^-1

## String

1. Tuliskan string dari "Aku gemar memasak"


Penyelesaian :


\>"Aku gemar memasak"


    Aku gemar memasak

## Nilai Boolean

1. benarkah bahwa:


$$(5 > 9) and (12 < 8)$$Penyelesaian :


\>5 \> 9 && 12 < 8


           0.00 

2. Apakah benar bahwa:


$$(9 > 3) and (2 < 7)$$Penyelesaian :


\>9 \> 3 && 2 < 7


           1.00 

## Keluaran



1. Tulisan format keluaran dari nilai :


$$tan (180)$$Penyelesaian :


\>defformat; tan(180)


    1.33869021035

\>longest tan(180)


          1.338690210351154 

\>printhex (tan(180))


    1.56B466D0EEFE6*16^0

\>longestformat; tan(180)


    1.338690210351154

## Matematika Simbolik

1. Hitunglah hasil dari soal berikut :


$$C(97,10) = \frac{70!}{46! \cdot 10!}$$Penyelesaian :


\>$& 70!/(46!\*10!) // nilai C(97,10)


$$599890949750448950864996706140160000$$\>$binomial(97,10) //menghitung C(97,10) menggunakan fungsi binomial()


$$12576469727536$$2. Hitunglah hasil dari soal berikut :


$$C(x,9)=\frac{x!}{(x-8)!7!}=\frac{(x-4)(x-2)x}{8}$$Penyelesaian :


\>$binomial(x,9) // c(x,9)


$$\frac{\left(x-8\right)\,\left(x-7\right)\,\left(x-6\right)\,\left(x
 -5\right)\,\left(x-4\right)\,\left(x-3\right)\,\left(x-2\right)\,
 \left(x-1\right)\,x}{362880}$$\>$&binomial(x,9) with x=10 // substitusi x=10 ke C(x,9)


$$10$$\>&"v := 8; v^2"


    
                                      64
    

3. Hitunglah faktor dari 870


Penuyelesaian :


\>&factor(870!)


    
            2596819011193403785861881359301482890710627924419305029611134\
    958469915953823239021428165285926580429812995070504553921687642023033\
    717981219194331070830763945636296833137496249393750040169029586060946\
    092513959476892023786715788258771339261079415350581478562758329240721\
    444608935926749235597425126102044576377537768369377001787092908065233\
    588569196700474709060590764347221250074451703349901838190096131266067\
    962998675698068893037085495147764496120996506878668761107952193017381\
    627975601656718676241536018626688849274833763950662032143475966744196\
    422955121677681538595847372067881343514682093158221066669571676822999\
    748962857865047356703005652709574065659540833700859653349082765872673\
    647719649672181366313717294752638660580057118846834844146890700664463\
    076641726729046893056019867672484876135661154468463568173059293017070\
    539225352981572809421003315269470955737240608334564501234837273851217\
    454839654555717938710185388219560700530909108753005940014089296902888\
    895241876765339210795971583849462336291113056654803259207379253797788\
    864936221226509576375689562742482986437486352351023675306683227259287\
    788480160547408504816093286560417461042376342726742180427550315706285\
    180690105623364323046248497231048902701177178145054985011168631159511\
    485480056899556486234365390255648619611461591746051159928980855982249\
    779268148997264952803095528887648584566322667239408458845308353495441\
    517486976532553169555307483959161770513249264886192777344864766566063\
    674487031984714930869203025812725713885519371464609988429539630150837\
    150435582366839540096614943201938034120403791774321199275143016517055\
    734151877283279445567354133560328291713759965967563965402021934963526\
    190170717735851789780470967241345875356524988955902032996388875707891\
    256080290132211577865437807856201671231976703681888000076945775073513\
    135134690925571613332586110964218623822529621515080487430306516508652\
    982006075289391271598515379491664530861207178796063894885056343392523\
    871972685054173475246302943098657225624780800000000000000000000000000\
    000000000000000000000000000000000000000000000000000000000000000000000\
    000000000000000000000000000000000000000000000000000000000000000000000\
    000000000000000000000000000000000000000000000000000
    

\>::: factor(870!)


    
             864  432  215  143   86   71   54   47   38   31   28   23
            2    3    5    7    11   13   17   19   23   29   31   37
       21   20   18   16   14   14   12   12   11   11   10   9   8    8
     41   43   47   53   59   61   67   71   73   79   83   89  97  101
        8    8    7    7    6    6    6    6    5    5    5    5    5    5
     103  107  109  113  127  131  137  139  149  151  157  163  167  173
        4    4    4    4    4    4    4    3    3    3    3    3    3    3
     179  181  191  193  197  199  211  223  227  229  233  239  241  251
        3    3    3    3    3    3    3    2    2    2    2    2    2    2
     257  263  269  271  277  281  283  293  307  311  313  317  331  337
        2    2    2    2    2    2    2    2    2    2    2    2    2    2
     347  349  353  359  367  373  379  383  389  397  401  409  419  421
        2    2
     431  433  439 443 449 457 461 463 467 479 487 491 499 503 509 521 523
     541 547 557 563 569 571 577 587 593 599 601 607 613 617 619 631 641
     643 647 653 659 661 673 677 683 691 701 709 719 727 733 739 743 751
     757 761 769 773 787 797 809 811 821 823 827 829 839 853 857 859 863
    

## Matriks



1. selesaikan matrik di bawah ini!


$$A=[5,6;7,8]$$Penyelesaian :


\>A=[5,6;7,8]


                          5                       6 
                          7                       8 

\>a=[5;6]


                          5 
                          6 

\>a'


    [5,  6]

\>inv(A)


         -4.000000000000002       3.000000000000001 
          3.500000000000002      -2.500000000000001 

\>A.a


                         61 
                         83 

\>A^2


                         25                      36 
                         49                      64 

\>A.A.A.A


                      11587                   13494 
                      15743                   18334 

\>power(A,8)


                  346694611               403753974 
                  471046303               548571598 

\>A/A


                          1                       1 
                          1                       1 

\>A/a


                          1                     1.2 
          1.166666666666667       1.333333333333333 

\>inv(A).a


                         -2 
                        2.5 

\>A\\A  //A^(-1)A


                          1                       0 
                          0                       1 

\>inv(A).A


          1.000000000000004                       0 
     -3.552713678800501e-15                       1 

\>A\*A


                         25                      36 
                         49                      64 

\>a^2


                         25 
                         36 

\>A|1


    Real 2 x 3 matrix
    
                          5     ...
                          7     ...

## Masalah suku bunga

1. Sebuah ruko akan dijual dengan harga $88,000 dengan uang muka
sebanyak $10,000. Jika seseorang meminjam uang untuk membeli ruko
tersebut dengan lama pinjaman 20 tahun dan suku bunga 5,4%, maka
berapa jumlah yang harus dibayarkan oleh peminjam di setiap bulannya


Penyelesaian :


\>K=88000-10000, q=1+5.4%, format(12,2); (K\*q^20)/(12\*20)


    78000
    1.054
         930.46 

# Menggambar Grafik 2D dengan EMT

Notebook ini menjelaskan tentang cara menggambar berbagaikurva dan
grafik 2D dengan software EMT. EMT menyediakan fungsi plot2d() untuk
menggambar berbagai kurva dan grafik dua dimensi (2D).


## Basic Plots

Ada fungsi plot yang sangat mendasar. Ada koordinat layar, yang selalu
berkisar dari 0 hingga 1024 di setiap sumbu, tidak peduli apakah
layarnya persegi atau tidak. Semut ada koordinat plot, yang dapat
diatur dengan setplot(). Pemetaan antara koordinat tergantung pada
jendela plot saat ini. Misalnya, shrinkwindow() default menyisakan
ruang untuk label sumbu dan judul plot.


Dalam contoh, kita hanya menggambar beberapa garis acak dalam berbagai
warna. Untuk detail tentang fungsi-fungsi ini, pelajari fungsi inti
EMT.


\>clg; // clear screen


Fungsi utamanya adalah untuk menghilangkan semua tampilan atau
informasi yang sebelumnya muncul di layar agar layar menjadi kosong
kembali.


\>window(0,0,1024,1024); // use all of the window


Fungsi window(0,0,1024,1024) berarti menetapkan atau mengatur ukuran
dan posisi jendela tampilan.


Penjelasan dari fungsi tersebut:


(0,0): Ini adalah koordinat titik awal (x, y) di layar, yang biasanya
merujuk ke pojok kiri atas dari layar atau jendela.


1024,1024: Ini merujuk ke lebar dan tinggi jendela dalam piksel.


\>setplot(0,1,0,1); // set plot coordinates


Fungsi setplot(0,1,0,1) digunakan untuk menetapkan rentang atau skala
koordinat dalam sebuah grafik atau plot.


Penjelasan dari fungsi tersebut:


0, 1 (untuk sumbu x): Ini berarti sumbu x dari grafik akan mulai dari
nilai 0 hingga 1.


0, 1 (untuk sumbu y): Ini berarti sumbu y dari grafik akan mulai dari
nilai 0 hingga 1.


\>hold on; // start overwrite mode


Fungsi hold on; digunakan untuk mempertahankan grafik yang sudah ada,
sehingga grafik baru yang ditambahkan akan ditumpuk atau ditambahkan
di atas grafik yang sudah ada, tanpa menghapus atau menimpa grafik
sebelumnya.


\>n=100; X=random(n,2); Y=random(n,2);  // get random points


Fungsi ini menghasilkan titik acak dalam bentuk koordinat (x, y) untuk
digunakan dalam sebuah grafik atau analisis data.


n=100;: Menetapkan nilai n sebagai 100. Ini berarti Anda ingin
menghasilkan 100 titik acak.


X=random(n,2);: Menghasilkan 100 titik acak untuk koordinat x. Fungsi
random(n,2) berarti bahwa matriks X akan berukuran 100 baris dan 2
kolom. Setiap baris berisi dua angka acak, yang mewakili dua dimensi
dari koordinat acak untuk setiap titik.


Y=random(n,2);: Serupa dengan X, ini menghasilkan 100 titik acak untuk
koordinat y. Fungsi random(n,2) di sini juga menghasilkan matriks 100
baris dan 2 kolom.


\>colors=rgb(random(n),random(n),random(n)); // get random colors


Fungsi colors=rgb(random(n),random(n),random(n)); digunakan untuk
menghasilkan warna acak dengan menggunakan nilai RGB (Red, Green,
Blue).Penjelasan dari fungsi diatas:


random(n): Ini menghasilkan n angka acak (dalam kasus ini, 100 angka
acak, karena sebelumnya n=100).


rgb(random(n),random(n),random(n)): Fungsi rgb menerima tiga
parameter, yaitu nilai acak untuk Red (R), Green (G), dan Blue (B).
Setiap parameter akan berisi daftar angka acak antara 0 dan 1 (atau 0
hingga 255 tergantung pada implementasi), yang mewakili intensitas
dari masing-masing warna.


colors: Variabel ini akan berisi 100 warna acak yang dihasilkan oleh
kombinasi acak dari nilai Red, Green, dan Blue. Setiap warna akan unik
dan dibentuk dari kombinasi acak dari ketiga komponen warna tersebut.


\>loop 1 to n; color(colors[#]); plot(X[#],Y[#]); end; // plot


FUngsi loop 1 to n; color(colors[#]); plot(X[#],Y[#]); end; berarti
melakukan looping atau perulangan dari 1 hingga n (yang dalam hal ini
n = 100) untuk memplot titik acak dengan warna acak yang dihasilkan.


Penjelasan dari fungsi diatas:


loop 1 to n;: Melakukan perulangan dari angka 1 hingga n (dalam hal
ini n = 100). Artinya, ada 100 iterasi.


color(colors[#]);: Pada setiap iterasi, fungsi ini memilih satu warna
acak dari array colors yang telah dihasilkan sebelumnya. Simbol #
adalah indeks yang sesuai dengan iterasi saat ini, jadi pada iterasi
pertama, itu adalah warna pertama, dan seterusnya.


plot(X[#],Y[#]);: Ini memplot titik pada koordinat (X[#], Y[#]), di
mana X[#] dan Y[#] masing-masing adalah nilai x dan y dari titik acak
yang sudah dihasilkan sebelumnya. Simbol # lagi-lagi menunjukkan
indeks iterasi saat ini, sehingga setiap titik memiliki koordinat dan
warna yang unik.


end;: Mengakhiri loop. Setelah semua titik dari 1 hingga n selesai
diplot, loop berhenti.


\>hold off; // end overwrite mode


Fungsi hold off; digunakan untuk mengembalikan ke mode default, di
mana grafik baru menimpa yang lama. Setelah ini, grafik berikutnya
yang diplot akan menggantikan plot yang sebelumnya, bukan
menambahkannya.


\>insimg; // insert to notebook


![images/Final%20Projek%20APLIKOM-171.png](images/Final%20Projek%20APLIKOM-171.png)

Fungsi insimg; digunakan untuk menyisipkan gambar ke dalam notebook
atau dokumen. Ini memungkinkan pengguna untuk mengintegrasikan grafik,
plot, atau hasil visual lainnya ke dalam catatan mereka, sehingga
dapat dengan mudah dilihat dan dianalisis dalam konteks yang lebih
besar.


\>reset;


Penting untuk menahan grafik, karena perintah plot() akan menghapus
jendela plot.


Untuk menghapus semua yang kami lakukan, kami menggunakan reset().


Untuk menampilkan gambar hasil plot di layar notebook, perintah
plot2d() dapat diakhiri dengan titik dua (:). Cara lain adalah
perintah plot2d() diakhiri dengan titik koma (;), kemudian menggunakan
perintah insimg() untuk menampilkan gambar hasil plot.


Untuk contoh lain, kita menggambar plot sebagai sisipan di plot lain.
Ini dilakukan dengan menentukan jendela plot yang lebih kecil.
Perhatikan bahwa jendela ini tidak menyediakan ruang untuk label sumbu
di luar jendela plot. Kita harus menambahkan beberapa margin untuk ini
sesuai kebutuhan. Perhatikan bahwa kita menyimpan dan memulihkan
jendela penuh, dan menahan plot saat ini sementara kita memplot
sisipan.


\>plot2d("x^3-x");


Fungsi plot2d("x^3-x"); dalam bahasa EMT (Ekspresi Menggunakan
Tindakan) digunakan untuk memplot grafik dua dimensi dari fungsi
matematika yang diberikan, dalam hal ini, fungsi


$$f(x)= x^{3}-x$$\>xw=200; yw=100; ww=300; hw=300;


xw: posisi x (horizontal) dari jendela.


yw: posisi y (vertikal) dari jendela.


ww: lebar jendela.


hw: tinggi jendela.


\>ow=window();


Menyimpan referensi ke jendela saat ini dalam variabel ow. Ini berguna
untuk mengembalikan ke jendela ini nanti.


\>window(xw,yw,xw+ww,yw+hw);


Mengatur jendela baru dengan posisi (xw, yw) sebagai sudut kiri atas
dan (xw+ww, yw+hw) sebagai sudut kanan bawah, berdasarkan nilai yang
telah didefinisikan.


\>hold on;


Mengaktifkan mode penambahan, sehingga grafik berikutnya akan
ditambahkan di atas grafik yang ada tanpa menghapusnya.


\>barclear(xw-50,yw-10,ww+60,ww+60);


Menghapus atau mengosongkan area grafik di sekitar koordinat yang
ditentukan. Ini akan menghapus area berbentuk persegi panjang di
jendela yang ditentukan oleh parameter yang diberikan.


\>plot2d("x^4-x",grid=6):


![images/Final%20Projek%20APLIKOM-173.png](images/Final%20Projek%20APLIKOM-173.png)

Memplot grafik dua dimensi dari fungsi


$$f(x)=x^{4}-4$$

dengan grid yang diatur pada tingkat 6, yang memberikan tampilan lebih
terstruktur pada grafik.


\>hold off;


Fungsi hold off; digunakan untuk mengakhiri mode penambahan grafik.
Ini berarti bahwa setelah perintah ini, grafik atau plot baru yang
dibuat akan menimpa grafik yang ada sebelumnya, bukan menambahkannya.


\>window(ow);


Plot dengan beberapa angka dicapai dengan cara yang sama. Ada fungsi
utilitas figure() untuk ini.


## Aspek Plot

Plot default menggunakan jendela plot persegi. Anda dapat mengubahnya
dengan fungsi aspect(). Jangan lupa untuk mengatur ulang aspek nanti.
Anda juga dapat mengubah default ini di menu dengan "Set Aspect" ke
rasio aspek tertentu atau ke ukuran jendela grafis saat ini.


Tetapi Anda dapat mengubahnya juga untuk satu plot. Untuk ini, ukuran
area plot saat ini diubah, dan jendela diatur sehingga label memiliki
ruang yang cukup.


\>aspect(2); // rasio panjang dan lebar 2:1


Fungsi ini mengatur rasio aspek dari grafik yang akan dibuat. Dengan
parameter 2, rasio panjang dan lebar grafik akan menjadi 2:1. Ini
berarti lebar grafik akan dua kali lipat dari tingginya, yang dapat
membantu dalam memperjelas visualisasi fungsi yang memiliki rentang
nilai yang lebih lebar.


\>plot2d(["sin(x)","cos(x)"],0,2pi):


![images/Final%20Projek%20APLIKOM-175.png](images/Final%20Projek%20APLIKOM-175.png)

\>aspect();


Fungsi aspect(); tanpa parameter biasanya digunakan untuk
mengembalikan rasio aspek grafik ke pengaturan default.


\>reset;


Fungsi reset() mengembalikan default plot termasuk rasio aspek.


Plot 2D di Euler


EMT Math Toolbox memiliki plot dalam 2D, baik untuk data maupun
fungsi. EMT menggunakan fungsi plot2d. Fungsi ini dapat memplot fungsi
dan data.


Dimungkinkan untuk memplot di Maxima menggunakan Gnuplot atau di
Python menggunakan Math Plot Lib.


Euler dapat memplot plot 2D dari


* 
ekspresi

* 
fungsi, variabel, atau kurva parameter,

* 
vektor nilai xy,

* 
awan titik di pesawat,

* 
kurva implisit dengan level atau area level.

* 
Fungsi kompleks


Gaya plot mencakup berbagai gaya untuk garis dan titik, plot batang,
dan plot berarsir.


Plot Ekspresi atau Variabel


Satu ekspresi dalam "x" (misalnya "4*x^2") atau nama fungsi (misalnya
"f") menghasilkan grafik fungsi.


Berikut adalah contoh paling dasar, yang menggunakan rentang default
dan mengatur y-range yang tepat agar sesuai dengan plot fungsi.


Catatan: Jika Anda mengakhiri baris perintah dengan titik dua ":",
plot akan dimasukkan ke dalam jendela teks. Jika tidak, tekan TAB
untuk melihat plot jika jendela plot tertutup.


\>plot2d("x^2"):


![images/Final%20Projek%20APLIKOM-176.png](images/Final%20Projek%20APLIKOM-176.png)

\>aspect(1.5); plot2d("x^3-x"):


![images/Final%20Projek%20APLIKOM-177.png](images/Final%20Projek%20APLIKOM-177.png)

\>a:=5.6; plot2d("exp(-a\*x^2)/a"); insimg(30); // menampilkan gambar hasil plot setinggi 25 baris


![images/Final%20Projek%20APLIKOM-178.png](images/Final%20Projek%20APLIKOM-178.png)

Dari beberapa contoh sebelumnya Anda dapat melihat bahwa aslinya
gambar plot menggunakan sumbu X dengan rentang nilai dari -2 sampai
dengan 2. Untuk mengubah rentang nilai X dan Y, Anda dapat menambahkan
nilai-nilai batas X (dan Y) di belakang ekspresi yang digambar.


Rentang plot diatur dengan parameter yang ditetapkan berikut


* 
a,b: X-range (default -2,2)

* 
c,d: jrange-y (default: skala dengan nilai)

* 
r: atau jari-jari di sekitar pusat plot

* 
cx,cy: koordinat pusat plot (default 0,0)


\>plot2d("x^3-x",-1,2):


![images/Final%20Projek%20APLIKOM-179.png](images/Final%20Projek%20APLIKOM-179.png)

\>plot2d("sin(x)",-2\*pi,2\*pi): // plot sin(x) pada interval [-2pi, 2pi]


![images/Final%20Projek%20APLIKOM-180.png](images/Final%20Projek%20APLIKOM-180.png)

\>plot2d("cos(x)","sin(3\*x)",xmin=0,xmax=2pi):


![images/Final%20Projek%20APLIKOM-181.png](images/Final%20Projek%20APLIKOM-181.png)

Alternatif untuk titik dua adalah perintah insimg(lines), yang
menyisipkan plot yang menempati sejumlah baris teks tertentu.


Dalam opsi, plot dapat diatur untuk muncul


* 
di jendela terpisah yang dapat diubah ukurannya,

* 
di jendela buku catatan.


Lebih banyak gaya dapat dicapai dengan perintah plot tertentu.


Bagaimanapun, tekan tombol tabulator untuk melihat plotnya, jika
tersembunyi.


Untuk membagi jendela menjadi beberapa plot, gunakan perintah
figure(). Dalam contoh, kita memplot x^1 hingga x^4 menjadi 4 bagian
jendela. Figure(0) mengatur ulang jendela default.


\>reset;

\>figure(2,2); ...  
\>  
Fungsi figure(2,2); digunakan untuk mengatur ukuran jendela grafik
baru menjadi 2 x 2, yang memungkinkan pengguna untuk memvisualisasikan
grafik dengan cara yang terorganisir dan jelas.


\>for n=1 to 4; figure(n); plot2d("x^"+n); end; ...  
\>   figure(0):


![images/Final%20Projek%20APLIKOM-182.png](images/Final%20Projek%20APLIKOM-182.png)

Di plot2d(), ada gaya alternatif yang tersedia dengan grid=x. Untuk
gambaran umum, kami menunjukkan berbagai gaya kisi dalam satu gambar
(lihat di bawah untuk perintah figure(). Grid gaya grid = 0 tidak
disertakan. Ini tidak menunjukkan kisi dan tidak ada bingkai.


\>figure(3,3); ...  
\>   for k=1:9; figure(k); plot2d("x^3-x",-2,1,grid=k); end; ...  
\>   figure(0):


![images/Final%20Projek%20APLIKOM-183.png](images/Final%20Projek%20APLIKOM-183.png)

Jika argumen untuk plot2d() adalah ekspresi diikuti oleh empat angka,
angka-angka ini adalah rentang x dan y untuk plot.


Atau, a, b, c, d dapat ditentukan sebagai parameter yang ditetapkan
sebagai a=... dll.


Dalam contoh berikut, kita mengubah gaya kisi, menambahkan label, dan
menggunakan label vertikal untuk sumbu y.


\>aspect(1.5); plot2d("sin(x)",0,2pi,-1.2,1.2,grid=3,xl="x",yl="sin(x)"):


![images/Final%20Projek%20APLIKOM-184.png](images/Final%20Projek%20APLIKOM-184.png)

\>plot2d("sin(x)+cos(2\*x)",0,4pi):


![images/Final%20Projek%20APLIKOM-185.png](images/Final%20Projek%20APLIKOM-185.png)

Gambar yang dihasilkan dengan memasukkan plot ke dalam jendela teks
disimpan di direktori yang sama dengan buku catatan, secara default di
subdirektori bernama "images". Mereka juga digunakan oleh ekspor HTML.


Anda cukup menandai gambar apa pun dan menyalinnya ke clipboard dengan
Ctrl-C. Tentu saja, Anda juga dapat mengekspor grafik saat ini dengan
fungsi di menu File.


Fungsi atau ekspresi dalam plot2d dievaluasi secara adaptif. Untuk
kecepatan lebih, matikan plot adaptif dengan &lt;adaptif dan tentukan
jumlah subinterval dengan n=... Ini seharusnya diperlukan dalam kasus
yang jarang terjadi saja.


\>plot2d("sign(x)\*exp(-x^2)",-1,1,<adaptive,n=10000):


![images/Final%20Projek%20APLIKOM-186.png](images/Final%20Projek%20APLIKOM-186.png)

\>plot2d("x^x",r=1.2,cx=1,cy=1):


![images/Final%20Projek%20APLIKOM-187.png](images/Final%20Projek%20APLIKOM-187.png)

Perhatikan bahwa x^x tidak didefinisikan untuk x&lt;=0. Fungsi plot2d
menangkap kesalahan ini, dan mulai merencanakan segera setelah fungsi
ditentukan. Ini berfungsi untuk semua fungsi yang mengembalikan NAN di
luar jangkauan definisi mereka.


\>plot2d("log(x)",-0.1,2):


![images/Final%20Projek%20APLIKOM-188.png](images/Final%20Projek%20APLIKOM-188.png)

Parameter square=true (atau &gt;square) memilih jrange-y secara otomatis
sehingga hasilnya adalah jendela plot persegi. Perhatikan bahwa secara
default, Euler menggunakan ruang persegi di dalam jendela plot.


\>plot2d("x^3-x",\>square):


![images/Final%20Projek%20APLIKOM-189.png](images/Final%20Projek%20APLIKOM-189.png)

\>plot2d(''integrate("sin(x)\*exp(-x^2)",0,x)'',0,2): // plot integral


![images/Final%20Projek%20APLIKOM-190.png](images/Final%20Projek%20APLIKOM-190.png)

Jika Anda membutuhkan lebih banyak ruang untuk label-y, panggil
shrinkwindow() dengan parameter yang lebih kecil, atau atur nilai
positif untuk "smaller" di plot2d().


\>plot2d("gamma(x)",1,10,yl="y-values",smaller=6,<vertical):


![images/Final%20Projek%20APLIKOM-191.png](images/Final%20Projek%20APLIKOM-191.png)

Symbolic expressions can also be used, since they are stored as simple
string expressions.


\>x=linspace(0,2pi,1000); plot2d(sin(5x),cos(7x)):


![images/Final%20Projek%20APLIKOM-192.png](images/Final%20Projek%20APLIKOM-192.png)

\>a:=5.6; expr &= exp(-a\*x^2)/a; // define expression

\>plot2d(expr,-2,2): // plot from -2 to 2


![images/Final%20Projek%20APLIKOM-193.png](images/Final%20Projek%20APLIKOM-193.png)

\>plot2d(expr,r=1,thickness=2): // plot in a square around (0,0)


![images/Final%20Projek%20APLIKOM-194.png](images/Final%20Projek%20APLIKOM-194.png)

\>plot2d(&diff(expr,x),\>add,style="--",color=red): // add another plot


![images/Final%20Projek%20APLIKOM-195.png](images/Final%20Projek%20APLIKOM-195.png)

\>plot2d(&diff(expr,x,2),a=-2,b=2,c=-2,d=1): // plot in rectangle


![images/Final%20Projek%20APLIKOM-196.png](images/Final%20Projek%20APLIKOM-196.png)

\>plot2d(&diff(expr,x),a=-2,b=2,\>square): // keep plot square


![images/Final%20Projek%20APLIKOM-197.png](images/Final%20Projek%20APLIKOM-197.png)

\>plot2d("x^2",0,1,steps=1,color=red,n=10):


![images/Final%20Projek%20APLIKOM-198.png](images/Final%20Projek%20APLIKOM-198.png)

\>plot2d("x^2",\>add,steps=2,color=blue,n=10):


![images/Final%20Projek%20APLIKOM-199.png](images/Final%20Projek%20APLIKOM-199.png)

# Fungsi dalam satu Parameter

Fungsi plot yang paling penting untuk plot planar adalah plot2d().
Fungsi ini diimplementasikan dalam bahasa Euler dalam file "plot.e",
yang dimuat di awal program.


Berikut adalah beberapa contoh menggunakan fungsi. Seperti biasa di
EMT, fungsi yang berfungsi untuk fungsi atau ekspresi lain, Anda dapat
meneruskan parameter tambahan (selain x) yang bukan variabel global ke
fungsi dengan parameter titik koma atau dengan koleksi panggilan.


\>function f(x,a) := x^2/a+a\*x^2-x; // define a function

\>a=0.3; plot2d("f",0,1;a): // plot with a=0.3


![images/Final%20Projek%20APLIKOM-200.png](images/Final%20Projek%20APLIKOM-200.png)

\>plot2d("f",0,1;0.4): // plot with a=0.4


![images/Final%20Projek%20APLIKOM-201.png](images/Final%20Projek%20APLIKOM-201.png)

\>plot2d({{"f",0.2}},0,1): // plot with a=0.2


![images/Final%20Projek%20APLIKOM-202.png](images/Final%20Projek%20APLIKOM-202.png)

\>plot2d({{"f(x,b)",b=0.1}},0,1): // plot with 0.1


![images/Final%20Projek%20APLIKOM-203.png](images/Final%20Projek%20APLIKOM-203.png)

\>function f(x) := x^3-x; ...  
\>   plot2d("f",r=1):


![images/Final%20Projek%20APLIKOM-204.png](images/Final%20Projek%20APLIKOM-204.png)

Berikut adalah ringkasan fungsi yang diterima


* 
ekspresi atau ekspresi simbolis dalam x

* 
fungsi atau fungsi simbolis dengan nama sebagai "f"

* 
fungsi simbolis hanya dengan nama f


Fungsi plot2d() juga menerima fungsi simbolis. Untuk fungsi simbolis,
nama saja berfungsi.


\>function f(x) &= diff(x^x,x)


    
                                x
                               x  (log(x) + 1)
    

\>plot2d(f,0,2):


![images/Final%20Projek%20APLIKOM-205.png](images/Final%20Projek%20APLIKOM-205.png)

Tentu saja, untuk ekspresi atau ekspresi simbolis, nama variabel sudah
cukup untuk memplotnya.


\>expr &= sin(x)\*exp(-x)


    
                                  - x
                                 E    sin(x)
    

\>plot2d(expr,0,3pi):


![images/Final%20Projek%20APLIKOM-206.png](images/Final%20Projek%20APLIKOM-206.png)

\>function f(x) &= x^x;

\>plot2d(f,r=1,cx=1,cy=1,color=blue,thickness=2);

\>plot2d(&diff(f(x),x),\>add,color=red,style="-.-"):


![images/Final%20Projek%20APLIKOM-207.png](images/Final%20Projek%20APLIKOM-207.png)

Untuk gaya garis ada berbagai opsi.


* 
style="...". Pilih dari "-", "--", "-.", ".", ".-.", "-.-".

* 
color: Lihat di bawah untuk warna.

* 
ketebalan: Defaultnya adalah 1.


Warna dapat dipilih sebagai salah satu warna default, atau sebagai
warna RGB.


* 
0..15: indeks warna default.

* 
Konstanta warna: putih, hitam, merah, hijau, biru, cyan, zaitun,
* abu-abu muda, abu-abu, abu-abu gelap, oranye, hijau muda, pirus, biru
* muda, oranye muda, kuning

* 
RGB(Merah,Hijau,Biru): Parameter adalah real di [0,1].


\>plot2d("exp(-x^2)",r=2,color=red,thickness=3,style="--"):


![images/Final%20Projek%20APLIKOM-208.png](images/Final%20Projek%20APLIKOM-208.png)

Berikut adalah tampilan warna EMT yang telah ditentukan sebelumnya.


\>aspect(2); columnsplot(ones(1,16),lab=0:15,grid=0,color=0:15):


![images/Final%20Projek%20APLIKOM-209.png](images/Final%20Projek%20APLIKOM-209.png)

Kode ini mengatur rasio aspek grafik menjadi 2:1 dan kemudian membuat
diagram kolom dengan 16 kolom yang memiliki tinggi sama (1), setiap
kolom diberi label dari 0 hingga 15 dan diwarnai dengan variasi warna.
Grafik ini akan memiliki tampilan yang rapi dan terorganisir tanpa
garis grid di latar belakang.


fungsi aspect(2); mengatur rasio aspek grafik menjadi 2:1, yang
berarti lebar grafik akan dua kali lipat dari tingginya.


columnsplot: Fungsi ini digunakan untuk membuat diagram kolom (bar
chart) dari data yang diberikan.


ones(1,16): Membuat vektor baris yang berisi 16 elemen, semua bernilai
1. Ini berarti semua kolom akan memiliki tinggi yang sama (1).


lab=0:15: Menetapkan label untuk sumbu x dari kolom, mulai dari 0
hingga 15, yang akan menjadi label untuk setiap kolom.


grid=0: Mengatur grid pada plot menjadi tidak ada. Ini berarti tidak
akan ada garis grid yang ditampilkan di latar belakang.


color=0:15: Mengatur warna kolom dengan menggunakan skala warna dari 0
hingga 15, sehingga setiap kolom dapat memiliki warna yang berbeda.


Tapi Anda bisa menggunakan warna apa saja.


\>columnsplot(ones(1,16),grid=0,color=rgb(0,0,linspace(0,1,15))):


![images/Final%20Projek%20APLIKOM-210.png](images/Final%20Projek%20APLIKOM-210.png)

# Menggambar Beberapa Kurva pada bidang koordinat yang sama

Plot lebih dari satu fungsi (beberapa fungsi) ke dalam satu jendela
dapat dilakukan dengan cara yang berbeda. Salah satu metode adalah
menggunakan &gt;add untuk beberapa panggilan ke plot2d secara
keseluruhan, tetapi panggilan pertama. Kami telah menggunakan fitur
ini dalam contoh di atas.


\>aspect(); plot2d("cos(x)",r=2,grid=6); plot2d("x",style=".",\>add):


![images/Final%20Projek%20APLIKOM-211.png](images/Final%20Projek%20APLIKOM-211.png)

\>aspect(1.5); plot2d("sin(x)",0,2pi); plot2d("cos(x)",color=blue,style="--",\>add):


![images/Final%20Projek%20APLIKOM-212.png](images/Final%20Projek%20APLIKOM-212.png)

Salah satu kegunaan &gt;add adalah untuk menambahkan titik pada kurva.


\>plot2d("sin(x)",0,pi); plot2d(2,sin(2),\>points,\>add):


![images/Final%20Projek%20APLIKOM-213.png](images/Final%20Projek%20APLIKOM-213.png)

Kami menambahkan titik persimpangan dengan label (pada posisi "cl"
untuk kiri tengah), dan memasukkan hasilnya ke dalam buku catatan.
Kami juga menambahkan judul ke plot.


\>plot2d(["cos(x)","x"],r=1.1,cx=0.5,cy=0.5, ...  
\>     color=[black,blue],style=["-","."], ...  
\>     grid=1);

\>x0=solve("cos(x)-x",1);  ...  
\>     plot2d(x0,x0,\>points,\>add,title="Intersection Demo");  ...  
\>     label("cos(x) = x",x0,x0,pos="cl",offset=20):


![images/Final%20Projek%20APLIKOM-214.png](images/Final%20Projek%20APLIKOM-214.png)

Dalam demo berikut, kita memplot fungsi sinc(x)=sin(x)/x dan ekspansi
Taylor ke-8 dan ke-16. Kami menghitung ekspansi ini menggunakan Maxima
melalui ekspresi simbolik.


Plot ini dilakukan dalam perintah multi-baris berikut dengan tiga
panggilan ke plot2d(). Yang kedua dan ketiga memiliki set bendera
(&gt;add), yang membuat plot menggunakan rentang sebelumnya.


Kami menambahkan kotak label yang menjelaskan fungsinya.


\>$taylor(sin(x)/x,x,0,4)


$$\frac{x^4}{120}-\frac{x^2}{6}+1$$\>plot2d("sinc(x)",0,4pi,color=green,thickness=2); ...  
\>     plot2d(&taylor(sin(x)/x,x,0,8),\>add,color=blue,style="--"); ...  
\>     plot2d(&taylor(sin(x)/x,x,0,16),\>add,color=red,style="-.-"); ...  
\>     labelbox(["sinc","T8","T16"],styles=["-","--","-.-"], ...  
\>       colors=[black,blue,red]):


![images/Final%20Projek%20APLIKOM-216.png](images/Final%20Projek%20APLIKOM-216.png)

Dalam contoh berikut, kami menghasilkan Bernstein-Polynomial.


$$B_i(x) = \binom{n}{i} x^i (1-x)^{n-i}$$\>plot2d("(1-x)^10",0,1); // plot first function

\>for i=1 to 10; plot2d("bin(10,i)\*x^i\*(1-x)^(10-i)",\>add); end;

\>insimg;


![images/Final%20Projek%20APLIKOM-218.png](images/Final%20Projek%20APLIKOM-218.png)

Metode kedua adalah menggunakan sepasang matriks nilai-x dan matriks
nilai-y dengan ukuran yang sama.


Kami menghasilkan matriks nilai dengan satu Bernstein-Polynomial di
setiap baris. Untuk ini, kita cukup menggunakan vektor kolom i. Lihat
pengantar tentang bahasa matriks untuk mempelajari lebih detail.


\>x=linspace(0,1,500);


Fungsi ini akan menghasilkan vektor x yang berisi 500 titik yang
terdistribusi secara merata antara 0 dan 1, siap untuk digunakan dalam
analisis atau pemrograman lebih lanjut.


\>n=10; k=(0:n)'; // n is row vector, k is column vector

\>y=bin(n,k)\*x^k\*(1-x)^(n-k); // y is a matrix then

\>plot2d(x,y):


![images/Final%20Projek%20APLIKOM-219.png](images/Final%20Projek%20APLIKOM-219.png)

Perhatikan bahwa parameter warna dapat berupa vektor. Kemudian setiap
warna digunakan untuk setiap baris matriks.


\>x=linspace(0,1,200); y=x^(1:10)'; plot2d(x,y,color=1:10):


![images/Final%20Projek%20APLIKOM-220.png](images/Final%20Projek%20APLIKOM-220.png)

Metode lain adalah menggunakan vektor ekspresi (string). Anda kemudian
dapat menggunakan array warna, array gaya, dan array ketebalan dengan
panjang yang sama.


\>plot2d(["sin(x)","cos(x)"],0,2pi,color=4:5): 


![images/Final%20Projek%20APLIKOM-221.png](images/Final%20Projek%20APLIKOM-221.png)

\>plot2d(["sin(x)","cos(x)"],0,2pi): // plot vector of expressions


![images/Final%20Projek%20APLIKOM-222.png](images/Final%20Projek%20APLIKOM-222.png)

We can get such a vector from Maxima using makelist() and mxm2str().


\>v &= makelist(binomial(10,i)\*x^i\*(1-x)^(10-i),i,0,10) // make list


    
                    10            9              8  2             7  3
            [(1 - x)  , 10 (1 - x)  x, 45 (1 - x)  x , 120 (1 - x)  x , 
               6  4             5  5             4  6             3  7
    210 (1 - x)  x , 252 (1 - x)  x , 210 (1 - x)  x , 120 (1 - x)  x , 
              2  8              9   10
    45 (1 - x)  x , 10 (1 - x) x , x  ]
    

\>mxm2str(v) // get a vector of strings from the symbolic vector


    (1-x)^10
    10*(1-x)^9*x
    45*(1-x)^8*x^2
    120*(1-x)^7*x^3
    210*(1-x)^6*x^4
    252*(1-x)^5*x^5
    210*(1-x)^4*x^6
    120*(1-x)^3*x^7
    45*(1-x)^2*x^8
    10*(1-x)*x^9
    x^10

\>plot2d(mxm2str(v),0,1): // plot functions


![images/Final%20Projek%20APLIKOM-223.png](images/Final%20Projek%20APLIKOM-223.png)

Alternatif lain adalah menggunakan bahasa matriks Euler.


Jika sebuah ekspresi menghasilkan matriks fungsi, dengan satu fungsi
di setiap baris, semua fungsi ini akan diplot menjadi satu plot.


Untuk ini, gunakan vektor parameter dalam bentuk vektor kolom. Jika
array warna ditambahkan, itu akan digunakan untuk setiap baris plot.


\>n=(1:10)'; plot2d("x^n",0,1,color=1:10):


![images/Final%20Projek%20APLIKOM-224.png](images/Final%20Projek%20APLIKOM-224.png)

Ekspresi dan fungsi satu baris dapat melihat variabel global.


Jika Anda tidak dapat menggunakan variabel global, Anda perlu
menggunakan fungsi dengan parameter tambahan, dan meneruskan parameter
ini sebagai parameter titik koma.


Berhati-hatilah, untuk menempatkan semua parameter yang ditetapkan ke
akhir perintah plot2d. Dalam contoh kita meneruskan a=5 ke fungsi f,
yang kita plot dari -10 hingga 10.


\>function f(x,a) := 1/a\*exp(-x^2/a); ...  
\>   plot2d("f",-10,10;5,thickness=2,title="a=5"):


![images/Final%20Projek%20APLIKOM-225.png](images/Final%20Projek%20APLIKOM-225.png)

Ekspresi dan fungsi satu baris dapat melihat variabel global. Atau,
gunakan koleksi dengan nama fungsi dan semua parameter tambahan.
Daftar khusus ini disebut koleksi panggilan, dan itu adalah cara yang
lebih disukai untuk meneruskan argumen ke fungsi yang dengan
sendirinya diteruskan sebagai argumen ke fungsi lain.


Dalam contoh berikut, kita menggunakan loop untuk memplot beberapa
fungsi (lihat tutorial tentang pemrograman untuk loop).


Jika Anda tidak dapat menggunakan variabel global, Anda perlu
menggunakan fungsi dengan parameter tambahan, dan meneruskan parameter
ini sebagai parameter titik koma.


Berhati-hatilah, untuk menempatkan semua parameter yang ditetapkan ke
akhir perintah plot2d. Dalam contoh kita meneruskan a=5 ke fungsi f,
yang kita plot dari -10 hingga 10.


\>plot2d({{"f",1}},-10,10); ...  
\>   for a=2:10; plot2d({{"f",a}},\>add); end:


![images/Final%20Projek%20APLIKOM-226.png](images/Final%20Projek%20APLIKOM-226.png)

Kita dapat mencapai hasil yang sama dengan cara berikut menggunakan
bahasa matriks EMT. Setiap baris matriks f(x,a) adalah satu fungsi.
Selain itu, kita dapat mengatur warna untuk setiap baris matriks. Klik
dua kali pada fungsi getspectral() untuk penjelasan.


\>x=-10:0.01:10; a=(1:10)'; plot2d(x,f(x,a),color=getspectral(a/10)):


![images/Final%20Projek%20APLIKOM-227.png](images/Final%20Projek%20APLIKOM-227.png)

## Label Teks

Dekorasi sederhana bisa


* 
judul dengan title="..."

* 
label x dan y dengan xl="...", yl="..."

* 
label teks lain dengan label("...",x,y)


Perintah label akan memplot ke dalam plot saat ini pada koordinat plot
(x,y). Itu bisa mengambil argumen posisional.


\>plot2d("x^3-x",-1,2,title="y=x^3-x",yl="y",xl="x"):


![images/Final%20Projek%20APLIKOM-228.png](images/Final%20Projek%20APLIKOM-228.png)

\>expr := "log(x)/x"; ...  
\>     plot2d(expr,0.5,5,title="y="+expr,xl="x",yl="y"); ...  
\>     label("(1,0)",1,0); label("Max",E,expr(E),pos="lc"):


![images/Final%20Projek%20APLIKOM-229.png](images/Final%20Projek%20APLIKOM-229.png)

Ada juga fungsi labelbox(), yang dapat menampilkan fungsi dan teks.
Dibutuhkan vektor string dan warna, satu item untuk setiap fungsi.


\>function f(x) &= x^2\*exp(-x^2);  ...  
\>   plot2d(&f(x),a=-3,b=3,c=-1,d=1);  ...  
\>   plot2d(&diff(f(x),x),\>add,color=blue,style="--"); ...  
\>   labelbox(["function","derivative"],styles=["-","--"], ...  
\>      colors=[black,blue],w=0.4):


![images/Final%20Projek%20APLIKOM-230.png](images/Final%20Projek%20APLIKOM-230.png)

Kotak ini ditambatkan di kanan atas secara default, tetapi &gt;kiri
menambatkan di kiri atas. Anda dapat memindahkannya ke tempat mana pun
yang Anda suka. Posisi jangkar adalah sudut kanan atas kotak, dan
angkanya adalah pecahan dari ukuran jendela grafis. Lebarnya otomatis.


Untuk plot titik, kotak label juga berfungsi. Tambahkan parameter
&gt;poin, atau vektor bendera, satu untuk setiap label.


Dalam contoh berikut, hanya ada satu fungsi. Jadi kita bisa
menggunakan string alih-alih vektor string. Kami mengatur warna teks
menjadi hitam untuk contoh ini.


\>n=10; plot2d(0:n,bin(n,0:n),\>addpoints); ...  
\>   labelbox("Binomials",styles="[]",\>points,x=0.1,y=0.1, ...  
\>   tcolor=black,\>left):


![images/Final%20Projek%20APLIKOM-231.png](images/Final%20Projek%20APLIKOM-231.png)

Gaya plot ini juga tersedia di statplot(). Seperti pada plot2d() warna
dapat diatur untuk setiap baris plot. Ada lebih banyak plot khusus
untuk tujuan statistik (lihat tutorial tentang statistik).


\>statplot(1:10,random(2,10),color=[red,blue]):


![images/Final%20Projek%20APLIKOM-232.png](images/Final%20Projek%20APLIKOM-232.png)

Fitur serupa adalah fungsi textbox().


Lebar secara default adalah lebar maksimum baris teks. Tapi itu bisa
diatur oleh pengguna juga.


\>function f(x) &= exp(-x)\*sin(2\*pi\*x); ...  
\>   plot2d("f(x)",0,2pi); ...  
\>   textbox(latex("\\text{Example of a damped oscillation}\\ f(x)=e^{-x}sin(2\\pi x)"),w=0.85):


![images/Final%20Projek%20APLIKOM-233.png](images/Final%20Projek%20APLIKOM-233.png)

Label teks, judul, kotak label, dan teks lainnya dapat berisi string
Unicode (lihat sintaks EMT untuk selengkapnya tentang string Unicode).


\>plot2d("x^3-x",title=u"x &rarr; x&sup3; - x"):


![images/Final%20Projek%20APLIKOM-234.png](images/Final%20Projek%20APLIKOM-234.png)

Label pada sumbu x dan y dapat vertikal, serta sumbu.


\>plot2d("sinc(x)",0,2pi,xl="x",yl=u"x &rarr; sinc(x)",\>vertical):


![images/Final%20Projek%20APLIKOM-235.png](images/Final%20Projek%20APLIKOM-235.png)

**Getah


Anda juga dapat memplot rumus LaTeX jika Anda telah menginstal sistem
LaTeX. Saya merekomendasikan MiKTeX. Jalur ke biner "latex" dan
"dvipng" harus berada di jalur sistem, atau Anda harus mengatur LaTeX
di menu opsi.


Perhatikan, penguraian LaTeX itu lambat. Jika Anda ingin menggunakan
LaTeX dalam plot animasi, Anda harus memanggil latex() sebelum loop
sekali dan menggunakan hasilnya (gambar dalam matriks RGB).


Dalam plot berikut, kami menggunakan LaTeX untuk label x dan y, label,
kotak label, dan judul plot.


\>plot2d("exp(-x)\*sin(x)/x",a=0,b=2pi,c=0,d=1,grid=6,color=blue, ...  
\>     title=latex("\\text{Function $\\Phi$}"), ...  
\>     xl=latex("\\phi"),yl=latex("\\Phi(\\phi)")); ...  
\>   textbox( ...  
\>     latex("\\Phi(\\phi) = e^{-\\phi} \\frac{\\sin(\\phi)}{\\phi}"),x=0.8,y=0.5); ...  
\>   label(latex("\\Phi",color=blue),1,0.4):


![images/Final%20Projek%20APLIKOM-236.png](images/Final%20Projek%20APLIKOM-236.png)

Seringkali, kita menginginkan spasi non-konformal dan label teks pada
sumbu x. Kita dapat menggunakan xaxis() dan yaxis() seperti yang akan
kita tunjukkan nanti.


Cara termudah adalah dengan melakukan plot kosong dengan bingkai
menggunakan grid=4, dan kemudian menambahkan kisi dengan ygrid() dan
xgrid(). Dalam contoh berikut, kita menggunakan tiga string LaTeX
untuk label pada sumbu x dengan xtick().


\>plot2d("sinc(x)",0,2pi,grid=4,<ticks); ...  
\>   ygrid(-2:0.5:2,grid=6); ...  
\>   xgrid([0:2]\*pi,<ticks,grid=6);  ...  
\>   xtick([0,pi,2pi],["0","\\pi","2\\pi"],\>latex):


![images/Final%20Projek%20APLIKOM-237.png](images/Final%20Projek%20APLIKOM-237.png)

Tentu saja, fungsi juga dapat digunakan.


\>function map f(x) ...


    if x>0 then return x^4
    else return x^2
    endif
    endfunction
</pre>
Parameter "peta" membantu menggunakan fungsi untuk vektor. Untuk


plot, itu tidak perlu. Tetapi untuk menunjukkan bahwa vektorisasi


berguna, kami menambahkan beberapa poin kunci ke plot pada x=-1, x=0
dan x=1.


Pada plot berikut, kami juga memasukkan beberapa kode LaTeX. Kami
menggunakannya untuk


dua label dan kotak teks. Tentu saja, Anda hanya akan dapat
menggunakan


LaTeX jika Anda telah menginstal LaTeX dengan benar.


\>plot2d("f",-1,1,xl="x",yl="f(x)",grid=6);  ...  
\>   plot2d([-1,0,1],f([-1,0,1]),\>points,\>add); ...  
\>   label(latex("x^3"),0.72,f(0.72)); ...  
\>   label(latex("x^2"),-0.52,f(-0.52),pos="ll"); ...  
\>   textbox( ...  
\>     latex("f(x)=\\begin{cases} x^3 & x\>0 \\\\ x^2 & x \\le 0\\end{cases}"), ...  
\>     x=0.7,y=0.2):


![images/Final%20Projek%20APLIKOM-238.png](images/Final%20Projek%20APLIKOM-238.png)

## Interaksi Pengguna

Saat memplot fungsi atau ekspresi, parameter &gt;user memungkinkan
pengguna untuk memperbesar dan menggeser plot dengan tombol kursor
atau mouse. Pengguna dapat


* 
memperbesar dengan + atau -

* 
Pindahkan plot dengan tombol kursor

* 
Pilih jendela plot dengan mouse

* 
Setel ulang tampilan dengan spasi

* 
keluar dengan pengembalian


Tombol spasi akan mengatur ulang plot ke jendela plot asli.


Saat memplot data, bendera &gt;user hanya akan menunggu penekanan tombol.


\>plot2d({{"x^3-a\*x",a=1}},\>user,title="Press any key!"):


    Row index 2 out of bounds!
    Try "trace errors" to inspect local variables after errors.
    plot2d:
        if auto then k2[2]=k1[2]; endif;

\>plot2d("exp(x)\*sin(x)",user=true, ...  
\>     title="+/- or cursor keys (return to exit)"):


![images/Final%20Projek%20APLIKOM-239.png](images/Final%20Projek%20APLIKOM-239.png)

Berikut ini menunjukkan cara lanjutan interaksi pengguna (lihat
tutorial tentang pemrograman untuk detailnya).


Fungsi bawaan mousedrag() menunggu peristiwa mouse atau keyboard. Ini
melaporkan mouse ke bawah, mouse bergerak atau mouse ke atas, dan
penekanan tombol. Fungsi dragpoints() memanfaatkan ini, dan
memungkinkan pengguna menyeret titik apa pun dalam plot.


Kita membutuhkan fungsi plot terlebih dahulu. Sebagai contoh, kita
melakukan interpolasi dalam 5 titik dengan polinomial. Fungsi harus
diplot ke dalam area plot tetap.


\>function plotf(xp,yp,select) ...


      d=interp(xp,yp);
      plot2d("interpval(xp,d,x)";d,xp,r=2);
      plot2d(xp,yp,>points,>add);
      if select>0 then
        plot2d(xp[select],yp[select],color=red,>points,>add);
      endif;
      title("Drag one point, or press space or return!");
    endfunction
</pre>
Perhatikan parameter titik koma di plot2d (d dan xp), yang diteruskan
ke evaluasi fungsi interp(). Tanpa ini, kita harus menulis fungsi
plotinterp() terlebih dahulu, mengakses nilai-nilai secara global.


Sekarang kita menghasilkan beberapa nilai acak, dan biarkan pengguna
menyeret titik-titiknya.


\>t=-1:0.5:1; dragpoints("plotf",t,random(size(t))-0.5):


![images/Final%20Projek%20APLIKOM-240.png](images/Final%20Projek%20APLIKOM-240.png)

Ada juga fungsi, yang memplot fungsi lain tergantung pada vektor
parameter, dan memungkinkan pengguna menyesuaikan parameter ini.


Pertama kita membutuhkan fungsi plot.


\>function plotf([a,b]) := plot2d("exp(a\*x)\*cos(2pi\*b\*x)",0,2pi;a,b);


Kemudian kita membutuhkan nama untuk parameter, nilai awal dan matriks
rentang nx2, opsional garis judul.


Ada slider interaktif, yang dapat mengatur nilai oleh pengguna. Fungsi
dragvalues() menyediakan ini.


\>dragvalues("plotf",["a","b"],[-1,2],[[-2,2];[1,10]], ...  
\>     heading="Drag these values:",hcolor=black):


![images/Final%20Projek%20APLIKOM-241.png](images/Final%20Projek%20APLIKOM-241.png)

Dimungkinkan untuk membatasi nilai yang diseret ke bilangan bulat.
Sebagai contoh, kita menulis fungsi plot, yang memplot polinomial
Taylor derajat n ke fungsi kosinus.


\>function plotf(n) ...


    plot2d("cos(x)",0,2pi,>square,grid=6);
    plot2d(&"taylor(cos(x),x,0,@n)",color=blue,>add);
    textbox("Taylor polynomial of degree "+n,0.1,0.02,style="t",>left);
    endfunction
</pre>
Sekarang kita membiarkan derajat n bervariasi dari 0 hingga 20 dalam
20 pemberhentian. Hasil dari dragvalues() digunakan untuk memplot
sketsa dengan n ini, dan untuk memasukkan plot ke dalam buku catatan.


\>nd=dragvalues("plotf","degree",2,[0,20],20,y=0.8, ...  
\>      heading="Drag the value:"); ...  
\>   plotf(nd):


![images/Final%20Projek%20APLIKOM-242.png](images/Final%20Projek%20APLIKOM-242.png)

Berikut ini adalah demonstrasi sederhana dari fungsi tersebut.
Pengguna dapat menggambar di atas jendela plot, meninggalkan jejak
titik.


\>function dragtest ...


      plot2d(none,r=1,title="Drag with the mouse, or press any key!");
      start=0;
      repeat
        {flag,m,time}=mousedrag();
        if flag==0 then return; endif;
        if flag==2 then
          hold on; mark(m[1],m[2]); hold off;
        endif;
      end
    endfunction
</pre>
\>dragtest // lihat hasilnya dan cobalah lakukan!


## Gaya Plot 2D

Secara default, EMT menghitung kutu sumbu otomatis dan menambahkan
label ke setiap centang. Ini dapat diubah dengan parameter grid. Gaya
default sumbu dan label dapat dimodifikasi. Selain itu, label dan
judul dapat ditambahkan secara manual. Untuk mengatur ulang ke gaya
default, gunakan reset().


\>aspect();

\>figure(3,4); ...  
\>    figure(1); plot2d("x^3-x",grid=0); ... // no grid, frame or axis 


Tidak ada tampilan bingkai dan sumbu


\> figure(2); plot2d("x^3-x",grid=1); ... // x-y-axis


Terdapat sumbu x-y


\> figure(3); plot2d("x^3-x",grid=2); ... // default ticks

\> figure(4); plot2d("x^3-x",grid=3); ... // x-y- axis with labels inside

\> figure(5); plot2d("x^3-x",grid=4); ... // no ticks, only labels

\> figure(6); plot2d("x^3-x",grid=5); ... // default, but no margin

\> figure(7); plot2d("x^3-x",grid=6); ... // axes only

\> figure(8); plot2d("x^3-x",grid=7); ... // axes only, ticks at axis

\> figure(9); plot2d("x^3-x",grid=8); ... // axes only, finer ticks at axis

\> figure(10); plot2d("x^3-x",grid=9); ... // default, small ticks inside

\> figure(11); plot2d("x^3-x",grid=10); ...// no ticks, axes only

\> figure(0):


![images/Final%20Projek%20APLIKOM-243.png](images/Final%20Projek%20APLIKOM-243.png)

Parameter &lt;frame mematikan bingkai, dan framecolor=blue mengatur
bingkai ke warna biru.


Jika Anda menginginkan centang Anda sendiri, Anda dapat menggunakan
style=0, dan menambahkan semuanya nanti.


\>aspect(1.5); 

\>plot2d("x^3-x",grid=0); // plot

\>frame; xgrid([-1,0,1]); ygrid(0): // add frame and grid


![images/Final%20Projek%20APLIKOM-244.png](images/Final%20Projek%20APLIKOM-244.png)

Untuk judul plot dan label sumbu, lihat contoh berikut.


\>plot2d("exp(x)",-1,1);

\>textcolor(black); // set the text color to black

\>title(latex("y=e^x")); // title above the plot

\>xlabel(latex("x")); // "x" for x-axis

\>ylabel(latex("y"),\>vertical); // vertical "y" for y-axis

\>label(latex("(0,1)"),0,1,color=blue): // label a point


![images/Final%20Projek%20APLIKOM-245.png](images/Final%20Projek%20APLIKOM-245.png)

Sumbu dapat digambar secara terpisah dengan xaxis() dan yaxis().


\>plot2d("x^3-x",<grid,<frame);

\>xaxis(0,xx=-2:1,style="-\>"); yaxis(0,yy=-5:5,style="-\>"):


![images/Final%20Projek%20APLIKOM-246.png](images/Final%20Projek%20APLIKOM-246.png)

Teks pada plot dapat diatur dengan label(). Dalam contoh berikut, "lc"
berarti pusat bawah. Ini mengatur posisi label relatif terhadap
koordinat plot.


\>function f(x) &= x^3-x


    
                                     3
                                    x  - x
    

\>plot2d(f,-1,1,\>square);

\>x0=fmin(f,0,1); // compute point of minimum

\>label("Rel. Min.",x0,f(x0),pos="lc"): // add a label there


![images/Final%20Projek%20APLIKOM-247.png](images/Final%20Projek%20APLIKOM-247.png)

Ada juga kotak teks.


\>plot2d(&f(x),-1,1,-2,2); // function

\>plot2d(&diff(f(x),x),\>add,style="--",color=red); // derivative

\>labelbox(["f","f'"],["-","--"],[black,red]): // label box


![images/Final%20Projek%20APLIKOM-248.png](images/Final%20Projek%20APLIKOM-248.png)

\>plot2d(["exp(x)","1+x"],color=[black,blue],style=["-","-.-"]):


![images/Final%20Projek%20APLIKOM-249.png](images/Final%20Projek%20APLIKOM-249.png)

\>gridstyle("-\>",color=gray,textcolor=gray,framecolor=gray);  ...  
\>    plot2d("x^3-x",grid=1);   ...  
\>    settitle("y=x^3-x",color=black); ...  
\>    label("x",2,0,pos="bc",color=gray);  ...  
\>    label("y",0,6,pos="cl",color=gray); ...  
\>    reset():


![images/Final%20Projek%20APLIKOM-250.png](images/Final%20Projek%20APLIKOM-250.png)

Untuk kontrol yang lebih baik, sumbu x dan sumbu y dapat dilakukan
secara manual.


Perintah fullwindow() memperluas jendela plot karena kita tidak lagi
membutuhkan tempat untuk label di luar jendela plot. Gunakan
shrinkwindow() atau reset() untuk mengatur ulang ke default.


\>fullwindow; ...  
\>    gridstyle(color=darkgray,textcolor=darkgray); ...  
\>    plot2d(["2^x","1","2^(-x)"],a=-2,b=2,c=0,d=4,<grid,color=4:6,<frame); ...  
\>    xaxis(0,-2:1,style="-\>"); xaxis(0,2,"x",<axis); ...  
\>    yaxis(0,4,"y",style="-\>"); ...  
\>    yaxis(-2,1:4,\>left); ...  
\>    yaxis(2,2^(-2:2),style=".",<left); ...  
\>    labelbox(["2^x","1","2^-x"],colors=4:6,x=0.8,y=0.2); ...  
\>    reset:


![images/Final%20Projek%20APLIKOM-251.png](images/Final%20Projek%20APLIKOM-251.png)

Berikut adalah contoh lain, di mana string Unicode digunakan dan sumbu
di luar area plot.


\>aspect(1.5); 

\>plot2d(["sin(x)","cos(x)"],0,2pi,color=[red,green],<grid,<frame); ...  
\>    xaxis(-1.1,(0:2)\*pi,xt=["0",u"&pi;",u"2&pi;"],style="-",\>ticks,\>zero);  ...  
\>    xgrid((0:0.5:2)\*pi,<ticks); ...  
\>    yaxis(-0.1\*pi,-1:0.2:1,style="-",\>zero,\>grid); ...  
\>    labelbox(["sin","cos"],colors=[red,green],x=0.5,y=0.2,\>left); ...  
\>    xlabel(u"&phi;"); ylabel(u"f(&phi;)"):


![images/Final%20Projek%20APLIKOM-252.png](images/Final%20Projek%20APLIKOM-252.png)

# Memetok Data 2D

Jika x dan y adalah vektor data, data ini akan digunakan sebagai
koordinat x dan y dari kurva. Dalam hal ini, a, b, c, dan d, atau
jari-jari r dapat ditentukan, atau jendela plot akan menyesuaikan
secara otomatis dengan data. Atau, &gt; persegi dapat diatur untuk
mempertahankan rasio aspek persegi.


Memplot ekspresi hanyalah singkatan dari plot data. Untuk plot data,
Anda memerlukan satu atau lebih baris nilai-x, dan satu atau lebih
baris nilai-y. Dari rentang dan nilai-x, fungsi plot2d akan menghitung
data untuk diplot, secara default dengan evaluasi adaptif dari fungsi
tersebut. Untuk plot titik gunakan "&gt;titik", untuk garis campuran dan
titik gunakan "&gt;titik tambahan".


Tetapi Anda dapat memasukkan data secara langsung.


* 
Gunakan vektor baris untuk x dan y untuk satu fungsi.

* 
Matriks untuk x dan y diplot baris demi baris.


Berikut adalah contoh dengan satu baris untuk x dan y.


\>x=-10:0.1:10; y=exp(-x^2)\*x; plot2d(x,y):


![images/Final%20Projek%20APLIKOM-253.png](images/Final%20Projek%20APLIKOM-253.png)

Data juga dapat diplot sebagai titik. Gunakan points=true untuk ini.
Plotnya bekerja seperti poligon, tetapi hanya menggambar sudutnya.


* 
style="...": Pilih dari "[]", "&lt;&gt;", "o", ".", "..", "+", "*", "[]#",
* "&lt;&gt;#", "o#", ".. #", "#", "|".


Untuk memplot kumpulan titik, gunakan &gt;titik. Jika warna adalah vektor
warna, masing-masing menunjuk


mendapat warna yang berbeda. Untuk matriks koordinat dan vektor kolom,
warna berlaku untuk baris matriks.


Parameter &gt;addpoints menambahkan titik ke segmen garis untuk plot
data.


\>xdata=[1,1.5,2.5,3,4]; ydata=[3,3.1,2.8,2.9,2.7]; // data

\>plot2d(xdata,ydata,a=0.5,b=4.5,c=2.5,d=3.5,style="."); // lines

\>plot2d(xdata,ydata,\>points,\>add,style="o"): // add points


![images/Final%20Projek%20APLIKOM-254.png](images/Final%20Projek%20APLIKOM-254.png)

\>p=polyfit(xdata,ydata,1); // get regression line

\>plot2d("polyval(p,x)",\>add,color=red): // add plot of line


![images/Final%20Projek%20APLIKOM-255.png](images/Final%20Projek%20APLIKOM-255.png)

# Menggambar Daerah Yang Dibatasi Kurva

Plot data benar-benar poligon. Kita juga dapat memplot kurva atau
kurva yang diisi.


* 
filled=true mengisi plot.

* 
style="...": Pilih dari "#", "/", "", "/".

* 
fillcolor: Lihat di atas untuk warna yang tersedia.


Warna isian ditentukan oleh argumen "fillcolor", dan pada &lt;outline
opsional mencegah menggambar batas untuk semua gaya kecuali yang
default.


\>t=linspace(0,2pi,1000); // parameter for curve


Perintah ini menghasilkan vektor t yang berisi 1000 titik yang
terdistribusi secara merata dari 0 hingga 2pi


\>x=sin(t)\*exp(t/pi); y=cos(t)\*exp(t/pi); // x(t) and y(t)

\>figure(1,2); aspect(16/9)

\>figure(1); plot2d(x,y,r=10); // plot curve

\>figure(2); plot2d(x,y,r=10,\>filled,style="/",fillcolor=red); // fill curve

\>figure(0):


![images/Final%20Projek%20APLIKOM-256.png](images/Final%20Projek%20APLIKOM-256.png)

Dalam contoh berikut, kita memplot elips terisi dan dua segi enam
terisi menggunakan kurva tertutup dengan 6 titik dengan gaya isian
yang berbeda.


\>x=linspace(0,2pi,1000); plot2d(sin(x),cos(x)\*0.5,r=1,\>filled,style="/"):


![images/Final%20Projek%20APLIKOM-257.png](images/Final%20Projek%20APLIKOM-257.png)

\>t=linspace(0,2pi,6); ...  
\>   plot2d(cos(t),sin(t),\>filled,style="/",fillcolor=red,r=1.2):


![images/Final%20Projek%20APLIKOM-258.png](images/Final%20Projek%20APLIKOM-258.png)

\>t=linspace(0,2pi,6); plot2d(cos(t),sin(t),\>filled,style="#"):


![images/Final%20Projek%20APLIKOM-259.png](images/Final%20Projek%20APLIKOM-259.png)

Contoh lain adalah septagon, yang kami buat dengan 7 titik pada
lingkaran satuan.


\>t=linspace(0,2pi,7);  ...  
\>    plot2d(cos(t),sin(t),r=1,\>filled,style="/",fillcolor=red):


![images/Final%20Projek%20APLIKOM-260.png](images/Final%20Projek%20APLIKOM-260.png)

Berikut ini adalah himpunan nilai maksimal dari empat kondisi linier
kurang dari atau sama dengan 3. Ini adalah A[k].v&lt;=3 untuk semua baris
A. Untuk mendapatkan sudut yang bagus, kami menggunakan n yang relatif
besar.


\>A=[2,1;1,2;-1,0;0,-1];

\>function f(x,y) := max([x,y].A');

\>plot2d("f",r=4,level=[0;3],color=green,n=111):


![images/Final%20Projek%20APLIKOM-261.png](images/Final%20Projek%20APLIKOM-261.png)

Poin utama dari bahasa matriks adalah memungkinkan untuk menghasilkan
tabel fungsi dengan mudah.


\>t=linspace(0,2pi,1000); x=cos(3\*t); y=sin(4\*t);


Kita sekarang memiliki vektor x dan y dari nilai. plot2d() dapat
memplot nilai-nilai ini


sebagai kurva yang menghubungkan titik-titik. Plot bisa diisi. Dalam
hal ini


Ini menghasilkan hasil yang bagus karena aturan penggulitan, yang
digunakan untuk


isi.


\>plot2d(x,y,<grid,<frame,\>filled):


![images/Final%20Projek%20APLIKOM-262.png](images/Final%20Projek%20APLIKOM-262.png)

Vektor interval diplot terhadap nilai x sebagai wilayah yang diisi


antara nilai interval yang lebih rendah dan atas.


Ini dapat berguna untuk memplot kesalahan perhitungan. Tapi itu bisa


juga digunakan untuk memplot kesalahan statistik.


\>t=0:0.1:1; ...  
\>    plot2d(t,interval(t-random(size(t)),t+random(size(t))),style="|");  ...  
\>    plot2d(t,t,add=true):


![images/Final%20Projek%20APLIKOM-263.png](images/Final%20Projek%20APLIKOM-263.png)

Jika x adalah vektor yang diurutkan, dan y adalah vektor interval,
maka plot2d akan memplot rentang interval yang terisi dalam bidang.
Gaya isian sama dengan gaya poligon.


\>t=-1:0.01:1; x=~t-0.01,t+0.01~; y=x^3-x;

\>plot2d(t,y):


![images/Final%20Projek%20APLIKOM-264.png](images/Final%20Projek%20APLIKOM-264.png)

Dimungkinkan untuk mengisi wilayah nilai untuk fungsi tertentu. Bagi


ini, level harus matriks 2xn. Baris pertama adalah batas bawah


dan baris kedua berisi batas atas.


\>expr := "2\*x^2+x\*y+3\*y^4+y"; // define an expression f(x,y)

\>plot2d(expr,level=[0;1],style="-",color=blue): // 0 <= f(x,y) <= 1


![images/Final%20Projek%20APLIKOM-265.png](images/Final%20Projek%20APLIKOM-265.png)



We can also fill ranges of values like


\>plot2d("(x^2+y^2)^2-x^2+y^2",r=1.2,level=[-1;0],style="/"):


![images/Final%20Projek%20APLIKOM-266.png](images/Final%20Projek%20APLIKOM-266.png)

\>plot2d("cos(x)","sin(x)^3",xmin=0,xmax=2pi,\>filled,style="/"):


![images/Final%20Projek%20APLIKOM-267.png](images/Final%20Projek%20APLIKOM-267.png)

# Grafik Fungsi Parametrik

Nilai x tidak perlu diurutkan. (x,y) hanya menggambarkan kurva. Jika x
diurutkan, kurva adalah grafik dari suatu fungsi.


Dalam contoh berikut, kita memplot spiral


lateks: gamma(t) = t cdot (cos(2pi t),sin(2pi t))


Kita perlu menggunakan sangat banyak titik untuk tampilan yang halus
atau fungsi adaptive() untuk mengevaluasi ekspresi (lihat fungsi
adaptive() untuk lebih jelasnya).


\>t=linspace(0,1,1000); ...  
\>   plot2d(t\*cos(2\*pi\*t),t\*sin(2\*pi\*t),r=1):


![images/Final%20Projek%20APLIKOM-268.png](images/Final%20Projek%20APLIKOM-268.png)

Atau, dimungkinkan untuk menggunakan dua ekspresi untuk kurva. Berikut
ini memplot kurva yang sama seperti di atas.


\>plot2d("x\*cos(2\*pi\*x)","x\*sin(2\*pi\*x)",xmin=0,xmax=1,r=1):


![images/Final%20Projek%20APLIKOM-269.png](images/Final%20Projek%20APLIKOM-269.png)

\>t=linspace(0,1,1000); r=exp(-t); x=r\*cos(2pi\*t); y=r\*sin(2pi\*t);

\>plot2d(x,y,r=1):


![images/Final%20Projek%20APLIKOM-270.png](images/Final%20Projek%20APLIKOM-270.png)

Pada contoh berikutnya, kita memplot kurva


dengan


\>t=linspace(0,2pi,1000); r=1+sin(3\*t)/2; x=r\*cos(t); y=r\*sin(t); ...  
\>   plot2d(x,y,\>filled,fillcolor=red,style="/",r=1.5):


![images/Final%20Projek%20APLIKOM-271.png](images/Final%20Projek%20APLIKOM-271.png)

# Menggambar Grafik Bilangan Kompleks

Array bilangan kompleks juga dapat diplot. Kemudian titik jaringan
akan terhubung. Jika sejumlah garis kisi ditentukan (atau vektor garis
kisi 1x2) dalam argumen cgrid hanya garis kisi yang terlihat.


Matriks bilangan kompleks akan secara otomatis diplot sebagai kisi
dalam bidang kompleks.


Dalam contoh berikut, kita memplot gambar lingkaran satuan di bawah
fungsi eksponensial. Parameter cgrid menyembunyikan beberapa kurva
grid.


\>aspect(); r=linspace(0,1,50); a=linspace(0,2pi,80)'; z=r\*exp(I\*a);...  
\>   plot2d(z,a=-1.25,b=1.25,c=-1.25,d=1.25,cgrid=10):


![images/Final%20Projek%20APLIKOM-272.png](images/Final%20Projek%20APLIKOM-272.png)

\>aspect(1.25); r=linspace(0,1,50); a=linspace(0,2pi,200)'; z=r\*exp(I\*a);

\>plot2d(exp(z),cgrid=[40,10]):


![images/Final%20Projek%20APLIKOM-273.png](images/Final%20Projek%20APLIKOM-273.png)

\>r=linspace(0,1,10); a=linspace(0,2pi,40)'; z=r\*exp(I\*a);

\>plot2d(exp(z),\>points,\>add):


![images/Final%20Projek%20APLIKOM-274.png](images/Final%20Projek%20APLIKOM-274.png)

Vektor bilangan kompleks secara otomatis diplot sebagai kurva dalam
bidang kompleks dengan bagian real dan bagian imajiner.


Dalam contoh, kita memplot lingkaran satuan dengan


\>t=linspace(0,2pi,1000); ...  
\>   plot2d(exp(I\*t)+exp(4\*I\*t),r=2):


![images/Final%20Projek%20APLIKOM-275.png](images/Final%20Projek%20APLIKOM-275.png)

# Plot Statistik

Ada banyak fungsi yang mengkhususkan diri pada plot statistik. Salah
satu plot yang sering digunakan adalah plot kolom.


Jumlah kumulatif dari nilai terdistribusi 0-1-normal menghasilkan
jalan acak.


\>plot2d(cumsum(randnormal(1,1000))):


![images/Final%20Projek%20APLIKOM-276.png](images/Final%20Projek%20APLIKOM-276.png)

Menggunakan dua baris menunjukkan jalan dalam dua dimensi.


\>X=cumsum(randnormal(2,1000)); plot2d(X[1],X[2]):


![images/Final%20Projek%20APLIKOM-277.png](images/Final%20Projek%20APLIKOM-277.png)

\>columnsplot(cumsum(random(10)),style="/",color=blue):


![images/Final%20Projek%20APLIKOM-278.png](images/Final%20Projek%20APLIKOM-278.png)

Ini juga dapat menampilkan string sebagai label.


\>months=["Jan","Feb","Mar","Apr","May","Jun", ...  
\>     "Jul","Aug","Sep","Oct","Nov","Dec"];

\>values=[10,12,12,18,22,28,30,26,22,18,12,8];

\>columnsplot(values,lab=months,color=red,style="-");

\>title("Temperature"):


![images/Final%20Projek%20APLIKOM-279.png](images/Final%20Projek%20APLIKOM-279.png)

\>k=0:10;

\>plot2d(k,bin(10,k),\>bar):


![images/Final%20Projek%20APLIKOM-280.png](images/Final%20Projek%20APLIKOM-280.png)

\>plot2d(k,bin(10,k)); plot2d(k,bin(10,k),\>points,\>add):


![images/Final%20Projek%20APLIKOM-281.png](images/Final%20Projek%20APLIKOM-281.png)

\>plot2d(normal(1000),normal(1000),\>points,grid=6,style=".."):


![images/Final%20Projek%20APLIKOM-282.png](images/Final%20Projek%20APLIKOM-282.png)

\>plot2d(normal(1,1000),\>distribution,style="O"):


![images/Final%20Projek%20APLIKOM-283.png](images/Final%20Projek%20APLIKOM-283.png)

\>plot2d("qnormal",0,5;2.5,0.5,\>filled):


![images/Final%20Projek%20APLIKOM-284.png](images/Final%20Projek%20APLIKOM-284.png)

Untuk memplot distribusi statistik eksperimental, Anda dapat
menggunakan distribution=n dengan plot2d.


\>w=randexponential(1,1000); // exponential distribution

\>plot2d(w,\>distribution): // or distribution=n with n intervals


![images/Final%20Projek%20APLIKOM-285.png](images/Final%20Projek%20APLIKOM-285.png)

Atau Anda dapat menghitung distribusi dari data dan memplot hasilnya
dengan &gt;bar di plot3d, atau dengan plot kolom.


\>w=normal(1000); // 0-1-normal distribution

\>{x,y}=histo(w,10,v=[-6,-4,-2,-1,0,1,2,4,6]); // interval bounds v

\>plot2d(x,y,\>bar):


![images/Final%20Projek%20APLIKOM-286.png](images/Final%20Projek%20APLIKOM-286.png)

Fungsi statplot() mengatur gaya dengan string sederhana.


\>statplot(1:10,cumsum(random(10)),"b"):


![images/Final%20Projek%20APLIKOM-287.png](images/Final%20Projek%20APLIKOM-287.png)

\>n=10; i=0:n; ...  
\>   plot2d(i,bin(n,i)/2^n,a=0,b=10,c=0,d=0.3); ...  
\>   plot2d(i,bin(n,i)/2^n,points=true,style="ow",add=true,color=blue):


![images/Final%20Projek%20APLIKOM-288.png](images/Final%20Projek%20APLIKOM-288.png)

Selain itu, data dapat diplot sebagai batang. Dalam hal ini, x harus
diurutkan dan satu elemen lebih panjang dari y. Bilah akan memanjang
dari x[i] ke x[i+1] dengan nilai y[i]. Jika x memiliki ukuran yang
sama dengan y, itu akan diperpanjang oleh satu elemen dengan spasi
terakhir.


Gaya isian dapat digunakan seperti di atas.


\>n=10; k=bin(n,0:n); ...  
\>   plot2d(-0.5:n+0.5,k,bar=true,fillcolor=lightgray):


![images/Final%20Projek%20APLIKOM-289.png](images/Final%20Projek%20APLIKOM-289.png)

Data untuk plot batang (bar=1) dan histogram (histogram=1) dapat
diberikan secara eksplisit dalam xv dan yv, atau dapat dihitung dari
distribusi empiris dalam xv dengan &gt;distribusi (atau distribusi=n).
Histogram nilai xv akan dihitung secara otomatis dengan &gt;histogram.
Jika &gt;genap ditentukan, nilai xv akan dihitung dalam interval bilangan
bulat.


\>plot2d(normal(10000),distribution=50):


![images/Final%20Projek%20APLIKOM-290.png](images/Final%20Projek%20APLIKOM-290.png)

\>k=0:10; m=bin(10,k); x=(0:11)-0.5; plot2d(x,m,\>bar):


![images/Final%20Projek%20APLIKOM-291.png](images/Final%20Projek%20APLIKOM-291.png)

\>columnsplot(m,k):


![images/Final%20Projek%20APLIKOM-292.png](images/Final%20Projek%20APLIKOM-292.png)

\>plot2d(random(600)\*6,histogram=6):


![images/Final%20Projek%20APLIKOM-293.png](images/Final%20Projek%20APLIKOM-293.png)

Untuk distribusi, ada parameter distribution=n, yang menghitung nilai
secara otomatis dan mencetak distribusi relatif dengan n sub-interval.


\>plot2d(normal(1,1000),distribution=10,style="\\/"):


![images/Final%20Projek%20APLIKOM-294.png](images/Final%20Projek%20APLIKOM-294.png)

Dengan parameter even=true, ini akan menggunakan interval bilangan
bulat.


\>plot2d(intrandom(1,1000,10),distribution=10,even=true):


![images/Final%20Projek%20APLIKOM-295.png](images/Final%20Projek%20APLIKOM-295.png)

Perhatikan bahwa ada banyak plot statistik, yang mungkin berguna.
Lihatlah tutorial tentang statistik.


\>columnsplot(getmultiplicities(1:6,intrandom(1,6000,6))):


![images/Final%20Projek%20APLIKOM-296.png](images/Final%20Projek%20APLIKOM-296.png)

\>plot2d(normal(1,1000),\>distribution); ...  
\>     plot2d("qnormal(x)",color=red,thickness=2,\>add):


![images/Final%20Projek%20APLIKOM-297.png](images/Final%20Projek%20APLIKOM-297.png)

Ada juga banyak plot khusus untuk statistik. Boxplot menunjukkan
kuartil distribusi ini dan banyak outlier. Menurut definisi, outlier
dalam boxplot adalah data yang melebihi 1,5 kali rentang 50% tengah
plot.


\>M=normal(5,1000); boxplot(quartiles(M)):


![images/Final%20Projek%20APLIKOM-298.png](images/Final%20Projek%20APLIKOM-298.png)

# Fungsi Implisit

Plot implisit menunjukkan garis level yang menyelesaikan f(x,y)=level,
di mana "level" dapat berupa nilai tunggal atau vektor nilai. Jika
level="auto", akan ada garis level nc, yang akan menyebar antara
minimum dan maksimum fungsi secara merata. Warna yang lebih gelap atau
lebih terang dapat ditambahkan dengan &gt;hue untuk menunjukkan nilai
fungsi. Untuk fungsi implisit, xv harus berupa fungsi atau ekspresi
dari parameter x dan y, atau, sebagai alternatif, xv dapat berupa
matriks nilai.


Euler dapat menandai garis level


lateks: f(x,y) = c


dari fungsi apa pun.


Untuk menggambar himpunan f(x,y)=c untuk satu atau lebih konstanta c,
Anda dapat menggunakan plot2d() dengan plot implisitnya di bidang.
Parameter untuk c adalah level=c, di mana c dapat berupa vektor garis
level. Selain itu, skema warna dapat digambar di latar belakang untuk
menunjukkan nilai fungsi untuk setiap titik dalam plot. Parameter "n"
menentukan kehalusan plot.


\>aspect(1.5); 

\>plot2d("x^2+y^2-x\*y-x",r=1.5,level=0,contourcolor=red):


![images/Final%20Projek%20APLIKOM-299.png](images/Final%20Projek%20APLIKOM-299.png)

\>expr := "2\*x^2+x\*y+3\*y^4+y"; // define an expression f(x,y)

\>plot2d(expr,level=0): // Solutions of f(x,y)=0


![images/Final%20Projek%20APLIKOM-300.png](images/Final%20Projek%20APLIKOM-300.png)

\>plot2d(expr,level=0:0.5:20,\>hue,contourcolor=white,n=200): // nice


![images/Final%20Projek%20APLIKOM-301.png](images/Final%20Projek%20APLIKOM-301.png)

\>plot2d(expr,level=0:0.5:20,\>hue,\>spectral,n=200,grid=4): // nicer


![images/Final%20Projek%20APLIKOM-302.png](images/Final%20Projek%20APLIKOM-302.png)

Ini juga berfungsi untuk plot data. Tetapi Anda harus menentukan
rentang


untuk label sumbu.


\>x=-2:0.05:1; y=x'; z=expr(x,y);

\>plot2d(z,level=0,a=-1,b=2,c=-2,d=1,\>hue):


![images/Final%20Projek%20APLIKOM-303.png](images/Final%20Projek%20APLIKOM-303.png)

\>plot2d("x^3-y^2",\>contour,\>hue,\>spectral):


![images/Final%20Projek%20APLIKOM-304.png](images/Final%20Projek%20APLIKOM-304.png)

\>plot2d("x^3-y^2",level=0,contourwidth=3,\>add,contourcolor=red):


![images/Final%20Projek%20APLIKOM-305.png](images/Final%20Projek%20APLIKOM-305.png)

\>z=z+normal(size(z))\*0.2;

\>plot2d(z,level=0.5,a=-1,b=2,c=-2,d=1):


![images/Final%20Projek%20APLIKOM-306.png](images/Final%20Projek%20APLIKOM-306.png)

\>plot2d(expr,level=[0:0.2:5;0.05:0.2:5.05],color=lightgray):


![images/Final%20Projek%20APLIKOM-307.png](images/Final%20Projek%20APLIKOM-307.png)

\>plot2d("x^2+y^3+x\*y",level=1,r=4,n=100):


![images/Final%20Projek%20APLIKOM-308.png](images/Final%20Projek%20APLIKOM-308.png)

\>plot2d("x^2+2\*y^2-x\*y",level=0:0.1:10,n=100,contourcolor=white,\>hue):


![images/Final%20Projek%20APLIKOM-309.png](images/Final%20Projek%20APLIKOM-309.png)

Dimungkinkan juga untuk mengisi set




dengan rentang level.


Dimungkinkan untuk mengisi wilayah nilai untuk fungsi tertentu. Untuk
ini, level harus berupa matriks 2xn. Baris pertama adalah batas bawah
dan baris kedua berisi batas atas.


\>plot2d(expr,level=[0;1],style="-",color=blue): // 0 <= f(x,y) <= 1


![images/Final%20Projek%20APLIKOM-310.png](images/Final%20Projek%20APLIKOM-310.png)

Plot implisit juga dapat menunjukkan rentang level. Kemudian level
harus berupa matriks 2xn dari interval level, di mana baris pertama
berisi awal dan baris kedua akhir dari setiap interval. Atau, vektor
baris sederhana dapat digunakan untuk level, dan parameter dl
memperluas nilai level ke interval.


\>plot2d("x^4+y^4",r=1.5,level=[0;1],color=blue,style="/"):


![images/Final%20Projek%20APLIKOM-311.png](images/Final%20Projek%20APLIKOM-311.png)

\>plot2d("x^2+y^3+x\*y",level=[0,2,4;1,3,5],style="/",r=2,n=100):


![images/Final%20Projek%20APLIKOM-312.png](images/Final%20Projek%20APLIKOM-312.png)

\>plot2d("x^2+y^3+x\*y",level=-10:20,r=2,style="-",dl=0.1,n=100):


![images/Final%20Projek%20APLIKOM-313.png](images/Final%20Projek%20APLIKOM-313.png)

\>plot2d("sin(x)\*cos(y)",r=pi,\>hue,\>levels,n=100):


![images/Final%20Projek%20APLIKOM-314.png](images/Final%20Projek%20APLIKOM-314.png)

Dimungkinkan juga untuk menandai suatu wilayah


Ini dilakukan dengan menambahkan level dengan dua baris.


\>plot2d("(x^2+y^2-1)^3-x^2\*y^3",r=1.3, ...  
\>     style="#",color=red,<outline, ...  
\>     level=[-2;0],n=100):


![images/Final%20Projek%20APLIKOM-315.png](images/Final%20Projek%20APLIKOM-315.png)

Dimungkinkan untuk menentukan tingkat tertentu. Misalnya, kita dapat
memplot solusi dari persamaan seperti


\>plot2d("x^3-x\*y+x^2\*y^2",r=6,level=1,n=100):


![images/Final%20Projek%20APLIKOM-316.png](images/Final%20Projek%20APLIKOM-316.png)

\>function starplot1 (v, style="/", color=green, lab=none) ...


      if !holding() then clg; endif;
      w=window(); window(0,0,1024,1024);
      h=holding(1);
      r=max(abs(v))*1.2;
      setplot(-r,r,-r,r);
      n=cols(v); t=linspace(0,2pi,n);
      v=v|v[1]; c=v*cos(t); s=v*sin(t);
      cl=barcolor(color); st=barstyle(style);
      loop 1 to n
        polygon([0,c[#],c[#+1]],[0,s[#],s[#+1]],1);
        if lab!=none then
          rlab=v[#]+r*0.1;
          {col,row}=toscreen(cos(t[#])*rlab,sin(t[#])*rlab);
          ctext(""+lab[#],col,row-textheight()/2);
        endif;
      end;
      barcolor(cl); barstyle(st);
      holding(h);
      window(w);
    endfunction
</pre>
Tidak ada kutu kisi atau sumbu di sini. Selain itu, kami menggunakan
jendela penuh untuk plot.


Kami memanggil reset sebelum kami menguji plot ini untuk mengembalikan
default grafis. Ini tidak perlu, jika Anda yakin bahwa plot Anda
berhasil.


\>reset; starplot1(normal(1,10)+5,color=red,lab=1:10):


![images/Final%20Projek%20APLIKOM-317.png](images/Final%20Projek%20APLIKOM-317.png)

Terkadang, Anda mungkin ingin merencanakan sesuatu yang tidak dapat
dilakukan plot2d, tetapi hampir.


Dalam fungsi berikut, kita melakukan plot impuls logaritma. Plot2d
dapat melakukan plot logaritma, tetapi tidak untuk bilah impuls.


\>function logimpulseplot1 (x,y) ...


      {x0,y0}=makeimpulse(x,log(y)/log(10));
      plot2d(x0,y0,>bar,grid=0);
      h=holding(1);
      frame();
      xgrid(ticks(x));
      p=plot();
      for i=-10 to 10;
        if i<=p[4] and i>=p[3] then
           ygrid(i,yt="10^"+i);
        endif;
      end;
      holding(h);
    endfunction
</pre>
Mari kita ujinya dengan nilai yang didistribusikan secara
eksponensial.


\>aspect(1.5); x=1:10; y=-log(random(size(x)))\*200; ...  
\>   logimpulseplot1(x,y):


![images/Final%20Projek%20APLIKOM-318.png](images/Final%20Projek%20APLIKOM-318.png)

Mari kita animasikan kurva 2D menggunakan plot langsung. Perintah
plot(x,y) hanya memplot kurva ke jendela plot. setplot(a,b,c,d)
mengatur jendela ini.


Fungsi wait(0) memaksa plot muncul di jendela grafis. Jika tidak,
penggambaran ulang terjadi dalam interval waktu yang jarang.


\>function animliss (n,m) ...


    t=linspace(0,2pi,500);
    f=0;
    c=framecolor(0);
    l=linewidth(2);
    setplot(-1,1,-1,1);
    repeat
      clg;
      plot(sin(n*t),cos(m*t+f));
      wait(0);
      if testkey() then break; endif;
      f=f+0.02;
    end;
    framecolor(c);
    linewidth(l);
    endfunction
</pre>
Tekan tombol apa saja untuk menghentikan animasi ini.


\>animliss(2,3); // lihat hasilnya, jika sudah puas, tekan ENTER


# Plot Logaritma

EMT menggunakan parameter "logplot" untuk skala logaritma.


Plot logaritma dapat diplot baik menggunakan skala logaritma di y
dengan logplot=1, atau menggunakan skala logaritma di x dan y dengan
logplot=2, atau di x dengan logplot=3.


* 
logplot=1: logaritma y

* 
logplot=2: x-y-logaritma

* 
logplot=3: x-logaritma


\>plot2d("exp(x^3-x)\*x^2",1,5,logplot=1):


![images/Final%20Projek%20APLIKOM-319.png](images/Final%20Projek%20APLIKOM-319.png)

\>plot2d("exp(x+sin(x))",0,100,logplot=1):


![images/Final%20Projek%20APLIKOM-320.png](images/Final%20Projek%20APLIKOM-320.png)

\>plot2d("exp(x+sin(x))",10,100,logplot=2):


![images/Final%20Projek%20APLIKOM-321.png](images/Final%20Projek%20APLIKOM-321.png)

\>plot2d("gamma(x)",1,10,logplot=1):


![images/Final%20Projek%20APLIKOM-322.png](images/Final%20Projek%20APLIKOM-322.png)

\>plot2d("log(x\*(2+sin(x/100)))",10,1000,logplot=3):


![images/Final%20Projek%20APLIKOM-323.png](images/Final%20Projek%20APLIKOM-323.png)

Ini juga berfungsi dengan plot data.


\>x=10^(1:20); y=x^2-x;

\>plot2d(x,y,logplot=2):


![images/Final%20Projek%20APLIKOM-324.png](images/Final%20Projek%20APLIKOM-324.png)

\>function f(x):= (1/3)x^3-x^2-3\*x+4

\>plot2d("f",-4,5):


![images/Final%20Projek%20APLIKOM-325.png](images/Final%20Projek%20APLIKOM-325.png)

# Contoh lain dan soal:

\>plot2d("x^7+y^9+x\*y",level=1,r=5,n=200):


![images/Final%20Projek%20APLIKOM-326.png](images/Final%20Projek%20APLIKOM-326.png)

\>plot2d(normal(1,1000),\>distribution); ...  
\>     plot2d("qnormal(x)",color=black,thickness=7,\>add):


![images/Final%20Projek%20APLIKOM-327.png](images/Final%20Projek%20APLIKOM-327.png)

\>plot2d("x^3-y^9",\>contour,\>hue,\>spectral):


![images/Final%20Projek%20APLIKOM-328.png](images/Final%20Projek%20APLIKOM-328.png)

\>reset;...  
\>  
Buatlah kurva dengan k dari 1 sampai 10, dengan fungsi


\>figure(5,2);...  
\>   for k=1:10; figure(k); plot2d("x^5-3x",-3,2,grid=k); end;...  
\>   figure(0):


![images/Final%20Projek%20APLIKOM-329.png](images/Final%20Projek%20APLIKOM-329.png)

Gambar plot fungsi berikut:


Penyelesaian:


\>reset;...  
\>   figure(2,2);...  
\>   for n=1 to 5; figure(n); plot2d("x^1"+n); end;... 

\>figure(0):


![images/Final%20Projek%20APLIKOM-330.png](images/Final%20Projek%20APLIKOM-330.png)

Gambarkan grafik fungsi berikut:


\>reset;...  
\>   aspect(3,1);...  
\>   figure(1,3); figure(1); plot2d("x^5+x+4", grid=2);...  
\>   figure(2); plot2d("4x^2x^2+4", grid=5);...  
\>   figure(3); plot2d("x^2+9x", grid=4);...  
\>   figure(0):


![images/Final%20Projek%20APLIKOM-331.png](images/Final%20Projek%20APLIKOM-331.png)

\>plot2d("x^3+y^3",r=1.5,level=[0;1],color=blue,style="/"):


![images/Final%20Projek%20APLIKOM-332.png](images/Final%20Projek%20APLIKOM-332.png)

\>plot2d("(x^3+y^3-2)^3-x^2\*y^3",r=1.3, ...  
\>     style="#",color=red,<outline, ...  
\>     level=[-2;0],n=100):


![images/Final%20Projek%20APLIKOM-333.png](images/Final%20Projek%20APLIKOM-333.png)

\>plot2d("sin(x)\*cos(y)",r=2pi,\>hue,\>levels,n=100):


![images/Final%20Projek%20APLIKOM-334.png](images/Final%20Projek%20APLIKOM-334.png)

\>plot2d("x^3+2\*y^3-x\*y",level=0:0.1:10,n=100,contourcolor=white,\>hue):


![images/Final%20Projek%20APLIKOM-335.png](images/Final%20Projek%20APLIKOM-335.png)

\>plot2d(normal(1,1000),\>distribution); ...  
\>     plot2d("qnormal(x)",color=red,thickness=3,\>add):


![images/Final%20Projek%20APLIKOM-336.png](images/Final%20Projek%20APLIKOM-336.png)

\>M=normal(5,1000); boxplot(quartiles(M)):


![images/Final%20Projek%20APLIKOM-337.png](images/Final%20Projek%20APLIKOM-337.png)

\>plot2d(random(500)\*5,histogram=5):


![images/Final%20Projek%20APLIKOM-338.png](images/Final%20Projek%20APLIKOM-338.png)

# Menggambar Plot 3D dengan EMT

Ini adalah pengenalan plot 3D di Euler. Kita membutuhkan plot 3D untuk
memvisualisasikan fungsi dari dua variabel.


Euler menggambar fungsi tersebut menggunakan algoritma pengurutan
untuk menyembunyikan bagian di latar belakang. Secara umum, Euler
menggunakan proyeksi pusat. Standarnya adalah dari kuadran x-y positif
menuju titik asal x=y=z=0, tetapi sudut=0° terlihat dari arah sumbu y.
Sudut pandang dan tinggi dapat diubah.


Euler dapat merencanakan


* 
permukaan dengan bayangan dan garis level atau rentang level,

* 
awan poin,

* 
kurva parametrik,

* 
permukaan implisit.


Plot 3D dari suatu fungsi menggunakan plot3d. Cara termudah adalah
dengan memplot ekspresi dalam x dan y. Parameter r mengatur kisaran
plot di sekitar (0,0).


\>aspect(1.5); plot3d("x^2+sin(y)",r=2\*pi): 


![images/Final%20Projek%20APLIKOM-339.png](images/Final%20Projek%20APLIKOM-339.png)

## 1) Menggambar Grafik Fungsi Dua Variabel dalam Bentuk

## Ekspresi Langsung

Grafik fungsi dua variabel dalam bentuk ekspresi langsung adalah
representasi visual dari hubungan matematis antara dua variabel
independen yang dinyatakan dalam bentuk persamaan atau ekspresi
matematis. Biasanya, grafik ini digunakan untuk menggambarkan hubungan
antara dua variabel dalam bidang dua dimensi dan tiga dimensi. Dalam
konteks ini, variabel independen (x dan y) adalah variabel input,
sedangkan variabel dependen (z) adalah variabel output yang dihasilkan
oleh ekspresi matematis.


Rumus umum untuk menggambar grafik fungsi dua variabel dalam bentuk
ekspresi langsung adalah:


$$z = f(x, y)$$Dalam rumus ini:


- z adalah variabel dependen yang ingin kita gambar dalam grafik.


- f(x, y) adalah ekspresi matematis yang menghubungkan variabel z
dengan variabel independen x dan y. Ekspresi ini dapat berupa fungsi
linear, fungsi kuadrat, fungsi akar kuadrat, eksponensial, logaritma,
trigonometri, nilai mutlak, atau jenis fungsi matematis lainnya,
tergantung pada hubungan yang ingin diilustrasikan.


## 1. Grafik Fungsi Linear



Fungsi linear dua variabel biasanya dinyatakan dalam bentuk


$$f(x,y)=ax+by+c$$

dimana a,b, dan c adalah konstanta.  Grafik fungsi linear ini adalah
sebuah bidang datar, dan bentuknya akan bervariasi tergantung pada
nilai a dan b.


Contoh:


$$f(x,y)=7x+3y+9$$\>plot3d("7\*x+3\*y+9"):


![images/Final%20Projek%20APLIKOM-343.png](images/Final%20Projek%20APLIKOM-343.png)

$$f(x,y)=-9x-3y-12$$\>plot3d("-9\*x-3\*y-12"):


![images/Final%20Projek%20APLIKOM-345.png](images/Final%20Projek%20APLIKOM-345.png)

## 2. Grafik Fungsi Kuadrat



Fungsi kuadrat dua variabel biasanya dinyatakan dalam bentuk


$$f(x,y)=ax^2+by^2+cxy+dx+ey+f$$

dimana a, b, c, d, e, dan f adalah konstanta. Grafik fungsi kuadrat
ini adalah sebuah permukaan yang dapat memiliki berbagai bentuk
tergantung pada nilai-nilai konstantanya.


Contoh:


$$f(x,y)= 4x^2+y^2+4xy+8x+3y+12$$\>plot3d("4\*x^2+y^2+4\*x\*y+8\*x+3\*y+12"):


![images/Final%20Projek%20APLIKOM-348.png](images/Final%20Projek%20APLIKOM-348.png)

## 3. Grafik Fungsi Akar Kuadrat



Grafik fungsi akar kuadrat dua variabel


$$f(x,y)=\sqrt{x^2+y^2}$$

adalah grafik permukaan yang menggambarkan jarak titik (x, y) dari
titik asal (0, 0) dalam ruang tiga dimensi.


Contoh:


$$f(x,y)=\sqrt{x^2+y^2}$$\>plot3d("sqrt(x^2+y^2)"):


![images/Final%20Projek%20APLIKOM-351.png](images/Final%20Projek%20APLIKOM-351.png)

$$f(x,y)=\sqrt{6x^2+9y^2}$$\>plot3d("sqrt(36\*x^2+9\*y^2)"):


![images/Final%20Projek%20APLIKOM-353.png](images/Final%20Projek%20APLIKOM-353.png)

## 4. Grafik Fungsi Eksponensial



Fungsi eksponensial dua variabel bisa dinyatakan


$$f(x,y)=a.b^{xy}$$

dimana a dan b adalah konstanta, x dan y adalah variabel. Fungsi ini
menggambarkan pertumbuhan eksponensial yang bergantung pada nilai x
dan y.


Contoh:


$$f(x,y)= 12.3^{xy}$$\>plot3d("12\*3^(x\*y)"):


![images/Final%20Projek%20APLIKOM-356.png](images/Final%20Projek%20APLIKOM-356.png)

$$f(x,y)= 5.-8^{xy}$$\>plot3d("5\*-8^(x\*y)"):


![images/Final%20Projek%20APLIKOM-358.png](images/Final%20Projek%20APLIKOM-358.png)

## 5. Grafik Fungsi Logaritma



Grafik fungsi logaritma dua variabel adalah grafik yang menggambarkan
nilai logaritma dari suatu ekspresi yang melibatkan dua variabel
(biasanya x dan y). Fungsi logaritma dua variabel ini dinyatakan
sebagai


$$f(x,y)=log_b(xy)$$

dimana b adalah basis logaritma. Basis logaritma ini dapat
berbeda-beda.


Contoh:


$$f(x,y)=log(xy), basis 10$$\>plot3d("log(x\*y)"):


![images/Final%20Projek%20APLIKOM-361.png](images/Final%20Projek%20APLIKOM-361.png)

$$f(x,y)=log(4x.9y), basis 10$$\>plot3d("log(4x\*9\*y)"):


![images/Final%20Projek%20APLIKOM-363.png](images/Final%20Projek%20APLIKOM-363.png)

## 6. Grafik Fungsi Trigonometri



Fungsi trigonometri dua variabel adalah fungsi matematika yang
melibatkan operasi trigonometri (seperti sin, cos, tan) pada kedua
variabel x dan y.


Contoh:


$$f(x,y)=sin(45x).cos(y)$$\>plot3d("sin(45x)\*cos(y)"):


![images/Final%20Projek%20APLIKOM-365.png](images/Final%20Projek%20APLIKOM-365.png)

$$f(x,y)=sin(2x).cos(4y)$$\>plot3d("sin(2x)\*cos(4y)"):


![images/Final%20Projek%20APLIKOM-367.png](images/Final%20Projek%20APLIKOM-367.png)

$$f(x,y)=sin(15x).tan(60y)$$\>plot3d("sin(15x)\*tan(60y)"):


![images/Final%20Projek%20APLIKOM-369.png](images/Final%20Projek%20APLIKOM-369.png)

$$f(x,y)=cos(x).tan(2y)$$\>plot3d("cos(x)\*tan(2y)"):


![images/Final%20Projek%20APLIKOM-371.png](images/Final%20Projek%20APLIKOM-371.png)

$$f(x,y)=cosec(6x).sec(2y)$$\>plot3d("cosec(6x)\*sec(2y)"):


![images/Final%20Projek%20APLIKOM-373.png](images/Final%20Projek%20APLIKOM-373.png)

## 7. Grafik Fungsi Nilai Mutlak



Fungsi nilai mutlak dua variabel, juga dikenal sebagai fungsi modul
dua variabel, dinyatakan sebagai


$$f(x,y)=|g(x,y)|$$

dimana g(x,y) adalah fungsi dua variabel.


Contoh:


$$f(x,y)=|x^2 - y^2|$$\>plot3d("abs(x^2 - y^2)"):


![images/Final%20Projek%20APLIKOM-376.png](images/Final%20Projek%20APLIKOM-376.png)

$$f(x,y)=|5x^2 + 3y^2|$$\>plot3d("abs(5\*x^2 + 3\*y^2)"):


![images/Final%20Projek%20APLIKOM-378.png](images/Final%20Projek%20APLIKOM-378.png)

$$f(x,y)=|-2x^2 - 5y^2|$$\>plot3d("abs(-2x^2 - 5y^2)"):


![images/Final%20Projek%20APLIKOM-380.png](images/Final%20Projek%20APLIKOM-380.png)

## Latihan soal



Buatkan grafik dari fungsi berikut:


1.


$$f(x,y)=16x-4y+6$$\>plot3d("16\*x - 4\*y +6"):


![images/Final%20Projek%20APLIKOM-382.png](images/Final%20Projek%20APLIKOM-382.png)

2.


$$f(x,y)=cos(45x).sin(15y)$$\>plot3d("cos(45\*x)\*sin(15\*y)"):


![images/Final%20Projek%20APLIKOM-384.png](images/Final%20Projek%20APLIKOM-384.png)

3.


$$f(x,y)=\sqrt{x^2+20y^2}$$\>plot3d("sqrt(x^2+20\*y^2)"):


![images/Final%20Projek%20APLIKOM-386.png](images/Final%20Projek%20APLIKOM-386.png)

## 2) Menggambar Grafik Fungsi Dua Variabel yang Rumusnya Disimpan

## dalam Variabel Ekspresi

## Apa yang dimaksud dengan Grafik Fungsi Dua Variabel?

Grafik fungsi dua variabel adalah representasi visual dari hubungan
antara sebuah fungsi matematika dengan dua variabel independen
(biasanya disebut sebagai "x" dan "y") dan variabel dependen (biasanya
disebut sebagai "z" atau "f(x, y)").


Dalam grafik ini, sumbu x dan sumbu y digunakan untuk menggambarkan
nilai-nilai dua variabel independen, sementara permukaan atau grafik
3D digunakan untuk menggambarkan nilai-nilai variabel dependen yang
dihasilkan oleh fungsi tersebut.


Grafik fungsi dua variabel membantu memvisualisasikan bagaimana nilai
variabel dependen (z) berubah seiring perubahan kedua variabel
independen (x dan y) sesuai dengan aturan fungsi tersebut.


## Fungsi matematika yg terlibat dalam Menggambar Grafik

## Fungsi Dua Variabel

1. Fungsi Linear


Bentuk umum :


$$f(x, y) = ax + by + c$$

di mana a, b, dan c adalah konstanta. Grafiknya adalah bidang datar.


2. Fungsi Kuadratik


Bentuk umum :


$$f(x, y) = ax^2 + by^2 + cxy + dx + ey + f.$$

Grafiknya dapat berupa permukaan yang berbentuk paraboloid, baik
terbuka ke atas atau ke bawah.


3.Fungsi Trigonometri


Bentuk umum sinus dan cosinus :


$$(x, y) = sin(x) + cos(y)$$

akan menghasilkan permukaan yang berulang-ulang naik dan turun.


4.Fungsi Pecahan


Bentuk umum :


$$f(x, y) = g(x, y) / h(x, y)$$

di mana g(x, y) dan h(x, y) adalah fungsi-fungsi lain.


grafiknya dapat menghasilkan berbagai pola yang tergantung pada sifat
fungsi g dan h.


## Menggambar Grafik Fungsi



Perintah yang digunakan untuk menggambar grafik fungsi dalam EMT yaitu
dengan menggunakan plot3d.


Untuk menampilkan grafik, akhiri perintah plot3d dengan tanda (:).


Tanda (:) akan menampilkan grafik di layar yang berbeda.


\>plot3d("6\*x^2+3\*y^2"):


![images/Final%20Projek%20APLIKOM-391.png](images/Final%20Projek%20APLIKOM-391.png)

\>plot3d("6\*x^2+3\*x\*sin(y)",-5,5,0,6\*pi):


![images/Final%20Projek%20APLIKOM-392.png](images/Final%20Projek%20APLIKOM-392.png)

## Menyimpan Variabel Ekspresi



Untuk menyimpan sebuah fungsi, dapat dilakukan dengan menggunakan
perintah function. Lalu, ketika ingin memanggil atau membuat grafik
dari fungsi tersebut, cukup dengan memanggil nama fungsi tersebut.


\>function a(x,y):= x^2+y^3

\>plot3d("a"):


![images/Final%20Projek%20APLIKOM-393.png](images/Final%20Projek%20APLIKOM-393.png)

\>function f(x,y):= x^3-y^2

\>plot3d("f"):


![images/Final%20Projek%20APLIKOM-394.png](images/Final%20Projek%20APLIKOM-394.png)

## Contoh Latihan Soal

$$f(x,y)= 14x^3+y^4$$\>function f(x,y):= 14\*x^3+y^4

\>plot3d("f"):


![images/Final%20Projek%20APLIKOM-396.png](images/Final%20Projek%20APLIKOM-396.png)

\>plot3d("a",\>user, ...  
\>   title="Turn with the vector keys (press return to finish)"):


![images/Final%20Projek%20APLIKOM-397.png](images/Final%20Projek%20APLIKOM-397.png)

Perintah ini mengizinkan pengguna untuk menggambar grafik 3D dari
fungsi yang mereka masukkan sendiri, serta memberikan petunjuk
interaktif tentang cara berinteraksi dengan grafik. Pengguna dapat
memutar tampilan grafik menggunakan tombol arah pada keyboard, dan
menekan "return" untuk menyelesaikan interaksi.


\>plot3d("a",r=5,n=80,fscale=4,scale=1.2,frame=3):


![images/Final%20Projek%20APLIKOM-398.png](images/Final%20Projek%20APLIKOM-398.png)

perintah ini akan menggambar grafik tiga dimensi dari fungsi "a" dalam
rentang x dan y dari -5 hingga 5, dengan 80 titik untuk detail yang
lebih halus. Nilai fungsi akan diperbesar 4 kali, dan grafik akan
ditampilkan dengan skala 1.2 untuk tampilan yang lebih jelas. Bingkai
grafis akan ditentukan oleh parameter frame=3.


\>view


    [5,  2.6,  2,  0.4]

\>plot3d("a",distance=3,zoom=2,angle=0,height=0):


![images/Final%20Projek%20APLIKOM-399.png](images/Final%20Projek%20APLIKOM-399.png)

\>plot3d("x^4+y^2",a=0,b=1,c=-1,d=1,angle=-20°,height=20°, ...  
\>   center=[0.4,0,0],zoom=5):


![images/Final%20Projek%20APLIKOM-400.png](images/Final%20Projek%20APLIKOM-400.png)

\>plot3d("a",r=2,<fscale,<scale,distance=13,height=50°, ...  
\>    center=[0,0,-2],frame=3):


![images/Final%20Projek%20APLIKOM-401.png](images/Final%20Projek%20APLIKOM-401.png)

\>plot3d("a",r=5,\>polar, ...  
\>   fscale=2,\>hue,n=100,zoom=4,\>contour,color=orange):


![images/Final%20Projek%20APLIKOM-402.png](images/Final%20Projek%20APLIKOM-402.png)

\>plot3d("x","a","y",r=2,zoom=3.5,frame=3):


![images/Final%20Projek%20APLIKOM-403.png](images/Final%20Projek%20APLIKOM-403.png)

FUNGSI LINEAR


---

\>function e(x,y):= 25x+15y-5

\>plot3d("e"):


![images/Final%20Projek%20APLIKOM-404.png](images/Final%20Projek%20APLIKOM-404.png)

\>plot3d("e",\>user, ...  
\>   title="Turn with the vector keys (press return to finish)"):


![images/Final%20Projek%20APLIKOM-405.png](images/Final%20Projek%20APLIKOM-405.png)

\>plot3d("e",r=10,n=80,fscale=4,scale=1.2,frame=3):


![images/Final%20Projek%20APLIKOM-406.png](images/Final%20Projek%20APLIKOM-406.png)

\>view


    [5,  2.6,  2,  0.4]

\>plot3d("e",distance=3,zoom=2,angle=0,height=0):


![images/Final%20Projek%20APLIKOM-407.png](images/Final%20Projek%20APLIKOM-407.png)

\>plot3d("e",a=0,b=1,c=-1,d=1,angle=-20°,height=20°, ...  
\>   center=[0.4,0,0],zoom=5):


![images/Final%20Projek%20APLIKOM-408.png](images/Final%20Projek%20APLIKOM-408.png)

\>plot3d("e",r=2,<fscale,<scale,distance=13,height=50°, ...  
\>   center=[0,0,-2],frame=3):


![images/Final%20Projek%20APLIKOM-409.png](images/Final%20Projek%20APLIKOM-409.png)

\>plot3d("e",r=5,\>polar, ...  
\>   fscale=2,\>hue,n=100,zoom=4,\>contour,color=gray):


![images/Final%20Projek%20APLIKOM-410.png](images/Final%20Projek%20APLIKOM-410.png)

\>plot3d("x","e","y",r=2,zoom=3.5,frame=3):


![images/Final%20Projek%20APLIKOM-411.png](images/Final%20Projek%20APLIKOM-411.png)

FUNGSI TRIGONOMETRI


---

\>function f(x,y):= cos(x+y)

\>plot3d("f")

\>plot3d("f",\>user, ...  
\>   title="Turn with the vector keys (press return to finish)"):


![images/Final%20Projek%20APLIKOM-412.png](images/Final%20Projek%20APLIKOM-412.png)

\>plot3d("f",r=10,n=80,fscale=4,scale=1.2,frame=3):


![images/Final%20Projek%20APLIKOM-413.png](images/Final%20Projek%20APLIKOM-413.png)

\>view


    [5,  2.6,  2,  0.4]

\>plot3d("f",distance=3,zoom=2,angle=0,height=0):


![images/Final%20Projek%20APLIKOM-414.png](images/Final%20Projek%20APLIKOM-414.png)

\>plot3d("f",a=0,b=1,c=-1,d=1,angle=-20°,height=20°, ...  
\>   center=[0.4,0,0],zoom=5):


![images/Final%20Projek%20APLIKOM-415.png](images/Final%20Projek%20APLIKOM-415.png)

\>plot3d("f",r=5,\>polar, ...  
\>   fscale=2,\>hue,n=100,zoom=4,\>contour,color=gray):


![images/Final%20Projek%20APLIKOM-416.png](images/Final%20Projek%20APLIKOM-416.png)

## 3) Menggambar Grafik Fungsi Dua Variabel yang Fungsinya

## Didefinisikan sebagai Fungsi Numerik

Sebelum masuk ke cara memvisualisasikan grafik, perlu diketahui apa
itu fungsi dua variabel dan apa itu fungsi numerik.


## Fungsi Dua Variabel

Fungsi dua variabel adalah jenis fungsi di mana ada dua variabel bebas
(biasanya dinotasikan sebagai x dan y) yang menentukan nilai dari
fungsi tersebut. Dengan kata lain, untuk setiap kombinasi nilai dari x
dan y, fungsi ini akan menghasilkan satu nilai output tertentu. Fungsi
dari dua variabel yang mana setiap kombinasi nilai dari kedua variabel
tersebut menghasilkan sebuah nilai tunggal.


## Fungsi Numerik

Fungsi dimana setiap pasangan variabel independen adalah angka atau
bilangan nyata. Secara sederhana, ketika memasukkan angka atau
bilangan nyata ke variabel-variabel dalam fungsi maka hasil akhir yang
dihasilkan juga angka atau bilangan nyata, bukan simbol atau ekspresi
yang belum dihitung.


Contoh:


ada fungsi


$$f(x,y)=2x+y$$Ketika kita memasukkan bilangan nyata ke x dan y maka akan dihasilkan
suatu bilangan nyata juga. Misal masukkan x=1 dan y=1. Akan diperoleh


$$2(1)+1=3$$## Visualisasi Grafik

Untuk memvisualisaikan fungsi dua variabel dengan fungsinya
didefinisikan sebagai fungsi numerik, akan dibuat grafik 3D dengan
sintaks plot3d. Untuk membedakan fungsi numerik dengan simbolik, pada
kali ini untuk setiap fungsi numerik dua variabel hanya akan memuat
variabel x dan y. Namun, dalam pemakaian secara umum, bisa digunakan
variabel apapun.


Penulisan Sintaks:


1) definisikan fungsi numerik


function f(x,y):= ax+by dengan a dan b adalah suatu konstanta dan
fungsi tidak selalu direpresentastikan dengan f tetapi bisa dengan
huruf apapun. Contoh : g(x,y)


2) sintaks plot3d


plot3d("f"):


Contoh Visualisasi Grafik:


1. Visualisasi grafik fungsi linear dua variabel


$$f(x,y) = 9x+2y$$\>function f(x,y):= 9\*x+2\*y

\>plot3d("f"):


![images/Final%20Projek%20APLIKOM-420.png](images/Final%20Projek%20APLIKOM-420.png)

2. Visualisasi grafik fungsi kuadrat dua variabel


$$f(x,y)=x^2+2xy+y^2$$\>function f(x,y):= x^2+2\*x\*y+y^2 

\>plot3d("f"):


![images/Final%20Projek%20APLIKOM-422.png](images/Final%20Projek%20APLIKOM-422.png)

3. Visualisasi Grafik Fungsi Eksponen Dua Variabel


$$g(x,y) = 6x^{2y+8}$$\>function g(x,y):= 6\*x^(2y+8)

\>plot3d("g"):


![images/Final%20Projek%20APLIKOM-424.png](images/Final%20Projek%20APLIKOM-424.png)

4. Grafik Fungsi Logaritma Dua Variabel


$$f(x,y)=\log(xy)$$\>function f(x,y):= log(x\*y)

\>plot3d("f"):


![images/Final%20Projek%20APLIKOM-426.png](images/Final%20Projek%20APLIKOM-426.png)

5. Grafik Fungsi Trigonometri Dua Variabel


$$h(x,y)=sin(xy)cos(y)$$\>function h(x,y):= sin(x\*y)\*cos(y)

\>plot3d("h"): 


![images/Final%20Projek%20APLIKOM-428.png](images/Final%20Projek%20APLIKOM-428.png)

6. Grafik Fungsi Nilai Mutlak Dua Variabel


$$i(x,y)=|(2x+y)|$$\>function i(x,y):= abs(2x+y)

\>plot3d("i"):


![images/Final%20Projek%20APLIKOM-430.png](images/Final%20Projek%20APLIKOM-430.png)

# Latihan Soal

Buatlah visualisasi grafik dari fungsi berikut ini!


$$f(x,y)=8^x+3y$$\>function f(x,y):=8^x+3\*y

\>plot3d ("f"):


![images/Final%20Projek%20APLIKOM-432.png](images/Final%20Projek%20APLIKOM-432.png)

$$g(x,y)=sin(7x^2y+1)$$\>function g(x,y):= sin(7\*x^2\*y+1)

\>plot3d("g"):


![images/Final%20Projek%20APLIKOM-434.png](images/Final%20Projek%20APLIKOM-434.png)

$$h(x,y)=|16x+sin(y^3+1)|$$\>function h(x,y):=abs(16\*x + sin(y^3+1))

\>plot3d("h"):


![images/Final%20Projek%20APLIKOM-436.png](images/Final%20Projek%20APLIKOM-436.png)

## 4) Menggambar Grafik Fungsi Dua Variabel yang Fungsinya

## Didefinisikan sebagai Fungsi Simbolik

Grafik Fungsi dua variabel yang fungsinya didefinisikan sebagai fungsi
simbolik adalah suatu grafik yang memvisualisasikan Persamaan Linear
Dua Variabel (PLDV) dalam koordinat kartesius dengan fungsinya
merupakan fungsi simbolik.


Proses visualisasi ini memungkinkan Kita untuk melihat dan memahami
bagaimana fungsi tersebut berperilaku dalam tiga dimensi.


Sedangkan yang dimaksud dengan fungsi simbolik yaitu fungsi yang
didefinisikan dalam bentuk matematika simbolik, artinya kita memiliki
ekspresi matematika yang menggambarkan hubungan antara dua variabel.
misalnya, jika kita memiliki fungsi


$$f(x, y) = x^2 + y^2$$

kita dapat menggambar grafiknya untuk melihat bentuk permukaan yang
dihasilkan oleh fungsi ini dalam tiga dimensi. Grafik ini mungkin akan
berupa tumpukan parabola yang membentuk kerucut.


Karakteristik fungsi simbolik adalah dengan mengganti tanda := menjadi
&amp;=


Perbedaan utama antara fungsi numerik dan fungsi simbolik adalah bahwa
fungsi numerik memberikan hasil numerik secara langsung (menghasilkan
angka), sementara fungsi simbolik memungkinkan kita untuk bekerja
dengan simbol matematika sebelum menghitung nilai numeriknya. Pilihan
antara keduanya tergantung pada kebutuhan analisis matematika yang
kita lakukan.


Tujuan menggambar grafik fungsi dua variabel adalah untuk memahami
pola, sifat, dan hubungan antara dua variabel tersebut secara visual,
yang dapat membantu dalam analisis dan pemahaman masalah matematika
atau ilmu pengetahuan yang melibatkan fungsi ini.


## Langkah-langkah Membuat Grafik

1) Definisikan fungsinya terlebih dahulu. Tentukan fungsi dua variabel
yang akan divisualisasikan dalam bentuk simbolik.


Misal diambil fungsi


$$f(x,y)=4x^2+y^2$$

Maka perintah yang dapat dituliskan yaitu:


\>function f(x,y)&= 4\*x^2+y^2;


2) Panggil fungsinya


\>plot3d("f(x,y)"):


![images/Final%20Projek%20APLIKOM-439.png](images/Final%20Projek%20APLIKOM-439.png)

3) Tentukan rentang variabelnya


\>plot3d("f(x,y)",-5,5,0,6\*pi):


![images/Final%20Projek%20APLIKOM-440.png](images/Final%20Projek%20APLIKOM-440.png)

## Membuat Grafik Fungsi Linear

$$g(x,y)=8x+4y$$\>function g(x,y) &= 8\*x+4\*y;

\>plot3d("g(x,y)"):


![images/Final%20Projek%20APLIKOM-442.png](images/Final%20Projek%20APLIKOM-442.png)

$$M(x,y)=-12x+7y$$\>function M(x,y) &= -12\*x+7\*y;

\>plot3d("M(x,y)"):


![images/Final%20Projek%20APLIKOM-444.png](images/Final%20Projek%20APLIKOM-444.png)

Rentang variabel:


\>plot3d("M(x,y)",-2,2,0,6\*pi):


![images/Final%20Projek%20APLIKOM-445.png](images/Final%20Projek%20APLIKOM-445.png)

## Membuat Grafik Fungsi Kuadrat

$$Q(x,y)=5x^2-7y^2$$\>function Q(x,y) &= 5\*x^2 - 7\*y^2;

\>plot3d("Q(x,y)"):


![images/Final%20Projek%20APLIKOM-447.png](images/Final%20Projek%20APLIKOM-447.png)

$$P(x,y)=8x^2-2xy+6y^2$$\>function P(x,y) &= 8\*x^2-2\*x\*y+6\*y^2;

\>plot3d("P(x,y)"):


![images/Final%20Projek%20APLIKOM-449.png](images/Final%20Projek%20APLIKOM-449.png)

Rentang variabel:


\>plot3d("P(x,y)",-10,10,0,9\*pi):


![images/Final%20Projek%20APLIKOM-450.png](images/Final%20Projek%20APLIKOM-450.png)

## Membuat Grafik Fungsi Akar Kuadrat

$$A(x,y)= \sqrt{49x^2+16y^2}$$\>function A(x,y) &= sqrt(49\*x^2+16\*y^2);

\>plot3d("A"):


![images/Final%20Projek%20APLIKOM-452.png](images/Final%20Projek%20APLIKOM-452.png)

$$W(x,y)= \sqrt{6x^2-2y^2}$$\>function W(x,y) &= sqrt(6\*x^2-2\*y^2);

\>plot3d("W"):


![images/Final%20Projek%20APLIKOM-454.png](images/Final%20Projek%20APLIKOM-454.png)

Rentang Variabel:


\>plot3d("W(x,y)",-20,100,0,5\*pi):


![images/Final%20Projek%20APLIKOM-455.png](images/Final%20Projek%20APLIKOM-455.png)

## Membuat Grafik Fungsi Eksponensial

$$F(x,y)= 27.12^{xy}$$\>function F(x,y) &= 27\*12^(x\*y);

\>plot3d("F"):


![images/Final%20Projek%20APLIKOM-457.png](images/Final%20Projek%20APLIKOM-457.png)

$$H(x,y)=25.(-20)^{xy}$$\>function H(x,y) &= 25\*-12^(x\*y);

\>plot3d("H"):


![images/Final%20Projek%20APLIKOM-459.png](images/Final%20Projek%20APLIKOM-459.png)

$$T(x,y)=(-21).8^{xy}$$\>function T(x,y) &= -21\*8^(x\*y);

\>plot3d("T"):


![images/Final%20Projek%20APLIKOM-461.png](images/Final%20Projek%20APLIKOM-461.png)

## Membuat Grafik Fungsi Logaritma

$$B(x,y)=log(x.2y), Basis 10$$\>function B(x,y) &= log(x\*2\*y);

\>plot3d("B"):


![images/Final%20Projek%20APLIKOM-463.png](images/Final%20Projek%20APLIKOM-463.png)

$$C(x,y)=log(30x.45y), basis 10$$\>function C(x,y) &= log(30\*x\*45\*y);

\>plot3d("C"):


![images/Final%20Projek%20APLIKOM-465.png](images/Final%20Projek%20APLIKOM-465.png)

## Membuat Grafik Fungsi Trigonometri

$$D(x,y)=sin(6x).cos(16y)$$\>function D(x,y) &= sin(6\*x)\*cos(16\*y);

\>plot3d("D"):


![images/Final%20Projek%20APLIKOM-467.png](images/Final%20Projek%20APLIKOM-467.png)

$$J(x,y)=sin(2x).tan(y)$$\>function J(x,y) &= sin(2\*x)\*tan(y);

\>plot3d("J"):


![images/Final%20Projek%20APLIKOM-469.png](images/Final%20Projek%20APLIKOM-469.png)

## Membuat Grafik Fungsi Nilai Mutlak

$$T(x,y)=|2x^2-y^2|$$\>function T(x,y) &= abs(2\*x^2 - y^2);

\>plot3d("T"):


![images/Final%20Projek%20APLIKOM-471.png](images/Final%20Projek%20APLIKOM-471.png)

## Latihan

Buatlah grafik dari fungsi berikut:


$$A(x,y)=x^2y+3y^2$$\>function A(x,y) &= x^2\*y+3\*y^2;

\>plot3d ("A"):


![images/Final%20Projek%20APLIKOM-473.png](images/Final%20Projek%20APLIKOM-473.png)

$$B(x,y)=4y^2-2x^2y+4x^3+24x^2$$\>function B(x,y)&= 4\*y^2-2\*x^2\*y+4\*x^3+24\*x^2;

\>plot3d("B"):


![images/Final%20Projek%20APLIKOM-475.png](images/Final%20Projek%20APLIKOM-475.png)

$$C(x,y)=cosec(9x)-tan(2y)$$\>function C(x,y)&= cosec(9\*x)-tan(2\*y);

\>plot3d ("C"):


![images/Final%20Projek%20APLIKOM-477.png](images/Final%20Projek%20APLIKOM-477.png)

Beri rentang variabel untuk fungsi C(x,y):


-100,50,0,2*pi


\>plot3d("C(x,y)",-100,50,0,2\*pi): 


![images/Final%20Projek%20APLIKOM-478.png](images/Final%20Projek%20APLIKOM-478.png)

## 5) Menggambar Data $x$, $y$, $z$ pada ruang Tiga Dimensi (3D)

  Menggambar data pada ruang tiga dimensi (3D) adalah proses  

visualisasi data yang mengubah informasi dalam tiga dimensi, yaitu
panjang, lebar, dan tinggi, menjadi representasi visual yang dapat
dipahami dan dianalisis.


  Tujuan dari menggambar data 3D adalah untuk membantu pemahaman dan  

interpretasi data yang lebih baik, terutama ketika data tersebut
memiliki komponen yang tidak dapat direpresentasikan dengan baik dalam
dua dimensi.


Sama seperti plot2d, plot3d menerima data. Untuk objek 3D, kita perlu
menyediakan matriks nilai x-, y- dan z, atau tiga fungsi atau ekspresi
fx(x,y), fy(x,y), fz(x,y).


$$\gamma(t,s) = (x(t,s),y(t,s),z(t,s))$$Karena x,y,z adalah matriks, kita asumsikan bahwa (t,s) melalui sebuah
kotak persegi. Hasilnya, kita dapat memplot gambar persegi panjang di
ruang angkasa.


Kita dapat menggunakan bahasa matriks Euler untuk menghasilkan
koordinat secara efektif.


Dalam contoh berikut, kami menggunakan vektor nilai t dan vektor kolom
nilai s untuk membuat parameter permukaan bola. Dalam gambar kita
dapat menandai daerah, dalam kasus kita daerah kutub.


## Contoh 1 grafik fungsi

\>t=-1:0.1:1; s=(-1:0.1:1)'; plot3d(t,s,t\*s):


![images/Final%20Projek%20APLIKOM-480.png](images/Final%20Projek%20APLIKOM-480.png)

Penjelasan sintaks dari plot


- plot3d = membawa euler untuk mengetahui perintah apa yang harus
dilakukan


- (” ...”) = tempat kita untuk memasukkan perintah yang kita inginkan


## Contoh 2

kita akan memebentuk plot dengan fungsi dibawah ini


$$5x^2 + y^2$$\>plot3d("5\*x^2+y^2"):


![images/Final%20Projek%20APLIKOM-482.png](images/Final%20Projek%20APLIKOM-482.png)

Selanjutnya kita akan menggambar garis pada plot dengan menggunakan
grid


\>plot3d("5\*x^2+y^2",grid=2):


![images/Final%20Projek%20APLIKOM-483.png](images/Final%20Projek%20APLIKOM-483.png)

Jika kita ingin memodifikasi plot dengan menambahkan warna pada plot,
bisa menggunakan fillcolor.


Fillcolor dapat diisi dengan 1 warna yang sama atau 2 warna yang
berbeda


\>plot3d("5\*x^2+y^2",grid= 2,fillcolor=[red,blue]):


![images/Final%20Projek%20APLIKOM-484.png](images/Final%20Projek%20APLIKOM-484.png)

## Contoh 3

Jika kita ingin membuat plot 3d pada fungsi


$$12x^2+y^3$$kita bisa menggunakan perintah seperti dibawah ini


\>plot3d("12x^2+y^3",grid=10,\>hue, color=red);

\>insimg()


![images/Final%20Projek%20APLIKOM-486.png](images/Final%20Projek%20APLIKOM-486.png)

Jika kita mau menebalkan warna pada gambar diatas makam bisa
menggunakan perintah


\>plot3d("12x^2+y^3",grid=10,fillcolor=[red,yellow]);

\>insimg()


![images/Final%20Projek%20APLIKOM-487.png](images/Final%20Projek%20APLIKOM-487.png)

## Contoh 4

Tentu saja, titik cloud juga dimungkinkan. Untuk memplot data titik
dalam ruang, kita membutuhkan tiga vektor untuk koordinat titik-titik
tersebut.


Gayanya sama seperti di plot2d dengan points=true;


\>n=500;...  
\>   plot3d(normal(1,n),normal(1,n),normal(1,n),points=true,style="."):


![images/Final%20Projek%20APLIKOM-488.png](images/Final%20Projek%20APLIKOM-488.png)

## 6) Membuat Gambar Grafik Tiga Dimensi (3D) yang

## Bersifat Interaktif dan animasi grafik 3D

Membuat gambar grafik tiga dimensi (3D) yang bersifat interaktif
adalah proses menciptakan visualisasi tiga dimensi yang memungkinkan
pengguna berinteraksi dengan objek-objek 3D. Interaktivitas dalam
gambar 3D memungkinkan pengguna untuk melakukan tindakan seperti
mengubah sudut pandang, memindahkan objek, atau berinteraksi dengan
elemen-elemen dalam adegan 3D. Sedangkan animasi grafik 3D dapat
mencakup pergerakan, tetapi juga dapat berarti perubahan dalam
tampilan atau atribut objek tanpa pergerakan fisik yang mencolok.


Interaksi user dimungkinkan dengan parameter &gt;user. dengan perintah
&gt;user kita dapat menekan tombol berikut.


* 
kiri, kanan, atas, bawah: memutar sudut pandang

* 
+,-: memperbesar atau memperkecil

* 
a: menghasilkan anaglyph (lihat di bawah)

* 
l : tombol nyalakan sumber cahaya (lihat dibawah)

* 
spasi: reset ke default

* 
kembali: akhiri interaksi


\>plot3d("exp(-x^2+y^2)",\>user,...  
\>   title="Coba gerakkan"): 


![images/Final%20Projek%20APLIKOM-489.png](images/Final%20Projek%20APLIKOM-489.png)

\>plot3d("exp(x^2+y^2)",\>user,...  
\>   title="Coba gerakkan)"):


![images/Final%20Projek%20APLIKOM-490.png](images/Final%20Projek%20APLIKOM-490.png)

## Animasi 3D

\>function testplot () := plot3d("x^2+y^3");...  
\>   rotate("testplot"); testplot():


![images/Final%20Projek%20APLIKOM-491.png](images/Final%20Projek%20APLIKOM-491.png)

Fungsi rotate yaitu untuk memutar plot.


Fungsi ini akan membuat animasi plot 3D dari fungsi


$$4x^2 + y^3$$

yang berputar di sekitar sumbu z dari sudut 0 hingga 360 derajat


\>plot3d("exp(-(4\*x^2+y^2)/5)",r=10,n=80,fscale=8,scale=1.2,frame=3,\>user):


![images/Final%20Projek%20APLIKOM-493.png](images/Final%20Projek%20APLIKOM-493.png)

Ada beberapa parameter untuk menskalakan fungsi atau mengubah tampilan
grafik.


fscale: menskalakan ke nilai fungsi (defaultnya adalah &lt;fscale).


scale: angka atau vektor 1x2 untuk diskalakan ke arah x dan y.


frame: jenis bingkai (default 1).


\>plot3d("4\*x^2+y^2",distance=10,zoom=5,angle=0,height=5):


![images/Final%20Projek%20APLIKOM-494.png](images/Final%20Projek%20APLIKOM-494.png)

Tampilan dapat diubah dengan berbagai cara.


* 
distance: jarak pandang ke plot.

* 
zoom: nilai zoom.

* 
angle: sudut terhadap sumbu y negatif dalam radian.

* 
height: ketinggian tampilan dalam radian.


\>plot3d("x^4+y^2",a=0,b=1,c=-1,d=1,angle=-20°,height=20°,...  
\>   center=[0,0,1],zoom=5):


![images/Final%20Projek%20APLIKOM-495.png](images/Final%20Projek%20APLIKOM-495.png)

Plot selalu terlihat berada di tengah kubus plot. Kita dapat
memindahkan bagian tengah dengan center parameter.


\>plot3d("x^2+1",a=-1,b=1,rotate=true,grid=5):


![images/Final%20Projek%20APLIKOM-496.png](images/Final%20Projek%20APLIKOM-496.png)

Parameter memutar memutar fungsi dalam x di sekitar sumbu x.


* 
rotate=1: Menggunakan sumbu x

* 
rotate=2: Menggunakan sumbu z


## 7) Menggambar Fungsi Parametrik Tiga Dimensi (3D)

## Pengertian

Fungsi parametrik adalah jenis fungsi matematika yang menggambarkan
hubungan antara dua atau lebih variabel, di mana setiap variabel
dinyatakan sebagai fungsi dari satu atau lebih parameter. Fungsi
parametrik digunakan untuk menggambarkan kurva, lintasan, atau
hubungan antara berbagai variabel yang bergantung pada
parameter-parameter tertentu.


Fungsi parametrik merupakan salah satu cara mendefinisikan kurva atau
permukaan dalam ruang 2D atau 3D menggunakan satu atau lebih parameter
independen.


* 
Dalam 2D, kurva dinyatakan sebagai x(t) dan y(t), di mana adalah t
* adalah parameter yang mengontrol posisi sepanjang kurva.

* 
Dalam 3D, kita menggunakan tiga persamaan parametrik untuk
* mendeskripsikan posisi x,y,z sebagai fungsi dari parameter t.Fungsi
* ini ditulis sebagai:
* x=f(t),
* y=g(t),
* z=h(t),


## Contoh Soal

\>plot3d("cos(x)\*cos(y)","sin(x)\*cos(y)","sin(y)", a=0,b=2\*pi,c=pi/2,d=-pi/2,...  
\>   \>hue,color=yellow,light=[0,1,0],<frame,...  
\>   n=90,grid=[25,50],wirecolor=black,zoom=4):


![images/Final%20Projek%20APLIKOM-497.png](images/Final%20Projek%20APLIKOM-497.png)

\>aspect(16/9); allwindow; ...  
\>   x:=linspace(0,2\*pi,100); y:=(-1:0.1:1)'; ...  
\>   plot3d(sin(x)\*(y/2\*sin(x/2)),cos(x)\*(y/2\*sin(x/2)),y/2\*cos(x/2), ...  
\>   <frame,hue=2,max=0.5,scale=1.5):


![images/Final%20Projek%20APLIKOM-498.png](images/Final%20Projek%20APLIKOM-498.png)

\>aspect(16/9); allwindow;...  
\>   x:=linspace(0,2\*pi,100); y:=(-1:0.1:1)';...  
\>   plot3d(sin(x)\*(y/2\*sin(x/2)),cos(x)\*(y/2\*sin(x/2)),y/2\*cos(x/2),...  
\>   \>lines,<frame,xmin=0,xmax=10,n=10,\>user):


![images/Final%20Projek%20APLIKOM-499.png](images/Final%20Projek%20APLIKOM-499.png)

\>reset;...  
\>   S:=normal(10,1250); plot3d(S[3],S[6],S[9],\>points,style="."):


![images/Final%20Projek%20APLIKOM-500.png](images/Final%20Projek%20APLIKOM-500.png)

\>S:=normal(10,1250); T:=cumsum(normal(10,1250));...  
\>   plot3d(T[2],T[5],T[8],\>wire,...  
\>   linewidth=2,\>anaglyph,zoom=3):


![images/Final%20Projek%20APLIKOM-501.png](images/Final%20Projek%20APLIKOM-501.png)

\>P=cumsum(normal(5,75));...  
\>   plot3d(P[3],P[4],P[5],\>anaglyph,\>wire):


![images/Final%20Projek%20APLIKOM-502.png](images/Final%20Projek%20APLIKOM-502.png)

## 8) Menggambar Fungsi Implisit Tiga Dimensi (3D)

Fungsi implisit (implicit function) adalah fungsi yang memuat lebih
dari satu variabel, berjenis variabel bebas dan variabel terikat yang
berada dalam satu ruas sehingga tidak bisa dipisahkan pada ruas yang
berbeda.


$$F(x,y,z)=0$$

(1 persamaan dan 3 variabel), terdiri dari 2 variabel bebas dan 1
terikat


Misalnya, F(x, y, z) = x^2 + y^2 + z^2 - 1 = 0 adalah persamaan
implisit yang menggambarkan bola dengan jari-jari 1 dan pusat di
(0,0,0).


Plot Implisit


Ada juga plot implisit dalam tiga dimensi. Euler menghasilkan
pemotongan melalui objek. Fitur plot3d mencakup plot implisit. Plot
ini menunjukkan himpunan nol suatu fungsi dalam tiga variabel.


Solusi dari


$$f(x,y,z) = 0$$dapat divisualisasikan dalam potongan yang sejajar dengan bidang x-y,
x-z, z-x dan y-z.


* 
implisit=1: dipotong sejajar bidang y-z

* 
implisit=2: dipotong sejajar dengan bidang x-z

* 
implisit=3: dipotong sejajar dengan bidang z-x (yang berarti
* pemotongan dilakukan dengan mempertahankan nilai y konstan)

* 
implisit=4: dipotong sejajar bidang x-y


Tambahkan nilai-nilai ini, jika Anda mau. Dalam contoh kita memplot


$$M = \{ (x,y,z) : x^2+y^3+zy=1 \}$$---

## Contoh Fungsi Implisit

\>plot3d("4\*x^2+y^3+z\*y-1",r=7,implicit=2):


![images/Final%20Projek%20APLIKOM-506.png](images/Final%20Projek%20APLIKOM-506.png)

\>plot3d("12\*x^2 + 9\*y^2 + 4\*z^2 - 25",r=8,implicit=4):


![images/Final%20Projek%20APLIKOM-507.png](images/Final%20Projek%20APLIKOM-507.png)

\>c=1; d=1;

\>plot3d("((x^2+y^2-c^2)^2+(z^2-1)^2)\*((y^2+z^2-c^2)^2+(x^2-1)^2)\*((z^2+x^2-c^2)^2+(y^2-1)^2)-d",r=2,<frame,\>implicit,\>user):


![images/Final%20Projek%20APLIKOM-508.png](images/Final%20Projek%20APLIKOM-508.png)

## Latihan soal

Gambarlah Fungsi implisit berikut dalam 3D


$$f(x,y,z)=5x^2+y^2-6z^2-12$$\>plot3d("5\*x^2+y^2-6\*z^2-12",r=8,implicit=3):


![images/Final%20Projek%20APLIKOM-510.png](images/Final%20Projek%20APLIKOM-510.png)

Gambarlah fungsi 3D dari fungsi implisit berikut ini


$$f(x,y,z)=xy+x^3y^2+xz^3-12=0$$

dengan r=4


\>plot3d("x\*y+x^3\*y^2+x\*z^3-12", r=4, implicit=3):


![images/Final%20Projek%20APLIKOM-512.png](images/Final%20Projek%20APLIKOM-512.png)

## 9) Mengatur tampilan, warna dan sudut pandang gambar permukaan

## Tiga Dimensi (3D) Dan Menampilkan kontur dan bidang kontur

## permukaan Tiga Dimensi(3D)

Untuk plot, Euler menambahkan garis grid. Sebagai gantinya
dimungkinkan untuk menggunakan garis level dan rona satu warna atau
rona berwarna spektral. Euler dapat menggambar tinggi fungsi pada plot
dengan bayangan. Di semua plot 3D, Euler dapat menghasilkan anaglyph
merah/sian.


-&gt; hue: Menyalakan bayangan cahaya alih-alih kabel.


-&gt; kontur: Memplot garis kontur otomatis pada plot.


- level=... (atau level): Sebuah vektor nilai untuk garis kontur.


Standarnya adalah level="auto", yang menghitung beberapa garis level
secara otomatis. Seperti yang Anda lihat di plot, level sebenarnya
adalah rentang level.


Gaya default dapat diubah. Untuk plot kontur berikut, kami menggunakan
grid yang lebih halus untuk 100x100 poin, skala fungsi dan plot, dan
menggunakan sudut pandang yang berbeda.


\>plot3d("exp(-x^2-y^2)",r=2,n=100,level="thin", ...  
\>    \>contour,\>spectral,fscale=1,scale=1.1,angle=45°,height=20°):


![images/Final%20Projek%20APLIKOM-513.png](images/Final%20Projek%20APLIKOM-513.png)

\>plot3d("exp(x\*y)",angle=100°,\>contour,color=yellow):


![images/Final%20Projek%20APLIKOM-514.png](images/Final%20Projek%20APLIKOM-514.png)

Bayangan default menggunakan warna abu-abu. Tetapi rentang warna
spektral juga tersedia.


-&gt; spektral: Menggunakan skema spektral default


- color=...: Menggunakan warna khusus atau skema spektral


Untuk plot berikut, kami menggunakan skema spektral default dan
menambah jumlah titik untuk mendapatkan tampilan yang sangat halus.


\>plot3d("x^2+y^2",\>spectral,\>contour,n=100):


![images/Final%20Projek%20APLIKOM-515.png](images/Final%20Projek%20APLIKOM-515.png)

Alih-alih garis level otomatis, kita juga dapat mengatur nilai garis
level. Ini akan menghasilkan garis level tipis alih-alih rentang
level.


\>plot3d("x^2-y^2",0,1,0,1,angle=220°,level=-1:0.2:1,color=redgreen):


![images/Final%20Projek%20APLIKOM-516.png](images/Final%20Projek%20APLIKOM-516.png)

Dalam plot berikut, kami menggunakan dua pita level yang sangat luas
dari -0,1 hingga 1, dan dari 0,9 hingga 1. Ini dimasukkan sebagai
matriks dengan batas level sebagai kolom.


Selain itu, kami melapisi kisi dengan 10 interval di setiap arah.


\>plot3d("x^2+y^3",level=[-0.1,0.9;0,1], ...  
\>     \>spectral,angle=30°,grid=10,contourcolor=blue):


![images/Final%20Projek%20APLIKOM-517.png](images/Final%20Projek%20APLIKOM-517.png)

Dalam contoh berikut, kami memplot himpunan, di mana


$$f(x,y) = x^y-y^x = 0$$Kami menggunakan satu garis tipis untuk garis level.


\>plot3d("x^y-y^x",level=0,a=0,b=6,c=0,d=6,contourcolor=red,n=100):


![images/Final%20Projek%20APLIKOM-519.png](images/Final%20Projek%20APLIKOM-519.png)

Dimungkinkan untuk menunjukkan bidang kontur di bawah plot. Warna dan
jarak ke plot dapat ditentukan.


\>plot3d("x^2+y^4",\>cp,cpcolor=green,cpdelta=0.2):


![images/Final%20Projek%20APLIKOM-520.png](images/Final%20Projek%20APLIKOM-520.png)

Berikut adalah beberapa gaya lagi. Kami selalu mematikan frame, dan
menggunakan berbagai skema warna untuk plot dan grid.


\>figure(2,2); ...  
\>   expr="y^3-x^2"; ...  
\>   figure(1);  ...  
\>     plot3d(expr,<frame,\>cp,cpcolor=spectral); ...  
\>   figure(2);  ...  
\>     plot3d(expr,<frame,\>spectral,grid=10,cp=2); ...  
\>   figure(3);  ...  
\>     plot3d(expr,<frame,\>contour,color=gray,nc=5,cp=3,cpcolor=greenred); ...  
\>   figure(4);  ...  
\>     plot3d(expr,<frame,\>hue,grid=10,\>transparent,\>cp,cpcolor=gray); ...  
\>   figure(0):


![images/Final%20Projek%20APLIKOM-521.png](images/Final%20Projek%20APLIKOM-521.png)

Ada beberapa skema spektral lainnya, bernomor dari 1 hingga 9. Tetapi
Anda juga dapat menggunakan warna=nilai, di mana nilai


* 
spektral: untuk rentang dari biru ke merah

* 
putih: untuk rentang yang lebih redup

* 
kuningbiru,ungu hijau,birukuning,hijaumerah

* 
birukuning, hijau ungu, kuning biru, merah hijau


\>figure(3,3); ...  
\>   for i=1:9;  ...  
\>     figure(i); plot3d("x^2+y^2",spectral=i,\>contour,\>cp,<frame,zoom=4);  ...  
\>   end; ...  
\>   figure(0):


![images/Final%20Projek%20APLIKOM-522.png](images/Final%20Projek%20APLIKOM-522.png)

Sumber cahaya dapat diubah dengan l dan tombol kursor selama interaksi
pengguna. Itu juga dapat diatur dengan parameter.


* 
cahaya: arah untuk cahaya

* 
amb: cahaya sekitar antara 0 dan 1


Perhatikan bahwa program tidak membuat perbedaan antara sisi plot.
Tidak ada bayangan. Untuk ini, Anda perlu Povray.


\>plot3d("-x^2-y^2", ...  
\>     hue=true,light=[0,1,1],amb=0,user=true, ...  
\>     title="Press l and cursor keys (return to exit)"):


![images/Final%20Projek%20APLIKOM-523.png](images/Final%20Projek%20APLIKOM-523.png)

Parameter warna mengubah warna permukaan. Warna garis level juga dapat
diubah.


\>plot3d("-x^2-y^2",color=rgb(0.2,0.2,0),hue=true,frame=false, ...  
\>     zoom=3,contourcolor=red,level=-2:0.1:1,dl=0.01):


![images/Final%20Projek%20APLIKOM-524.png](images/Final%20Projek%20APLIKOM-524.png)

Warna 0 memberikan efek pelangi khusus.


\>plot3d("x^2/(x^2+y^2+1)",color=0,hue=true,grid=10):


![images/Final%20Projek%20APLIKOM-525.png](images/Final%20Projek%20APLIKOM-525.png)

Permukaannya juga bisa transparan.


\>plot3d("x^2+y^2",\>transparent,grid=10,wirecolor=red):


![images/Final%20Projek%20APLIKOM-526.png](images/Final%20Projek%20APLIKOM-526.png)

## 10) Menggambar Diagram Batang Tiga Dimensi

Bar plots/plot batang juga dimungkinkan. Untuk itu, kita harus
menyediakannya


* 
x: vektor baris dengan n+1 elemen

* 
y: vektor kolom dengan n+1 elemen

* 
z: matriks nilai nxn.


z bisa lebih besar, tetapi hanya nilai nxn yang akan digunakan.


Dalam contoh ini, pertama-tama kita menghitung nilainya. Kemudian kita
sesuaikan x dan y, sehingga vektor-vektornya berpusat pada nilai yang
digunakan.


\>x=-1:0.1:1; y=x'; z=x^2+y^2; ...  
\>   xa=(x|1.1)-0.05; ya=(y\_1.1)-0.05; ...  
\>   plot3d(xa,ya,z,bar=true):


![images/Final%20Projek%20APLIKOM-527.png](images/Final%20Projek%20APLIKOM-527.png)

\>x=-0.01:0.1:1; y=x'; z=x+2/3\*y; ...  
\>   xa=(x|1.1)-0.05; ya=(y\_1.1)-0.05; ...  
\>   plot3d(xa,ya,z,bar=true):


![images/Final%20Projek%20APLIKOM-528.png](images/Final%20Projek%20APLIKOM-528.png)

\>x=-0.01:0.1:1; y=x'; z=1/2\*x+1/2\*y; ...  
\>   xa=(x|1.1); ya=(y\_1.1); ...  
\>   plot3d(xa,ya,z,bar=true):


![images/Final%20Projek%20APLIKOM-529.png](images/Final%20Projek%20APLIKOM-529.png)

Dimungkinkan untuk membagi plot suatu permukaan menjadi dua bagian
atau lebih.


\>x=-1:0.1:1; y=x'; z=1/10\*x+1/10\*y; d=zeros(size(x)); ...  
\>   plot3d(x,y,z,disconnect=2:2:5):


![images/Final%20Projek%20APLIKOM-530.png](images/Final%20Projek%20APLIKOM-530.png)

\>x=-1:0.1:1; y=x'; z=x+y; d=zeros(size(x)); ...  
\>   plot3d(x,y,z,disconnect=2:2:20):


![images/Final%20Projek%20APLIKOM-531.png](images/Final%20Projek%20APLIKOM-531.png)

Jika memuat atau menghasilkan matriks data M dari file dan perlu
memplotnya dalam 3D, Anda dapat menskalakan matriks ke [-1,1] dengan
skala(M), atau menskalakan matriks dengan &gt;zscale. Hal ini dapat
dikombinasikan dengan faktor penskalaan individual yang diterapkan
sebagai tambahan.


\>i=1:20; j=i'; ...  
\>   plot3d(i\*j^2+100\*normal(20,20),\>zscale,scale=[1,1,1.5],angle=-40°,zoom=1.8):


![images/Final%20Projek%20APLIKOM-532.png](images/Final%20Projek%20APLIKOM-532.png)

\>Z=intrandom(5,100,6); v=zeros(5,6); ...  
\>   loop 1 to 5; v[#]=getmultiplicities(1:6,Z[#]); end; ...  
\>   columnsplot3d(v',scols=1:5,ccols=[1:5]):


![images/Final%20Projek%20APLIKOM-533.png](images/Final%20Projek%20APLIKOM-533.png)

\>Z=intrandom(6,100,6); v=zeros(6,2); ...  
\>   loop 1 to 6; v[#]=getmultiplicities(1:2,Z[#]); end; ...  
\>   columnsplot3d(v',scols=1:6,ccols=[1:6]):


![images/Final%20Projek%20APLIKOM-534.png](images/Final%20Projek%20APLIKOM-534.png)

\>Z=intrandom(7,1000,6); v=zeros(7,1); ...  
\>   loop 1 to 7; v[#]=getmultiplicities(1:1,Z[#]); end; ...  
\>   columnsplot3d(v',scols=1:7,ccols=[1:7]):


![images/Final%20Projek%20APLIKOM-535.png](images/Final%20Projek%20APLIKOM-535.png)

## 11) Menggambar Permukaan Benda Putar

\>plot2d("(x^2+y^2-1)^3-x^2\*y^3",r=1.3, ...  
\>   style="#",color=blue,<outline, ...  
\>   level=[-2;0],n=100):


![images/Final%20Projek%20APLIKOM-536.png](images/Final%20Projek%20APLIKOM-536.png)

\>ekspresi &= (x^2+y^2-1)^3-x^2\*y^3; $ekspresi


$$\left(y^2+x^2-1\right)^3-x^2\,y^3$$Kami ingin memutar kurva jantung di sekitar sumbu y. Berikut adalah
ungkapan, yang mendefinisikan hati:


$$f(x,y)=(x^2+y^2-1)^3-x^2.y^3.$$Selanjutnya kita atur


$$x=r.cos(a),\quad y=r.sin(a).$$\>function fr(r,a) &= ekspresi with [x=r\*cos(a),y=r\*sin(a)] | trigreduce; $fr(r,a)


$$\left(r^2-1\right)^3+\frac{\left(\sin \left(5\,a\right)-\sin \left(
 3\,a\right)-2\,\sin a\right)\,r^5}{16}$$Hal ini memungkinkan untuk mendefinisikan fungsi numerik, yang
memecahkan r, jika a diberikan. Dengan fungsi itu kita dapat memplot
jantung yang diputar sebagai permukaan parametrik.


\>function map f(a) := bisect("fr",0,2;a); ...  
\>   t=linspace(-pi/2,pi/2,100); r=f(t);  ...  
\>   s=linspace(pi,2pi,100)'; ...  
\>   plot3d(r\*cos(t)\*sin(s),r\*cos(t)\*cos(s),r\*sin(t), ...  
\>   \>hue,<frame,color=yellow,zoom=4,amb=0,max=0.7,grid=12,height=50°):


![images/Final%20Projek%20APLIKOM-541.png](images/Final%20Projek%20APLIKOM-541.png)

Berikut ini adalah plot 3D dari gambar di atas yang diputar di sekitar
sumbu z. Kami mendefinisikan fungsi, yang menggambarkan objek.


\>function f(x,y,z) ...


    r=x^2+y^2;
    return (r+z^2-1)^3-r*z^3;
     endfunction
</pre>
\>plot3d("f(x,y,z)", ...  
\>   xmin=0,xmax=1.2,ymin=-1.2,ymax=1.2,zmin=-1.2,zmax=1.4, ...  
\>   implicit=1,angle=-30°,zoom=2.5,n=[10,60,60],\>anaglyph):


![images/Final%20Projek%20APLIKOM-542.png](images/Final%20Projek%20APLIKOM-542.png)

## 12) Menggambar Grafik 3D dengan Povray di EMT

Menggambar Povray Dengan bantuan file Euler povray.e, Euler dapat
menghasilkan file Povray. Hasilnya sangat bagus untuk dilihat.


Untuk dapat menjalankan sintaks dalam povray perlu menginstal Povray
(32bit atau 64bit) dari http://www.povray.org/, dan meletakkan
sub-direktori "bin" dari Povray ke pathway, atau mengatur variabel
"defaultpovray" dengan path lengkap yang menunjuk ke "pvengine.exe".


Interface Povray dari Euler menghasilkan file Povray di direktori home
pengguna, dan memanggil Povray untuk mengurai file-file ini. Nama file
default adalah current.pov, dan direktori default adalah eulerhome(),
biasanya c:\Users\Username\Euler. Povray menghasilkan file PNG, yang
dapat dimuat oleh Euler ke dalam buku catatan. Untuk membersihkan
file-file ini, gunakan povclear().


Sintaks yang digunakan untuk menjalankan povray adalah pov3d. Fungsi
pov3d memiliki komponen yang sama dengan plot3d. Ini dapat
menghasilkan grafik fungsi f(x,y), atau permukaan dengan koordinat
X,Y,Z dalam matriks, termasuk garis level opsional. Fungsi ini memulai
raytracer secara otomatis, dan memuat gambar ke dalam notebook Euler.


Selain pov3d(), ada banyak fungsi yang menghasilkan objek Povray.
Fungsi-fungsi ini mengembalikan string, yang berisi kode Povray untuk
objek. Untuk menggunakan fungsi ini, mulai file Povray dengan
povstart(). Kemudian gunakan writeln(...) untuk menulis objek ke file
gambar. Terakhir, akhiri file dengan povend(). Secara default,
raytracer akan dimulai, dan PNG akan dimasukkan ke dalam notebook
Euler.


Fungsi objek memiliki parameter yang disebut "look", yang membutuhkan
string dengan kode Povray untuk tekstur dan hasil akhir objek. Fungsi
povlook() dapat digunakan untuk menghasilkan string ini. Ini memiliki
parameter untuk warna, transparansi, Phong Shading dll.


Lingkup Povray memiliki sistem koordinat lain. Interface ini
menerjemahkan semua koordinat ke sistem Povray. Jadi Anda dapat terus
berpikir dalam sistem koordinat Euler dengan z menunjuk vertikal ke
atas, dan x,y,z sumbu dalam arti tangan kanan.


Anda perlu memuat file povray.


\>load povray;


Pastikan, direktori bin Povray ada di path. Jika tidak, edit variabel
berikut sehingga berisi path ke povray yang dapat dieksekusi.


\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

## Contoh Penggunaan



Akan diberikan contoh sederhana penggunaan povray pada EMT


Perintah berikut menghasilkan file povray di direktori pengguna dan
menjalankan Povray untuk ray tracing file ini.


Jika memulai perintah berikut, GUI Povray akan terbuka, menjalankan
file, dan menutup secara otomatis. Karena alasan keamanan, akan
ditanya, apakah ingin mengizinkan file exe untuk dijalankan. Agar
pertanyaan tersebut tidak muncul lagi bisa dipilih batal.


\>pov3d("3\*x^2+4\*y^2",zoom=4);


![images/Final%20Projek%20APLIKOM-543.png](images/Final%20Projek%20APLIKOM-543.png)

hasil visualisasi fungsi dapat dibuat menjadi transparan dan
menambahkan hasil akhir lainnya.


\> pov3d("(x^2+y^3)",axiscolor=blue,angle=30°, ...  
\>     look=povlook(yellow,0.2),level=-1:0.5:1,zoom=3);


![images/Final%20Projek%20APLIKOM-544.png](images/Final%20Projek%20APLIKOM-544.png)

\>pov3d("((x-1)^2+(y+1)^2)\*((x+1)^2+y^2)/40",r=1.5, ...  
\>     angle=120°,level=1/40,dlevel=0.005,light=[-1,1,1],height=45°,n=50, ...  
\>     <fscale,zoom=3.8);


![images/Final%20Projek%20APLIKOM-545.png](images/Final%20Projek%20APLIKOM-545.png)

## Object Povray



Contoh-contoh di atas tadi merupakan visualisasi permukaan fungsi
dengan menggunakan sintaks pov3d. Untuk menghasilkan objek dalam
povray perlu ditulis menjadi file povray.


Untuk menghasilkan output dimulai dengan povstart()


\>load povray; ...  
\>   defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

\>povstart(zoom=3.5)

\>c1=povcylinder(-povx,povx,1,povlook(orange)); ...  
\>   c2=povcylinder(-povy,povy,1,povlook(yellow)); ...  
\>   c3=povcylinder(-povz,povz,1,povlook(lightblue));


Di atas telah didefinisikan tiga silinder yang disimpan dalam string


di Euler. Fungsi povx(), povy(), dll. hanya mengembalikan vektor


[1,0,0] yang dapat digunakan sebagai gantinya.


\>c1


    cylinder { &lt;-1,0,0&gt;, &lt;1,0,0&gt;, 1
     texture { pigment { color rgb &lt;0.941176,0.509804,0.392157&gt; }  } 
     finish { ambient 0.2 } 
     }

Akan ditambahkan tekstur ke objek dengan tiga warna berbeda yaitu
orange, yellow, dan lightblue.


Untuk menamahkan tekstur ini dapat digunakan sintaks povlook(), yang
mengembalikan string dengan kode Povray yang relevan. Selain
menambahkan warna, ditambahkan juga transparansi dan cahaya.


\>povlook(rgb(0.1,0.2,0.3),0.1,0.5)


     texture { pigment { color rgbf &lt;0.101961,0.2,0.301961,0.1&gt; }  } 
     finish { ambient 0.5 } 
    

\>writeln(povintersection([c1,c2,c3]));

\>povend;


![images/Final%20Projek%20APLIKOM-546.png](images/Final%20Projek%20APLIKOM-546.png)

## Contoh Lain

Akan ditampilkan fungsi untuk membuat sebuah donat


\>povstart(angle=0,height=45°); //height untuk menampilkan fungsi dengan suatiu derajat tertentu 

\>function povdonat (r1,r2,look="") := "torus {"+r1+","+r2+look+"}"; //fungsi untuk menampilkan sebuah donat

\>writeln(povobject(povdonat(1,0.5),povlook(lightblue,\>phong),xrotate(90°)));

\>povend();


![images/Final%20Projek%20APLIKOM-547.png](images/Final%20Projek%20APLIKOM-547.png)

## 13) Menggambar Grafik Tiga Dimensi alam modus anaglif

Untuk menghasilkan anaglyph untuk kacamata merah/sian, Povray harus
berjalan dua kali dari posisi kamera yang berbeda. Ini menghasilkan
dua file Povray dan dua file PNG, yang dimuat dengan fungsi
loadanaglyph().


Tentu saja, Anda memerlukan kacamata merah/sian untuk melihat contoh
berikut dengan benar.


Fungsi pov3d() memiliki sakelar sederhana untuk menghasilkan
anaglyphs.


\>pov3d("-exp(-x^2-y^2)/2",r=2,height=45°,\>anaglyph, ...  
\>     center=[0,0,0.5],zoom=3.5);


![images/Final%20Projek%20APLIKOM-548.png](images/Final%20Projek%20APLIKOM-548.png)

Jika Anda membuat adegan dengan objek, Anda perlu menempatkan generasi
adegan ke dalam fungsi, dan menjalankannya dua kali dengan nilai yang
berbeda untuk parameter anaglyph.


\>function myscene ...


      s=povsphere(povc,1);
      cl=povcylinder(-povz,povz,0.5);
      clx=povobject(cl,rotate=xrotate(90°));
      cly=povobject(cl,rotate=yrotate(90°));
      c=povbox([-1,-1,0],1);
      un=povunion([cl,clx,cly,c]);
      obj=povdifference(s,un,povlook(red));
      writeln(obj);
      writeAxes();
    endfunction
</pre>
Fungsi povanaglyph() melakukan semua ini. Parameternya seperti di
povstart() dan povend() digabungkan.


\>povanaglyph("myscene",zoom=4.5);


![images/Final%20Projek%20APLIKOM-549.png](images/Final%20Projek%20APLIKOM-549.png)

## 14) Fungsi Implisit menggunakan Povray

Povray dapat memplot himpunan di mana f(x,y,z)=0, seperti parameter
implisit di plot3d. Namun hasilnya terlihat jauh lebih baik.


Sintaks untuk fungsinya sedikit berbeda. Anda tidak dapat menggunakan
keluaran ekspresi Maxima atau Euler.


$$((x^2+y^2-c^2)^2+(z^2-1)^2)*((y^2+z^2-c^2)^2+(x^2-1)^2)*((z^2+x^2-c^2)^2+(y^2-1)^2)=d$$\>load povray;

\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

\>povstart(angle=25°,height=10°);

\>writeln(povsurface("pow(x,2)+pow(y,2)\*pow(z,2)-1",povlook(blue),povbox(-2,2,"")));

\>povend();


![images/Final%20Projek%20APLIKOM-551.png](images/Final%20Projek%20APLIKOM-551.png)

\>load povray;

\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

\>povstart(angle=70°,height=50°,zoom=4);

\>writeln(povsurface("pow(x,2)\*y-pow(y,3)-pow(z,2)",povlook(green))); ...  
\>   writeAxes(); ...  
\>   povend();


![images/Final%20Projek%20APLIKOM-552.png](images/Final%20Projek%20APLIKOM-552.png)

\>load povray;

\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

\>povstart(angle=70°,height=30°);

\>writeln(povsurface("pow(x,2)+pow(y,2)\*pow(z,2)-1",povlook(red),povbox(-2,2,"")));

\>povend();


![images/Final%20Projek%20APLIKOM-553.png](images/Final%20Projek%20APLIKOM-553.png)

## Contoh lain

\>povstart(angle=45, height=100);

\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

\>writeln(povsurface("pow(x,2)+pow(y,3)\*pow(z,2)-1", povlook(blue),povbox(-25,4,""))); 

\>povend(); 


![images/Final%20Projek%20APLIKOM-554.png](images/Final%20Projek%20APLIKOM-554.png)

## 15) Menggambar Titik pada ruang Tiga Dimensi (3D)

Alih-alih fungsi, kita dapat memplot dengan koordinat. Seperti pada
plot3d, kita membutuhkan tiga matriks untuk mendefinisikan objek.


Dalam contoh kita memutar fungsi di sekitar sumbu z.


\>function f(x) := x^3-x+1; ...  
\>   x=-1:0.01:1; t=linspace(0,2pi,8)'; ...  
\>   Z=x; X=cos(t)\*f(x); Y=sin(t)\*f(x); ...  
\>   pov3d(X,Y,Z,angle=40°,height=20°,axis=0,zoom=4,light=[10,-5,5]);


![images/Final%20Projek%20APLIKOM-555.png](images/Final%20Projek%20APLIKOM-555.png)

Dalam contoh berikut, kami memplot gelombang teredam. Kami
menghasilkan gelombang dengan bahasa matriks Euler.


Kami juga menunjukkan, bagaimana objek tambahan dapat ditambahkan ke
adegan pov3d. Untuk pembuatan objek, lihat contoh berikut. Perhatikan
bahwa plot3d menskalakan plot, sehingga cocok dengan kubus satuan.


\>r=linspace(0,1,80); phi=linspace(0,2pi,80)'; ...  
\>   x=r\*cos(phi); y=r\*sin(phi); z=exp(-5\*r)\*cos(8\*pi\*r)/3;  ...  
\>   pov3d(x,y,z,zoom=5,axis=0,add=povsphere([0,0,0.5],0.1,povlook(green)), ...  
\>     w=500,h=300);


![images/Final%20Projek%20APLIKOM-556.png](images/Final%20Projek%20APLIKOM-556.png)

Dengan metode bayangan canggih dari Povray, sangat sedikit titik yang
dapat menghasilkan permukaan yang sangat halus. Hanya di perbatasan
dan dalam bayang-bayang triknya mungkin menjadi jelas.


Untuk ini, kita perlu menambahkan vektor normal di setiap titik
matriks.


\>Z &= 4\*x^2\*y^3


    
                                      2  3
                                   4 x  y
    

Persamaan permukaannya adalah [x,y,Z]. Kami menghitung dua turunan ke
x dan y ini dan mengambil produk silang sebagai normal.


\>dx &= diff([x,y,Z],x); dy &= diff([x,y,Z],y);


Kami mendefinisikan normal sebagai produk silang dari turunan ini, dan
mendefinisikan fungsi koordinat.


\>N &= crossproduct(dx,dy); NX &= N[1]; NY &= N[2]; NZ &= N[3]; N,


    
                                  3        2  2
                          [- 8 x y , - 12 x  y , 1]
    

Kami hanya menggunakan 25 poin.


\>x=-1:0.5:1; y=x';

\>pov3d(x,y,Z(x,y),angle=10°, ...  
\>     xv=NX(x,y),yv=NY(x,y),zv=NZ(x,y),<shadow);


![images/Final%20Projek%20APLIKOM-557.png](images/Final%20Projek%20APLIKOM-557.png)

Berikut ini adalah simpul Trefoil yang dilakukan oleh A. Busser di
Povray. Ada versi yang ditingkatkan dari ini dalam contoh.


  <a href="Contoh\Trefoil Simpul.html">Simpul trefoil</a>  

Untuk tampilan yang bagus dengan tidak terlalu banyak titik, kami
menambahkan vektor normal di sini. Kami menggunakan Maxima untuk
menghitung normal bagi kami. Pertama, ketiga fungsi koordinat sebagai
ekspresi simbolik.


\>X &= ((4+sin(3\*y))+cos(x))\*cos(2\*y); ...  
\>   Y &= ((4+sin(3\*y))+cos(x))\*sin(2\*y); ...  
\>   Z &= sin(x)+2\*cos(3\*y);


Kemudian kedua vektor turunan ke x dan y.


\>dx &= diff([X,Y,Z],x); dy &= diff([X,Y,Z],y);


Sekarang normal, yang merupakan produk silang dari dua turunan.


\>dn &= crossproduct(dx,dy);


Kami sekarang mengevaluasi semua ini secara numerik.


\>x:=linspace(-%pi,%pi,40); y:=linspace(-%pi,%pi,100)';


Vektor normal adalah evaluasi dari ekspresi simbolik dn[i] untuk
i=1,2,3. Sintaks untuk ini adalah &amp;"expression"(parameters). Ini
adalah alternatif dari metode pada contoh sebelumnya, di mana kita
mendefinisikan ekspresi simbolik NX, NY, NZ terlebih dahulu.


\>pov3d(X(x,y),Y(x,y),Z(x,y),axis=0,zoom=5,w=450,h=350, ...  
\>     <shadow,look=povlook(gray), ...  
\>     xv=&"dn[1]"(x,y), yv=&"dn[2]"(x,y), zv=&"dn[3]"(x,y));


![images/Final%20Projek%20APLIKOM-558.png](images/Final%20Projek%20APLIKOM-558.png)

Kami juga dapat menghasilkan grid dalam 3D.


\>povstart(zoom=4); ...  
\>   x=-1:0.5:1; r=1-(x+1)^2/6; ...  
\>   t=(0°:30°:360°)'; y=r\*cos(t); z=r\*sin(t); ...  
\>   writeln(povgrid(x,y,z,d=0.02,dballs=0.05)); ...  
\>   povend();


![images/Final%20Projek%20APLIKOM-559.png](images/Final%20Projek%20APLIKOM-559.png)

With povgrid(), curves are possible.


\>povstart(center=[0,0,1],zoom=3.6); ...  
\>   t=linspace(0,2,1000); r=exp(-t); ...  
\>   x=cos(2\*pi\*10\*t)\*r; y=sin(2\*pi\*10\*t)\*r; z=t; ...  
\>   writeln(povgrid(x,y,z,povlook(red))); ...  
\>   writeAxis(0,2,axis=3); ...  
\>   povend();


![images/Final%20Projek%20APLIKOM-560.png](images/Final%20Projek%20APLIKOM-560.png)

# Latihan Soal

1. Buatlah plot 3D dari fungsi


$$f(x,y)=x^3+3y^2$$

dengan zoom 3 dan angle 55 derajat menggunakan povray


\>pov3d("x^3+3\*y^2",zoom=3,angle=55°);


![images/Final%20Projek%20APLIKOM-562.png](images/Final%20Projek%20APLIKOM-562.png)

2. Buatlah gabungan 2 silinder dengan fungsi povx() berwarna merah dan
povz() berwarna kuning dan zoom 4


\>povstart(zoom=4)

\>c1 = povcylinder (-povx,povx,1,povlook(red));

\>c2 = povcylinder (-povz,povz,1,povlook(yellow));

\>writeln(povintersection([c1,c2]));

\>povend();


![images/Final%20Projek%20APLIKOM-563.png](images/Final%20Projek%20APLIKOM-563.png)

\> 


3. Buatlah grafik 3D dari fungsi kuadrat berikut ini dengan parameter
tambahan:


$$z=4x^2-2y^2$$

Tampilkan grafik tersebut dengan transparent, dan menggunakan grid
dengan resolusi 50, dengan warna biru pada garis di plot tersebut


\>plot3d("4\*x^2-2\*y^2",\>transparent,grid=50,wirecolor=blue):


![images/Final%20Projek%20APLIKOM-565.png](images/Final%20Projek%20APLIKOM-565.png)

# Visualisasi dan Perhitungan Geometri dengan EMT

Euler menyediakan beberapa fungsi untuk melakukan visualisasi dan
perhitungan geometri, baik secara numerik maupun analitik (seperti
biasanya tentunya, menggunakan Maxima). Fungsi-fungsi untuk
visualisasi dan perhitungan geometeri tersebut disimpan di dalam file
program "geometry.e", sehingga file tersebut harus dipanggil sebelum
menggunakan fungsi-fungsi atau perintah-perintah untuk geometri.


\>load geometry


    Numerical and symbolic geometry.

## Fungsi-fungsi Geometri

Fungsi-fungsi untuk Menggambar Objek Geometri:


  defaultd:=textheight()*1.5: nilai asli untuk parameter d  
  setPlotrange(x1,x2,y1,y2): menentukan rentang x dan y pada bidang  

koordinat


  setPlotRange(r): pusat bidang koordinat (0,0) dan batas-batas
sumbu-x dan y adalah -r sd r


  plotPoint (P, "P"): menggambar titik P dan diberi label "P"


  plotSegment (A,B, "AB", d): menggambar ruas garis AB, diberi label
"AB" sejauh d


  plotLine (g, "g", d): menggambar garis g diberi label "g" sejauh d


  plotCircle (c,"c",v,d): Menggambar lingkaran c dan diberi label "c"


  plotLabel (label, P, V, d): menuliskan label pada posisi P


Fungsi-fungsi Geometri Analitik (numerik maupun simbolik):


  turn(v, phi): memutar vektor v sejauh phi  
  turnLeft(v):   memutar vektor v ke kiri  
  turnRight(v):  memutar vektor v ke kanan  
  normalize(v): normal vektor v  
  crossProduct(v, w): hasil kali silang vektorv dan w.  
  lineThrough(A, B): garis melalui A dan B, hasilnya [a,b,c] sdh.  

ax+by=c.


  lineWithDirection(A,v): garis melalui A searah vektor v


  getLineDirection(g): vektor arah (gradien) garis g


  getNormal(g): vektor normal (tegak lurus) garis g


  getPointOnLine(g):  titik pada garis g


  perpendicular(A, g):  garis melalui A tegak lurus garis g


  parallel (A, g):  garis melalui A sejajar garis g


  lineIntersection(g, h):  titik potong garis g dan h


  projectToLine(A, g):   proyeksi titik A pada garis g


  distance(A, B):  jarak titik A dan B


  distanceSquared(A, B):  kuadrat jarak A dan B


  quadrance(A, B): kuadrat jarak A dan B


  areaTriangle(A, B, C):  luas segitiga ABC


  computeAngle(A, B, C):   besar sudut &lt;ABC


  angleBisector(A, B, C): garis bagi sudut &lt;ABC


  circleWithCenter (A, r): lingkaran dengan pusat A dan jari-jari r


  getCircleCenter(c):  pusat lingkaran c


  getCircleRadius(c):  jari-jari lingkaran c


  circleThrough(A,B,C):  lingkaran melalui A, B, C


  middlePerpendicular(A, B): titik tengah AB


  lineCircleIntersections(g, c): titik potong garis g dan lingkran c


  circleCircleIntersections (c1, c2):  titik potong lingkaran c1 dan
c2


  planeThrough(A, B, C):  bidang melalui titik A, B, C


Fungsi-fungsi Khusus Untuk Geometri Simbolik:


  getLineEquation (g,x,y): persamaan garis g dinyatakan dalam x dan y  
  getHesseForm (g,x,y,A): bentuk Hesse garis g dinyatakan dalam x dan  

y dengan titik A pada


  sisi positif (kanan/atas) garis


  quad(A,B): kuadrat jarak AB


  spread(a,b,c): Spread segitiga dengan panjang sisi-sisi a,b,c, yakni
sin(alpha)^2 dengan


  alpha sudut yang menghadap sisi a.


  crosslaw(a,b,c,sa): persamaan 3 quads dan 1 spread pada segitiga
dengan panjang sisi a, b, c.


  triplespread(sa,sb,sc): persamaan 3 spread sa,sb,sc yang memebntuk
suatu segitiga


  doublespread(sa): Spread sudut rangkap Spread 2*phi, dengan
sa=sin(phi)^2 spread a.


## Contoh 1: Luas, Lingkaran Luar, Lingkaran Dalam Segitiga

Untuk menggambar objek-objek geometri, langkah pertama adalah
menentukan rentang sumbu-sumbu koordinat. Semua objek geometri akan
digambar pada satu bidang koordinat, sampai didefinisikan bidang
koordinat yang baru.


\>setPlotRange(-0.5,2.5,-0.5,2.5); // mendefinisikan bidang koordinat baru 


Sekarang tetapkan tiga poin dan plot.


\>A=[1,0]; plotPoint(A,"A"); // definisi dan gambar tiga titik

\>B=[0,1]; plotPoint(B,"B");

\>C=[2,2]; plotPoint(C,"C");


Kemudian untuk tiga segmen.


\>plotSegment(A,B,"c"); // c=AB

\>plotSegment(B,C,"a"); // a=BC

\>plotSegment(A,C,"b"); // b=AC


Fungsi geometri mencakup fungsi untuk membuat garis dan lingkaran.
Format untuk garis adalah [a,b,c], yang mewakili garis dengan
persamaan ax+by=c.


\>lineThrough(B,C) // garis yang melalui B dan C


    [-1,  2,  2]

Hitung garis tegak lurus melalui A pada BC.


\>h=perpendicular(A,lineThrough(B,C)); // garis h tegak lurus BC melalui A


Dan persimpangan dengan BC.


\>D=lineIntersection(h,lineThrough(B,C)); // D adalah titik potong h dan BC


Plot that.


\>plotPoint(D,value=1); // koordinat D ditampilkan

\>aspect(1); plotSegment(A,D): // tampilkan semua gambar hasil plot...()


![images/Final%20Projek%20APLIKOM-566.png](images/Final%20Projek%20APLIKOM-566.png)

Hitung luas ABC:


$$L_{\triangle ABC}= \frac{1}{2}AD.BC.$$\>norm(A-D)\*norm(B-C)/2 // AD=norm(A-D), BC=norm(B-C)


    1.5

Bandingkan dengan rumus determinan.


\>areaTriangle(A,B,C) // hitung luas segitiga langusng dengan fungsi


    1.5

Cara lain menghitung luas segitigas ABC:


\>distance(A,D)\*distance(B,C)/2


    1.5

Sudut di C.


\>degprint(computeAngle(B,C,A))


    36°52'11.63''

Kemudian menggambarkan lingkaran luar segitiga.


\>c=circleThrough(A,B,C); // lingkaran luar segitiga ABC

\>R=getCircleRadius(c); // jari2 lingkaran luar 

\>O=getCircleCenter(c); // titik pusat lingkaran c 

\>plotPoint(O,"O"); // gambar titik "O"

\>plotCircle(c,"Lingkaran luar segitiga ABC"):


![images/Final%20Projek%20APLIKOM-568.png](images/Final%20Projek%20APLIKOM-568.png)

Tampilkan koordinat titik pusat dan jari-jari lingkaran luar.


\>O, R


    [1.16667,  1.16667]
    1.17851130198

Sekarang akan digambar lingkaran dalam segitiga ABC. Titik pusat
lingkaran dalam adalah titik potong garis-garis bagi sudut.


\>l=angleBisector(A,C,B); // garis bagi <ACB

\>g=angleBisector(C,A,B); // garis bagi <CAB

\>P=lineIntersection(l,g) // titik potong kedua garis bagi sudut


    [0.86038,  0.86038]

Tambahkan semuanya ke plot.


\>color(5); plotLine(l); plotLine(g); color(1); // gambar kedua garis bagi sudut

\>plotPoint(P,"P"); // gambar titik potongnya

\>r=norm(P-projectToLine(P,lineThrough(A,B))) // jari-jari lingkaran dalam


    0.509653732104

\>plotCircle(circleWithCenter(P,r),"Lingkaran dalam segitiga ABC"): // gambar lingkaran dalam


![images/Final%20Projek%20APLIKOM-569.png](images/Final%20Projek%20APLIKOM-569.png)

## Latihan

1. Tentukan ketiga titik singgung lingkaran dalam dengan sisi-sisi
segitiga ABC.


\>setPlotRange(-3.5,5.5,-3.5,5.5);

\>A=[-3,1]; plotPoint(A,"A");

\>B=[1,-3]; plotPoint(B,"B");

\>C=[5,5]; plotPoint(C,"C");


2. Gambar segitiga dengan titik-titik sudut ketiga titik singgung
tersebut. Merupakan segitiga apakah itu?


\>plotSegment(A,B,"c")

\>plotSegment(B,C,"a")

\>plotSegment(A,C,"b")

\>aspect(1):


![images/Final%20Projek%20APLIKOM-570.png](images/Final%20Projek%20APLIKOM-570.png)

3. Hitung luas segitiga tersebut.


\>lineThrough(A,B)


    [4,  4,  -8]

\>h=perpendicular(C,lineThrough(A,B));

\>D=lineIntersection(h,lineThrough(A,B));

\>plotPoint(D,value=1);

\>aspect(1); plotSegment(C,D):


![images/Final%20Projek%20APLIKOM-571.png](images/Final%20Projek%20APLIKOM-571.png)

\>distance(C,D)\*distance(A,B)/2


    24

Jadi luas segitiga di atas adalah 24


4. Tunjukkan bahwa garis bagi sudut yang ke tiga juga melalui titik
pusat lingkaran dalam.


\>l=angleBisector(A,C,B);

\>g=angleBisector(C,A,B);

\>P=lineIntersection(l,g)


    [0.441518,  0.441518]

\>color(5); plotLine(l); plotLine(g); color(1);

\>plotPoint(P,"P");

\>r=norm(P-projectToLine(P,lineThrough(A,B)))


    2.03861492842

\>plotCircle(circleWithCenter(P,r),"Lingkaran dalam segitiga ABC"):


![images/Final%20Projek%20APLIKOM-572.png](images/Final%20Projek%20APLIKOM-572.png)

Jadi, terbukti bahwa garis bagi sudut yang ketiga juga melalui titik
pusat lingkaran dalam.


5. Gambar jari-jari lingkaran dalam.


\>r=norm(P-projectToLine(P,lineThrough(A,B)))


    2.03861492842

\>plotCircle(circleWithCenter(P,r),"Lingkaran dalam segitiga ABC"):


![images/Final%20Projek%20APLIKOM-573.png](images/Final%20Projek%20APLIKOM-573.png)

6. Hitung luas lingkaran luar dan luas lingkaran dalam segitiga ABC.
Adakah hubungan antara luas kedua lingkaran tersebut dengan luas
segitiga ABC?


\>c=circleThrough(A,B,C);

\>R=getCircleRadius(c);

\>O=getCircleCenter(c);

\>plotPoint(O,"O");

\>plotCircle(c,"Lingkaran luar segitiga ABC"):


![images/Final%20Projek%20APLIKOM-574.png](images/Final%20Projek%20APLIKOM-574.png)

## Contoh 2: Geometri Simbolik

Kita dapat menghitung geometri eksak dan simbolik menggunakan Maxima.


File geometri.e menyediakan fungsi yang sama (dan lebih banyak lagi)
di Maxima. Namun, kita dapat menggunakan perhitungan simbolis
sekarang.


\>A &= [1,0]; B &= [0,1]; C &= [2,2]; // menentukan tiga titik A, B, C


Fungsi untuk garis dan lingkaran bekerja seperti fungsi Euler, tetapi
memberikan perhitungan simbolis.


\>c &= lineThrough(B,C) // c=BC


    
                                 [- 1, 2, 2]
    

Kita bisa mendapatkan persamaan garis dengan mudah.


\>$getLineEquation(c,x,y), $solve(%,y) | expand // persamaan garis c


$$2\,y-x=2$$$$\left[ y=\frac{x}{2}+1 \right] $$\>$getLineEquation(lineThrough([x1,y1],[x2,y2]),x,y), $solve(%,y) // persamaan garis melalui(x1, y1) dan (x2, y2)


$$x\,\left({\it y_1}-{\it y_2}\right)+\left(\frac{\sqrt{5}-1}{2}-
 {\it x_1}\right)\,y={\it x_1}\,\left({\it y_1}-{\it y_2}\right)+
 \left(\frac{\sqrt{5}-1}{2}-{\it x_1}\right)\,{\it y_1}$$$$\left[ y=\frac{\left(2\,{\it x_1}-2\,x\right)\,{\it y_2}+\left(2\,x
 -\sqrt{5}+1\right)\,{\it y_1}}{2\,{\it x_1}-\sqrt{5}+1} \right] $$\>$getLineEquation(lineThrough(A,[x1,y1]),x,y) // persamaan garis melalui A dan (x1, y1)


$$\left({\it x_1}-1\right)\,y-x\,{\it y_1}=-{\it y_1}$$\>h &= perpendicular(A,lineThrough(B,C)) // h melalui A tegak lurus BC


    
                                  [2, 1, 2]
    

\>Q &= lineIntersection(c,h) // Q titik potong garis c=BC dan h


    
                                     2  6
                                    [-, -]
                                     5  5
    

\>$projectToLine(A,lineThrough(B,C)) // proyeksi A pada BC


$$\left[ \frac{2}{5} , \frac{6}{5} \right] $$\>$distance(A,Q) // jarak AQ


$$\frac{3}{\sqrt{5}}$$\>cc &= circleThrough(A,B,C); $cc // (titik pusat dan jari-jari) lingkaran melalui A, B, C


$$\left[ \frac{7}{6} , \frac{7}{6} , \frac{5}{3\,\sqrt{2}} \right] $$\>r&=getCircleRadius(cc); $r , $float(r) // tampilkan nilai jari-jari


$$\frac{5}{3\,\sqrt{2}}$$$$1.178511301977579$$\>$computeAngle(A,C,B) // nilai <ACB


$$\arccos \left(\frac{4}{5}\right)$$\>$solve(getLineEquation(angleBisector(A,C,B),x,y),y)[1] // persamaan garis bagi <ACB


$$y=x$$\>P &= lineIntersection(angleBisector(A,C,B),angleBisector(C,B,A)); $P // titik potong 2 garis bagi sudut


$$\left[ \frac{\sqrt{2}\,\sqrt{5}+2}{6} , \frac{\sqrt{2}\,\sqrt{5}+2
 }{6} \right] $$\>P() // hasilnya sama dengan perhitungan sebelumnya


    [0.86038,  0.86038]

## Garis dan Lingkaran yang Berpotongan

Tentu saja, kita juga bisa memotong garis dengan lingkaran, dan
lingkaran dengan lingkaran.


\>A &:= [1,0]; c=circleWithCenter(A,4);

\>B &:= [1,2]; C &:= [2,1]; l=lineThrough(B,C);

\>setPlotRange(5); plotCircle(c); plotLine(l);


Persimpangan garis dengan lingkaran mengembalikan dua titik dan jumlah
titik persimpangan.


\>{P1,P2,f}=lineCircleIntersections(l,c);

\>P1, P2, f


    [4.64575,  -1.64575]
    [-0.645751,  3.64575]
    2

\>plotPoint(P1); plotPoint(P2):


![images/Final%20Projek%20APLIKOM-588.png](images/Final%20Projek%20APLIKOM-588.png)

Begitu pula di Maxima.


\>c &= circleWithCenter(A,4) // lingkaran dengan pusat A jari-jari 4


    
                                  [1, 0, 4]
    

\>l &= lineThrough(B,C) // garis l melalui B dan C


    
                                  [1, 1, 3]
    

\>$lineCircleIntersections(l,c) | radcan, // titik potong lingkaran c dan garis l


$$\left[ \left[ \sqrt{7}+2 , 1-\sqrt{7} \right]  , \left[ 2-\sqrt{7}
  , \sqrt{7}+1 \right]  \right] $$Akan ditunjukkan bahwa sudut-sudut yang menghadap busur yang sama
adalah sama besar.


\>C=A+normalize([-2,-3])\*4; plotPoint(C); plotSegment(P1,C); plotSegment(P2,C);

\>degprint(computeAngle(P1,C,P2))


    69°17'42.68''

\>C=A+normalize([-4,-3])\*4; plotPoint(C); plotSegment(P1,C); plotSegment(P2,C);

\>degprint(computeAngle(P1,C,P2))


    69°17'42.68''

\>insimg;


![images/Final%20Projek%20APLIKOM-590.png](images/Final%20Projek%20APLIKOM-590.png)

## Garis Sumbu

Berikut adalah langkah-langkah menggambar garis sumbu ruas garis AB:


1. Gambar lingkaran dengan pusat A melalui B.


2. Gambar lingkaran dengan pusat B melalui A.


3. Tarik garis melallui kedua titik potong kedua lingkaran tersebut.
Garis ini merupakan garis sumbu (melalui titik tengah dan tegak lurus)
AB.


\>A=[2,2]; B=[-1,-2];

\>c1=circleWithCenter(A,distance(A,B));

\>c2=circleWithCenter(B,distance(A,B));

\>{P1,P2,f}=circleCircleIntersections(c1,c2);

\>l=lineThrough(P1,P2);

\>setPlotRange(5); plotCircle(c1); plotCircle(c2);

\>plotPoint(A); plotPoint(B); plotSegment(A,B); plotLine(l):


![images/Final%20Projek%20APLIKOM-591.png](images/Final%20Projek%20APLIKOM-591.png)

Selanjutnya, kami melakukan hal yang sama di Maxima dengan koordinat
umum.


\>A &= [a1,a2]; B &= [b1,b2];

\>c1 &= circleWithCenter(A,distance(A,B));

\>c2 &= circleWithCenter(B,distance(A,B));

\>P &= circleCircleIntersections(c1,c2); P1 &= P[1]; P2 &= P[2];


Persamaan untuk persimpangan cukup terlibat. Tetapi kita dapat
menyederhanakannya, jika kita memecahkan y.


\>g &= getLineEquation(lineThrough(P1,P2),x,y);

\>$solve(g,y)


$$\left[ y=\frac{-\left(2\,{\it b_1}-2\,{\it a_1}\right)\,x+{\it b_2}
 ^2+{\it b_1}^2-{\it a_2}^2-{\it a_1}^2}{2\,{\it b_2}-2\,{\it a_2}}
  \right] $$Ini memang sama dengan tegak lurus tengah, yang dihitung dengan cara
yang sama sekali berbeda.


\>$solve(getLineEquation(middlePerpendicular(A,B),x,y),y)


$$\left[ y=\frac{-\left(2\,{\it b_1}-2\,{\it a_1}\right)\,x+{\it b_2}
 ^2+{\it b_1}^2-{\it a_2}^2-{\it a_1}^2}{2\,{\it b_2}-2\,{\it a_2}}
  \right] $$\>h &=getLineEquation(lineThrough(A,B),x,y);

\>$solve(h,y)


$$\left[ y=\frac{\left({\it b_2}-{\it a_2}\right)\,x-{\it a_1}\,
 {\it b_2}+{\it a_2}\,{\it b_1}}{{\it b_1}-{\it a_1}} \right] $$Perhatikan hasil kali gradien garis g dan h adalah:


$$\frac{-(b_1-a_1)}{(b_2-a_2)}\times \frac{(b_2-a_2)}{(b_1-a_1)} = -1.$$Artinya kedua garis tegak lurus.


# Contoh 3: Rumus Heron

Rumus Heron menyatakan bahwa luas segitiga dengan panjang sisi-sisi a,
b dan c adalah:


$$L = \sqrt{s(s-a)(s-b)(s-c)}\quad \text{ dengan } s=(a+b+c)/2,$$atau bisa ditulis dalam bentuk lain:


$$L = \frac{1}{4}\sqrt{(a+b+c)(b+c-a)(a+c-b)(a+b-c)}$$Untuk membuktikan hal ini kita misalkan C(0,0), B(a,0) dan A(x,y),
b=AC, c=AB. Luas segitiga ABC adalah


$$L_{\triangle ABC}=\frac{1}{2}a\times y.$$Nilai y didapat dengan menyelesaikan sistem persamaan:


$$x^2+y^2=b^2, \quad (x-a)^2+y^2=c^2.$$\>setPlotRange(-1,10,-1,8); plotPoint([0,0], "C(0,0)"); plotPoint([5.5,0], "B(a,0)");  ...  
\>    plotPoint([7.5,6], "A(x,y)");

\>plotSegment([0,0],[5.5,0], "a",25); plotSegment([5.5,0],[7.5,6],"c",15);  ...  
\>   plotSegment([0,0],[7.5,6],"b",25); 

\>plotSegment([7.5,6],[7.5,0],"t=y",25):


![images/Final%20Projek%20APLIKOM-600.png](images/Final%20Projek%20APLIKOM-600.png)

\>sol &= solve([x^2+y^2=b^2,(x-a)^2+y^2=c^2],[x,y])


    
                                      []
    

\>ysol &= y with sol[2][2]; $'y=sqrt(factor(ysol^2))


    Maxima said:
    part: invalid index of list or matrix.
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    ysol &amp;= y with sol[2][2]; $'y=sqrt(factor(ysol^2)) ...
                            ^

Kami mendapatkan formula Heron.


\>function H(a,b,c) &= sqrt(factor((ysol\*a/2)^2)); $'H(a,b,c)=H(a,b,c)


$$H\left(a , b , \left[ 1 , 0 , 4 \right] \right)=\frac{\left| a
 \right| \,\left| {\it ysol}\right| }{2}$$\>$'Luas=H(2,5,6) // luas segitiga dengan panjang sisi-sisi 2, 5, 6


$${\it Luas}=\left| {\it ysol}\right| $$Tentu saja, setiap segitiga persegi panjang adalah kasus yang
terkenal.


\>$H(3,4,5) //luas segitiga siku-siku dengan panjang sisi 3, 4, 5


$$\frac{3\,\left| {\it ysol}\right| }{2}$$Dan juga jelas, bahwa ini adalah segitiga dengan luas maksimal dan dua
sisi 3 dan 4.


\>aspect (1.5); plot2d($H(3,4,x),1,7): // Kurva luas segitiga sengan panjang sisi 3, 4, x (1<= x <=7)


    Variable or function ysol not found.
    Error in expression: 3*abs(ysol)/2
    %ploteval:
        y0=f$(x[1],args());
    adaptiveevalone:
        s=%ploteval(g$,t;args());
    Try "trace errors" to inspect local variables after errors.
    plot2d:
        dw/n,dw/n^2,dw/n,auto;args());

Kasus umum juga berhasil.


\>$solve(diff(H(a,b,c)^2,c)=0,c)


    Maxima said:
    diff: second argument must be a variable; found [1,0,4]
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    $solve(diff(H(a,b,c)^2,c)=0,c) ...
                                  ^

Sekarang mari kita temukan himpunan semua titik di mana b+c=d untuk
beberapa konstanta d. Diketahui bahwa ini adalah elips.


\>s1 &= subst(d-c,b,sol[2]); $s1


    Maxima said:
    part: invalid index of list or matrix.
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    s1 &amp;= subst(d-c,b,sol[2]); $s1 ...
                             ^

And make functions of this.


\>function fx(a,c,d) &= rhs(s1[1]); $fx(a,c,d), function fy(a,c,d) &= rhs(s1[2]); $fy(a,c,d)


$$0$$$$0$$Sekarang kita bisa menggambar set. Sisi b bervariasi dari 1 hingga 4.
Sudah diketahui bahwa kita mendapatkan elips.


Kita dapat memeriksa persamaan umum untuk elips ini, i.e.


dimana (xm,ym) adalah pusatnya, dan u dan v adalah setengah sumbu.


\>$ratsimp((fx(a,c,d)-a/2)^2/u^2+fy(a,c,d)^2/v^2 with [u=d/2,v=sqrt(d^2-a^2)/2])


$$\left[ \frac{a^2}{d^2} , \frac{a^2}{d^2} , \frac{a^2}{d^2} , \frac{
 a^2}{d^2} , \frac{a^2}{d^2} , \frac{a^2}{d^2} , \frac{a^2}{d^2} , 
 \frac{a^2}{d^2} , \frac{a^2}{d^2} , \frac{a^2}{d^2} , \frac{a^2}{d^2
 } \right] $$Kita melihat bahwa tinggi dan dengan demikian luas segitiga adalah
maksimum untuk x=0. Dengan demikian luas segitiga dengan a+b+c=d
adalah maksimal, jika sama sisi. Kami ingin menurunkan ini secara
analitis.


\>eqns &= [diff(H(a,b,d-(a+b))^2,a)=0,diff(H(a,b,d-(a+b))^2,b)=0]; $eqns


$$\left[ \frac{a\,{\it ysol}^2}{2}=0 , 0=0 \right] $$Kita mendapatkan beberapa minimum, yang termasuk segitiga dengan satu
sisi 0, dan solusi a=b=c=d/3.


\>$solve(eqns,[a,b])


$$\left[ \left[ a=0 , b={\it \%r_1} \right]  \right] $$Ada juga metode Lagrange, memaksimalkan H(a,b,c)^2 sehubungan dengan
a+b+d=d.


\>&solve([diff(H(a,b,c)^2,a)=la,diff(H(a,b,c)^2,b)=la, ...  
\>      diff(H(a,b,c)^2,c)=la,a+b+c=d],[a,b,c,la])


    Maxima said:
    diff: second argument must be a variable; found [1,0,4]
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    ... la,    diff(H(a,b,c)^2,c)=la,a+b+c=d],[a,b,c,la]) ...
                                                         ^

Kita bisa membuat plot situasinya


First set the points in Maxima.


\>A &= at([x,y],sol[2]); $A


    Maxima said:
    part: invalid index of list or matrix.
     -- an error. To debug this try: debugmode(true);
    
    Error in:
    A &amp;= at([x,y],sol[2]); $A ...
                         ^

\>B &= [0,0]; $B, C &= [a,0]; $C


$$\left[ 0 , 0 \right] $$$$\left[ a , 0 \right] $$Kemudian atur rentang plot, dan plot poinnya.


\>setPlotRange(0,5,-2,3); ...  
\>   a=4; b=3; c=2; ...  
\>   plotPoint(mxmeval("B"),"B"); plotPoint(mxmeval("C"),"C"); ...  
\>   plotPoint(mxmeval("A"),"A"):


    Variable a1 not found!
    Use global variables or parameters for string evaluation.
    Error in Evaluate, superfluous characters found.
    Try "trace errors" to inspect local variables after errors.
    mxmeval:
        return evaluate(mxm(s));
    Error in:
    ... otPoint(mxmeval("C"),"C"); plotPoint(mxmeval("A"),"A"): ...
                                                         ^

Plot the segments.


\>plotSegment(mxmeval("A"),mxmeval("C")); ...  
\>   plotSegment(mxmeval("B"),mxmeval("C")); ...  
\>   plotSegment(mxmeval("B"),mxmeval("A")):


    Variable a1 not found!
    Use global variables or parameters for string evaluation.
    Error in Evaluate, superfluous characters found.
    Try "trace errors" to inspect local variables after errors.
    mxmeval:
        return evaluate(mxm(s));
    Error in:
    plotSegment(mxmeval("A"),mxmeval("C")); plotSegment(mxmeval("B ...
                            ^

CompHitung tengah tegak lurus di Maxima.


\>h &= middlePerpendicular(A,B); g &= middlePerpendicular(B,C);


Dan pusat keliling.


\>U &= lineIntersection(h,g);


Kita mendapatkan rumus untuk jari-jari lingkaran melingkar.


\>&assume(a\>0,b\>0,c\>0); $distance(U,B) | radcan


$$\frac{\sqrt{{\it a_2}^2+{\it a_1}^2}\,\sqrt{{\it a_2}^2+{\it a_1}^2
 -2\,a\,{\it a_1}+a^2}}{2\,\left| {\it a_2}\right| }$$Mari kita tambahkan ini ke plot.


\>plotPoint(U()); ...  
\>   plotCircle(circleWithCenter(mxmeval("U"),mxmeval("distance(U,C)"))):


    Variable a2 not found!
    Use global variables or parameters for string evaluation.
    Error in ^
    Error in expression: [a/2,(a2^2+a1^2-a*a1)/(2*a2)]
    Error in:
    plotPoint(U()); plotCircle(circleWithCenter(mxmeval("U"),mxmev ...
                 ^

Dengan menggunakan geometri, kita mendapatkan rumus sederhana


untuk radius. Kita dapat memeriksa, apakah ini benar-benar benar
dengan Maxima. Maxima akan memperhitungkan ini hanya jika kita
mengkutududukkannya.


\>$c^2/sin(computeAngle(A,B,C))^2  | factor


$$\left[ \frac{{\it a_2}^2+{\it a_1}^2}{{\it a_2}^2} , 0 , \frac{16\,
 \left({\it a_2}^2+{\it a_1}^2\right)}{{\it a_2}^2} \right] $$# Contoh 4: Garis Euler dan Parabola

Garis Euler adalah garis yang ditentukan dari segitiga apa pun yang
tidak sama sisi. Ini adalah garis tengah segitiga, dan melewati
beberapa titik penting yang ditentukan dari segitiga, termasuk
ortosentrum, pusat lilitan, centroid, titik Exeter dan pusat lingkaran
sembilan titik segitiga.


Untuk demonstrasi, kita menghitung dan memplot garis Euler dalam
segitiga.


Pertama, kita mendefinisikan sudut segitiga di Euler. Kami menggunakan
definisi, yang terlihat dalam ekspresi simbolis.


\>A::=[-1,-1]; B::=[2,0]; C::=[1,2];


Untuk memplot objek geometris, kita mengatur area plot, dan
menambahkan titik-titik ke dalamnya. Semua plot objek geometris
ditambahkan ke plot saat ini.


\>setPlotRange(3); plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C");


Kita juga bisa menambahkan sisi segitiga.


\>plotSegment(A,B,""); plotSegment(B,C,""); plotSegment(C,A,""):


![images/Final%20Projek%20APLIKOM-613.png](images/Final%20Projek%20APLIKOM-613.png)

Berikut adalah luas segitiga, menggunakan rumus penentu. Tentu saja,
kita harus mengambil nilai absolut dari hasil ini.


\>$areaTriangle(A,B,C)


$$-\frac{7}{2}$$Kita dapat menghitung koefisien sisi c.


\>c &= lineThrough(A,B)


    
                                [- 1, 3, - 2]
    

Dan juga dapatkan rumus untuk baris ini.


\>$getLineEquation(c,x,y)


$$3\,y-x=-2$$Untuk bentuk Hesse, kita perlu menentukan titik, sehingga titik
tersebut berada di sisi positif dari Hesseform. Memasukkan titik
menghasilkan jarak positif ke garis.


\>$getHesseForm(c,x,y,C), $at(%,[x=C[1],y=C[2]])


$$\frac{3\,y-x+2}{\sqrt{10}}$$$$\frac{7}{\sqrt{10}}$$Sekarang kita menghitung lingkaran lingkaran ABC.


\>LL &= circleThrough(A,B,C); $getCircleEquation(LL,x,y)


$$\left(y-\frac{5}{14}\right)^2+\left(x-\frac{3}{14}\right)^2=\frac{
 325}{98}$$\>O &= getCircleCenter(LL); $O


$$\left[ \frac{3}{14} , \frac{5}{14} \right] $$Plot lingkaran dan pusatnya. Cu dan Anda simbolis. Kami mengevaluasi
ekspresi ini untuk Euler.


\>plotCircle(LL()); plotPoint(O(),"O"):


![images/Final%20Projek%20APLIKOM-620.png](images/Final%20Projek%20APLIKOM-620.png)

Kita dapat menghitung persimpangan ketinggian di ABC (ortosent) secara
numerik dengan perintah berikut.


\>H &= lineIntersection(perpendicular(A,lineThrough(C,B)),...  
\>     perpendicular(B,lineThrough(A,C))); $H


$$\left[ \frac{11}{7} , \frac{2}{7} \right] $$Sekarang kita dapat menghitung garis Euler dari segitiga.


\>el &= lineThrough(H,O); $getLineEquation(el,x,y)


$$-\frac{19\,y}{14}-\frac{x}{14}=-\frac{1}{2}$$Tambahkan ke plot kita.


\>plotPoint(H(),"H"); plotLine(el(),"Garis Euler"):


![images/Final%20Projek%20APLIKOM-623.png](images/Final%20Projek%20APLIKOM-623.png)

Pusat gravitasi harus berada di garis ini.


\>M &= (A+B+C)/3; $getLineEquation(el,x,y) with [x=M[1],y=M[2]]


$$-\frac{1}{2}=-\frac{1}{2}$$\>plotPoint(M(),"M"): // titik berat


![images/Final%20Projek%20APLIKOM-625.png](images/Final%20Projek%20APLIKOM-625.png)

Teorinya memberitahu kita MH=2*MO. Kita perlu menyederhanakan dengan
radcan untuk mencapai ini.


\>$distance(M,H)/distance(M,O)|radcan


$$2$$Fungsi termasuk fungsi untuk sudut juga.


\>$computeAngle(A,C,B), degprint(%())


$$\arccos \left(\frac{4}{\sqrt{5}\,\sqrt{13}}\right)$$    60°15'18.43''

Persamaan untuk pusat incircle tidak terlalu bagus.


\>Q &= lineIntersection(angleBisector(A,C,B),angleBisector(C,B,A))|radcan; $Q


$$\left[ \frac{\left(2^{\frac{3}{2}}+1\right)\,\sqrt{5}\,\sqrt{13}-15
 \,\sqrt{2}+3}{14} , \frac{\left(\sqrt{2}-3\right)\,\sqrt{5}\,\sqrt{
 13}+5\,2^{\frac{3}{2}}+5}{14} \right] $$Mari kita hitung juga ekspresi untuk jari-jari lingkaran yang
tertulis.


\>r &= distance(Q,projectToLine(Q,lineThrough(A,B)))|ratsimp; $r


$$\frac{\sqrt{\left(-41\,\sqrt{2}-31\right)\,\sqrt{5}\,\sqrt{13}+115
 \,\sqrt{2}+614}}{7\,\sqrt{2}}$$\>LD &=  circleWithCenter(Q,r); // Lingkaran dalam


Mari kita tambahkan ini ke plot.


\>color(5); plotCircle(LD()):


![images/Final%20Projek%20APLIKOM-630.png](images/Final%20Projek%20APLIKOM-630.png)

## Parabola

Selanjutnya akan dicari persamaan tempat kedudukan titik-titik yang berjarak sama ke titik C
dan ke garis AB.


\>p &= getHesseForm(lineThrough(A,B),x,y,C)-distance([x,y],C); $p='0


$$\frac{3\,y-x+2}{\sqrt{10}}-\sqrt{\left(2-y\right)^2+\left(1-x
 \right)^2}=0$$Persamaan tersebut dapat digambar menjadi satu dengan gambar sebelumnya.


\>plot2d(p,level=0,add=1,contourcolor=6):


![images/Final%20Projek%20APLIKOM-632.png](images/Final%20Projek%20APLIKOM-632.png)

Ini seharusnya menjadi beberapa fungsi, tetapi pemecah default Maxima
hanya dapat menemukan solusinya, jika kita kuadratkan persamaannya.
Akibatnya, kami mendapatkan solusi palsu.


\>akar &= solve(getHesseForm(lineThrough(A,B),x,y,C)^2-distance([x,y],C)^2,y)


    
            [y = - 3 x - sqrt(70) sqrt(9 - 2 x) + 26, 
                                  y = - 3 x + sqrt(70) sqrt(9 - 2 x) + 26]
    

Solusi pertama adalah


maxima: akar[1]


Menambahkan solusi pertama ke plot menunjukkan, bahwa itu memang jalan
yang kita cari. Teorinya memberi tahu kita bahwa itu adalah parabola
yang diputar.


\>plot2d(&rhs(akar[1]),add=1):


![images/Final%20Projek%20APLIKOM-633.png](images/Final%20Projek%20APLIKOM-633.png)

\>function g(x) &= rhs(akar[1]); $'g(x)= g(x)// fungsi yang mendefinisikan kurva di atas


$$g\left(x\right)=-3\,x-\sqrt{70}\,\sqrt{9-2\,x}+26$$\>T &=[-1, g(-1)]; // ambil sebarang titik pada kurva tersebut

\>dTC &= distance(T,C); $fullratsimp(dTC), $float(%) // jarak T ke C


$$\sqrt{1503-54\,\sqrt{11}\,\sqrt{70}}$$$$2.135605779339061$$\>U &= projectToLine(T,lineThrough(A,B)); $U // proyeksi T pada garis AB 


$$\left[ \frac{80-3\,\sqrt{11}\,\sqrt{70}}{10} , \frac{20-\sqrt{11}\,
 \sqrt{70}}{10} \right] $$\>dU2AB &= distance(T,U); $fullratsimp(dU2AB), $float(%) // jatak T ke AB


$$\sqrt{1503-54\,\sqrt{11}\,\sqrt{70}}$$$$2.135605779339061$$Ternyata jarak T ke C sama dengan jarak T ke AB. Coba Anda pilih titik T yang lain dan
ulangi perhitungan-perhitungan di atas untuk menunjukkan bahwa hasilnya juga sama.


# Contoh 5: Trigonometri Rasional

Ini terinspirasi oleh sebuah pembicaraan N.J.Wildberger. Dalam bukunya
"Divine Proportions", Wildberger mengusulkan untuk mengganti gagasan
klasik tentang jarak dan sudut dengan segi empat dan penyebaran.
Dengan menggunakan ini, memang mungkin untuk menghindari fungsi
trigonometri dalam banyak contoh, dan tetap "rasional".


Berikut ini, saya memperkenalkan konsep, dan memecahkan beberapa
masalah. Saya menggunakan perhitungan simbolik Maxima di sini, yang
menyembunyikan keuntungan utama dari trigonometri rasional bahwa
perhitungan dapat dilakukan hanya dengan kertas dan pensil. Anda
diundang untuk memeriksa hasilnya tanpa komputer.


Intinya adalah bahwa perhitungan rasional simbolik sering kali
menghasilkan hasil yang sederhana. Sebaliknya, trigonometri klasik
menghasilkan hasil trigonometri yang rumit, yang mengevaluasi
perkiraan numerik saja.


\>load geometry;


Untuk perkenalan pertama, kami menggunakan segitiga persegi panjang
dengan proporsi Mesir yang terkenal 3, 4 dan 5. Perintah berikut
adalah perintah Euler untuk memplot geometri bidang yang terkandung
dalam file Euler "geometry.e".


\>C&:=[0,0]; A&:=[4,0]; B&:=[0,3]; ...  
\>   setPlotRange(-1,5,-1,5); ...  
\>   plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); ...  
\>   plotSegment(B,A,"c"); plotSegment(A,C,"b"); plotSegment(C,B,"a"); ...  
\>   insimg(30);


![images/Final%20Projek%20APLIKOM-640.png](images/Final%20Projek%20APLIKOM-640.png)

Tentu,


di mana wa adalah sudut pada A. Cara biasa untuk menghitung sudut ini,
adalah dengan mengambil kebalikan dari fungsi sinus. Hasilnya adalah
sudut yang tidak dapat dicerna, yang hanya dapat dicetak kira-kira.


\>wa := arcsin(3/5); degprint(wa)


    36°52'11.63''

Trigonometri rasional mencoba menghindari hal ini.


Gagasan pertama dari trigonometri rasional adalah segi empat, yang
menggantikan jarak. Faktanya, itu hanya jarak kuadrat. Berikut ini, a,
b, dan c menunjukkan segi empat sisi.


Teorema Pythogoras hanya menjadi a+b=c kemudian.


\>a &= 3^2; b &= 4^2; c &= 5^2; &a+b=c


    
                                   25 = 25
    

Gagasan kedua dari trigonometri rasional adalah penyebaran. Spread
mengukur pembukaan antar garis. Ini adalah 0, jika garisnya sejajar,
dan 1, jika garisnya persegi panjang. Ini adalah kuadrat sinus dari
sudut antara dua garis.


Penyebaran garis AB dan AC pada gambar di atas didefinisikan
sebagaithe lines AB and AC in the image above is defined as


di mana a dan c adalah kuadrat dari segitiga persegi panjang dengan
satu sudut di A.


\>sa &= a/c; $sa


$$\frac{9}{25}$$Ini lebih mudah dihitung daripada sudut, tentu saja. Tetapi Anda
kehilangan properti bahwa sudut dapat ditambahkan dengan mudah.


Tentu saja, kita dapat mengonversi nilai perkiraan kita untuk sudut wa
menjadi sprad, dan mencetaknya sebagai pecahan.


\>fracprint(sin(wa)^2)


    9/25

Hukum kosinus trgonometri klasik diterjemahkan menjadi berikut "cross
law".


Di sini a, b, dan c adalah segi empat dari sisi-sisi segitiga, dan sa
adalah penyebaran di sudut A. Sisi a, seperti biasa, berlawanan dengan
sudut A.


Hukum ini diimplementasikan dalam file geometri.e yang kita muat ke
Euler.


\>$crosslaw(aa,bb,cc,saa)


$$\left[ \left({\it bb}-{\it aa}+\frac{7}{6}\right)^2 , \left(
 {\it bb}-{\it aa}+\frac{7}{6}\right)^2 , \left({\it bb}-{\it aa}+
 \frac{5}{3\,\sqrt{2}}\right)^2 \right] =\left[ \frac{14\,{\it bb}\,
 \left(1-{\it saa}\right)}{3} , \frac{14\,{\it bb}\,\left(1-{\it saa}
 \right)}{3} , \frac{5\,2^{\frac{3}{2}}\,{\it bb}\,\left(1-{\it saa}
 \right)}{3} \right] $$Dalam kasus kami, kami mendapatkan


\>$crosslaw(a,b,c,sa)


$$1024=1024$$Mari kita gunakan crosslaw ini untuk menemukan penyebaran di A. Untuk
melakukan ini, kami menghasilkan crosslaw untuk segi empat a, b, dan
c, dan menyelesaikannya untuk spread sa yang tidak diketahui.


Anda dapat melakukan ini dengan tangan dengan mudah, tetapi saya
menggunakan Maxima. Tentu saja, kami mendapatkan hasilnya, kami sudah
memilikinya.


\>$crosslaw(a,b,c,x), $solve(%,x)


$$1024=1600\,\left(1-x\right)$$$$\left[ x=\frac{9}{25} \right] $$Kami sudah tahu ini. Definisi spread adalah kasus khusus dari
crosslaw.


Kita juga dapat menyelesaikan ini untuk umum a, b, c. Hasilnya adalah
rumus yang menghitung penyebaran sudut segitiga yang diberikan segi
empat dari tiga sisi.


\>$solve(crosslaw(aa,bb,cc,x),x)


$$\left[ \left[ \frac{168\,{\it bb}\,x+36\,{\it bb}^2+\left(-72\,
 {\it aa}-84\right)\,{\it bb}+36\,{\it aa}^2-84\,{\it aa}+49}{36} , 
 \frac{168\,{\it bb}\,x+36\,{\it bb}^2+\left(-72\,{\it aa}-84\right)
 \,{\it bb}+36\,{\it aa}^2-84\,{\it aa}+49}{36} , \frac{15\,2^{\frac{
 5}{2}}\,{\it bb}\,x+18\,{\it bb}^2+\left(-36\,{\it aa}-15\,2^{\frac{
 3}{2}}\right)\,{\it bb}+18\,{\it aa}^2-15\,2^{\frac{3}{2}}\,{\it aa}
 +25}{18} \right] =0 \right] $$Kita bisa membuat fungsi dari hasilnya. Fungsi seperti itu sudah
didefinisikan dalam file geometri.e Euler.


\>$spread(a,b,c)


$$\frac{9}{25}$$Sebagai contoh, kita dapat menggunakannya untuk menghitung sudut
segitiga dengan sisi


Hasilnya rasional, yang tidak mudah didapatkan jika kita menggunakan
trigonometri klasik.


\>$spread(a,a,4\*a/7)


$$\frac{6}{7}$$Ini adalah sudut dalam derajat.


\>degprint(arcsin(sqrt(6/7)))


    67°47'32.44''

## Contoh lain

Sekarang, mari kita coba contoh yang lebih lanjut.


Kami menetapkan tiga sudut segitiga sebagai berikut.


\>A&:=[1,2]; B&:=[4,3]; C&:=[0,4]; ...  
\>   setPlotRange(-1,5,1,7); ...  
\>   plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); ...  
\>   plotSegment(B,A,"c"); plotSegment(A,C,"b"); plotSegment(C,B,"a"); ...  
\>   insimg;


![images/Final%20Projek%20APLIKOM-649.png](images/Final%20Projek%20APLIKOM-649.png)

Dengan menggunakan Pythogoras, mudah untuk menghitung jarak antara dua
titik. Pertama-tama saya menggunakan jarak fungsi file Euler untuk
geometri. Fungsi jarak menggunakan geometri klasik.


\>$distance(A,B)


$$\sqrt{10}$$Euler juga berisi fungsi untuk kuadran antara dua titik.


Dalam contoh berikut, karena c+b bukan a, segitiga tidak persegi
panjang.


\>c &= quad(A,B); $c, b &= quad(A,C); $b, a &= quad(B,C); $a,


$$10$$$$5$$$$17$$Pertama, mari kita hitung sudut tradisional. Fungsi computeAngle
menggunakan metode biasa berdasarkan produk titik dari dua vektor.
Hasilnya adalah beberapa perkiraan floating point.


\>wb &= computeAngle(A,B,C); $wb, $(wb/pi\*180)()


$$\arccos \left(\frac{11}{\sqrt{10}\,\sqrt{17}}\right)$$    32.4711922908

Dengan menggunakan pensil dan kertas, kita dapat melakukan hal yang
sama dengan hukum silang. Kami memasukkan kuadrat a, b, dan c ke dalam
hukum silang dan menyelesaikan x.


\>$crosslaw(a,b,c,x), $solve(%,x), //(b+c-a)^=4b.c(1-x)


$$4=200\,\left(1-x\right)$$$$\left[ x=\frac{49}{50} \right] $$Artinya, apa yang dilakukan penyebaran fungsi yang didefinisikan dalam
"geometri.e".


\>sb &= spread(b,a,c); $sb


$$\frac{49}{170}$$Maxima mendapatkan hasil yang sama dengan menggunakan trigonometri
biasa, jika kita memaksanya. Itu menyelesaikan suku sin(arccos(...))
menjadi hasil pecahan. Sebagian besar siswa tidak dapat melakukan ini.


\>$sin(computeAngle(A,B,C))^2


$$\frac{49}{170}$$Setelah kita memiliki penyebaran di B, kita dapat menghitung tinggi ha
di sisi a. Ingatlah bahwa


by definition.


\>ha &= c\*sb; $ha


$$\frac{49}{17}$$Gambar berikut telah diproduksi dengan program geometri C.a.R., yang
dapat menggambar segi empat dan penyebaran.


gambar: (20) Rational_Geometry_CaR.png


Menurut definisi panjang ha adalah akar kuadrat dari segi empatnya.


\>$sqrt(ha)


$$\frac{7}{\sqrt{17}}$$Sekarang kita dapat menghitung luas segitiga. Jangan lupa, bahwa kita
berurusan dengan segi empat!


\>$sqrt(ha)\*sqrt(a)/2


$$\frac{7}{2}$$Rumus penentu yang biasa menghasilkan hasil yang sama.


\>$areaTriangle(B,A,C)


$$\frac{7}{2}$$## Rumus Heron

Sekarang, mari kita selesaikan masalah ini secara umum!


\>&remvalue(a,b,c,sb,ha);


Pertama-tama kita menghitung spread di B untuk segitiga dengan sisi a,
b, dan c. Kemudian kita menghitung luas kuadrat ("quadrea"?),
faktorkan dengan Maxima, dan kita mendapatkan rumus Heron yang
terkenal.


Harus diakui, ini sulit dilakukan dengan pensil dan kertas.


\>$spread(b^2,c^2,a^2), $factor(%\*c^2\*a^2/4)


$$\frac{-c^4-\left(-2\,b^2-2\,a^2\right)\,c^2-b^4+2\,a^2\,b^2-a^4}{4
 \,a^2\,c^2}$$$$\frac{\left(-c+b+a\right)\,\left(c-b+a\right)\,\left(c+b-a\right)\,
 \left(c+b+a\right)}{16}$$## Aturan Triple Spread

Kerugian spread adalah tidak lagi sekadar menambahkan sudut yang sama.


Namun, tiga spread segitiga memenuhi aturan "triple spread" berikut.


\>&remvalue(sa,sb,sc); $triplespread(sa,sb,sc)


$$\left({\it sc}+{\it sb}+{\it sa}\right)^2=2\,\left({\it sc}^2+
 {\it sb}^2+{\it sa}^2\right)+4\,{\it sa}\,{\it sb}\,{\it sc}$$Aturan ini berlaku untuk tiga sudut mana pun yang jumlahnya mencapai
180°.


Sejak penyebaran


sama, aturan penyebaran tiga kali lipat juga benar, jika


Karena penyebaran sudut negatifnya sama, maka aturan penyebaran
rangkap tiga juga berlaku, jika


Misalnya, kita dapat menghitung sebaran sudut 60°. Yaitu 3/4.
Persamaan tersebut memiliki solusi kedua, di mana semua sebarannya
adalah 0.


\>$solve(triplespread(x,x,x),x)


$$\left[ x=\frac{3}{4} , x=0 \right] $$Sebaran 90° jelas adalah 1. Jika dua sudut dijumlahkan menjadi 90°,
sebarannya memecahkan persamaan sebaran rangkap tiga dengan a,b,1.
Dengan perhitungan berikut kita memperoleh a+b=1.


\>$triplespread(x,y,1), $solve(%,x)


$$\left(y+x+1\right)^2=2\,\left(y^2+x^2+1\right)+4\,x\,y$$$$\left[ x=1-y \right] $$Karena sebaran 180°-t sama dengan sebaran t, rumus sebaran rangkap
tiga juga berlaku, jika satu sudut adalah jumlah atau selisih dari dua
sudut lainnya.


Jadi kita dapat menemukan sebaran sudut yang digandakan. Perhatikan
bahwa ada dua solusi lagi. Kita buat ini menjadi fungsi.


\>$solve(triplespread(a,a,x),x), function doublespread(a) &= factor(rhs(%[1]))


$$\left[ x=4\,a-4\,a^2 , x=0 \right] $$    
                                - 4 (a - 1) a
    

## Garis Bagi Sudut

Kita sudah tahu situasinya seperti ini.


\>C&:=[0,0]; A&:=[4,0]; B&:=[0,3]; ...  
\>   setPlotRange(-1,5,-1,5); ...  
\>   plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); ...  
\>   plotSegment(B,A,"c"); plotSegment(A,C,"b"); plotSegment(C,B,"a"); ...  
\>   insimg;


![images/Final%20Projek%20APLIKOM-670.png](images/Final%20Projek%20APLIKOM-670.png)

Mari kita hitung panjang garis bagi sudut di A. Namun, kita ingin
menyelesaikannya untuk a,b,c umum.


\>&remvalue(a,b,c);


Jadi pertama-tama kita hitung sebaran sudut yang dibagi dua di A,
menggunakan rumus sebaran rangkap tiga.


Masalah dengan rumus ini muncul lagi. Rumus ini memiliki dua solusi.
Kita harus memilih yang benar. Solusi lainnya mengacu pada sudut yang
dibagi dua 180°-wa.


\>$triplespread(x,x,a/(a+b)), $solve(%,x), sa2 &= rhs(%[1]); $sa2


$$\left(2\,x+\frac{a}{b+a}\right)^2=2\,\left(2\,x^2+\frac{a^2}{\left(
 b+a\right)^2}\right)+\frac{4\,a\,x^2}{b+a}$$$$\left[ x=\frac{-\sqrt{b}\,\sqrt{b+a}+b+a}{2\,b+2\,a} , x=\frac{
 \sqrt{b}\,\sqrt{b+a}+b+a}{2\,b+2\,a} \right] $$$$\frac{-\sqrt{b}\,\sqrt{b+a}+b+a}{2\,b+2\,a}$$Mari kita periksa persegi panjang Mesir.


\>$sa2 with [a=3^2,b=4^2]


$$\frac{1}{10}$$Kita dapat mencetak sudut dalam Euler, setelah mentransfer sebaran ke
radian.


\>wa2 := arcsin(sqrt(1/10)); degprint(wa2)


    18°26'5.82''

Titik P merupakan perpotongan garis bagi sudut dengan sumbu y.


\>P := [0,tan(wa2)\*4]


    [0,  1.33333]

\>plotPoint(P,"P"); plotSegment(A,P):


![images/Final%20Projek%20APLIKOM-675.png](images/Final%20Projek%20APLIKOM-675.png)

Mari kita periksa sudut-sudut pada contoh spesifik kita.


\>computeAngle(C,A,P), computeAngle(P,A,B)


    0.321750554397
    0.321750554397

Sekarang kita hitung panjang garis bagi AP.


Kita gunakan teorema sinus pada segitiga APC. Teorema ini menyatakan
bahwa


$$\frac{BC}{\sin(w_a)} = \frac{AC}{\sin(w_b)} = \frac{AB}{\sin(w_c)}$$berlaku di sembarang segitiga. Kuadratkan, itu diterjemahkan menjadi
apa yang disebut "hukum sebaran"


$$\frac{a}{s_a} = \frac{b}{s_b} = \frac{c}{s_b}$$di mana a, b, c menunjukkan kuadran.


Karena CPA sebarannya adalah 1-sa2, kita memperoleh bisa/1=b/(1-sa2)
dan dapat menghitung bisa (kuadran garis bagi sudut).


\>&factor(ratsimp(b/(1-sa2))); bisa &= %; $bisa


$$\frac{2\,b\,\left(b+a\right)}{\sqrt{b}\,\sqrt{b+a}+b+a}$$Mari kita periksa rumus ini untuk nilai-nilai Mesir kita.


\>sqrt(mxmeval("at(bisa,[a=3^2,b=4^2])")), distance(A,P)


    4.21637021356
    4.21637021356

Kita juga dapat menghitung P menggunakan rumus spread.


\>py&=factor(ratsimp(sa2\*bisa)); $py


$$-\frac{b\,\left(\sqrt{b}\,\sqrt{b+a}-b-a\right)}{\sqrt{b}\,\sqrt{b+
 a}+b+a}$$Nilainya sama dengan yang kita dapatkan dengan rumus trigonometri.


\>sqrt(mxmeval("at(py,[a=3^2,b=4^2])"))


    1.33333333333

## Sudut Tali Busur

Perhatikan situasi berikut.


\>setPlotRange(1.2); ...  
\>   color(1); plotCircle(circleWithCenter([0,0],1)); ...  
\>   A:=[cos(1),sin(1)]; B:=[cos(2),sin(2)]; C:=[cos(6),sin(6)]; ...  
\>   plotPoint(A,"A"); plotPoint(B,"B"); plotPoint(C,"C"); ...  
\>   color(3); plotSegment(A,B,"c"); plotSegment(A,C,"b"); plotSegment(C,B,"a"); ...  
\>   color(1); O:=[0,0];  plotPoint(O,"0"); ...  
\>   plotSegment(A,O); plotSegment(B,O); plotSegment(C,O,"r"); ...  
\>   insimg;


![images/Final%20Projek%20APLIKOM-680.png](images/Final%20Projek%20APLIKOM-680.png)

Kita dapat menggunakan Maxima untuk memecahkan rumus penyebaran
rangkap tiga untuk sudut-sudut di pusat O untuk r. Dengan demikian,
kita memperoleh rumus untuk jari-jari kuadrat pericircle dalam bentuk
kuadran sisi-sisinya.


Kali ini, Maxima menghasilkan beberapa nol kompleks, yang kita
abaikan.


\>&remvalue(a,b,c,r); // hapus nilai-nilai sebelumnya untuk perhitungan baru

\>rabc &= rhs(solve(triplespread(spread(b,r,r),spread(a,r,r),spread(c,r,r)),r)[4]); $rabc


$$-\frac{a\,b\,c}{c^2-2\,b\,c+a\,\left(-2\,c-2\,b\right)+b^2+a^2}$$Kita dapat menjadikannya fungsi Euler.


\>function periradius(a,b,c) &= rabc;


Mari kita periksa hasilnya untuk titik A, B, C.


\>a:=quadrance(B,C); b:=quadrance(A,C); c:=quadrance(A,B);


Radiusnya memang 1.


\>periradius(a,b,c)


    1

Faktanya, sebaran CBA hanya bergantung pada b dan c. Ini adalah
teorema sudut tali busur.


\>$spread(b,a,c)\*rabc | ratsimp


$$\frac{b}{4}$$Faktanya, sebarannya adalah b/(4r), dan kita melihat bahwa sudut tali
busur b adalah setengah sudut pusat.


\>$doublespread(b/(4\*r))-spread(b,r,r) | ratsimp


$$0$$# Contoh 6: Jarak Minimal pada Bidang

## Catatan awal

Fungsi yang, pada titik M di bidang, menetapkan jarak AM antara titik
tetap A dan M, memiliki garis datar yang agak sederhana: lingkaran
yang berpusat di A.


\>&remvalue();

\>A=[-1,-1];

\>function d1(x,y):=sqrt((x-A[1])^2+(y-A[2])^2)

\>fcontour("d1",xmin=-2,xmax=0,ymin=-2,ymax=0,hue=1, ...  
\>   title="If you see ellipses, please set your window square"):


![images/Final%20Projek%20APLIKOM-684.png](images/Final%20Projek%20APLIKOM-684.png)

dan grafiknya cukup sederhana: bagian atas kerucut:


\>plot3d("d1",xmin=-2,xmax=0,ymin=-2,ymax=0):


![images/Final%20Projek%20APLIKOM-685.png](images/Final%20Projek%20APLIKOM-685.png)

Tentu saja minimum 0 dicapai di A.


## Dua titik

Sekarang kita lihat fungsi MA+MB di mana A dan B adalah dua titik
(tetap). Merupakan "fakta yang diketahui" bahwa kurva level adalah
elips, titik fokusnya adalah A dan B; kecuali untuk minimum AB yang
konstan pada segmen [AB]:


\>B=[1,-1];

\>function d2(x,y):=d1(x,y)+sqrt((x-B[1])^2+(y-B[2])^2)

\>fcontour("d2",xmin=-2,xmax=2,ymin=-3,ymax=1,hue=1):


![images/Final%20Projek%20APLIKOM-686.png](images/Final%20Projek%20APLIKOM-686.png)

Grafiknya lebih menarik:


\>plot3d("d2",xmin=-2,xmax=2,ymin=-3,ymax=1):


![images/Final%20Projek%20APLIKOM-687.png](images/Final%20Projek%20APLIKOM-687.png)

Pembatasan pada garis (AB) lebih terkenal:


\>plot2d("abs(x+1)+abs(x-1)",xmin=-3,xmax=3):


![images/Final%20Projek%20APLIKOM-688.png](images/Final%20Projek%20APLIKOM-688.png)

## Tiga poin

Sekarang semuanya menjadi kurang sederhana: Tidak banyak yang tahu
bahwa MA+MB+MC mencapai nilai minimumnya di satu titik bidang, tetapi
menentukannya tidaklah sesederhana itu:


1) Jika salah satu sudut segitiga ABC lebih dari 120° (misalkan di A),
maka nilai minimumnya tercapai di titik ini (misalkan AB+AC).


Contoh:


\>C=[-4,1];

\>function d3(x,y):=d2(x,y)+sqrt((x-C[1])^2+(y-C[2])^2)

\>plot3d("d3",xmin=-5,xmax=3,ymin=-4,ymax=4);

\>insimg;


![images/Final%20Projek%20APLIKOM-689.png](images/Final%20Projek%20APLIKOM-689.png)

\>fcontour("d3",xmin=-4,xmax=1,ymin=-2,ymax=2,hue=1,title="The minimum is on A");

\>P=(A\_B\_C\_A)'; plot2d(P[1],P[2],add=1,color=12);

\>insimg;


![images/Final%20Projek%20APLIKOM-690.png](images/Final%20Projek%20APLIKOM-690.png)

2) Namun jika semua sudut segitiga ABC kurang dari 120°, maka nilai
minimumnya berada di titik F di bagian dalam segitiga, yang merupakan
satu-satunya titik yang sudut-sudut sisi ABC-nya sama (masing-masing
sudutnya 120°):


\>C=[-0.5,1];

\>plot3d("d3",xmin=-2,xmax=2,ymin=-2,ymax=2):


![images/Final%20Projek%20APLIKOM-691.png](images/Final%20Projek%20APLIKOM-691.png)

\>fcontour("d3",xmin=-2,xmax=2,ymin=-2,ymax=2,hue=1,title="The Fermat point");

\>P=(A\_B\_C\_A)'; plot2d(P[1],P[2],add=1,color=12);

\>insimg;


![images/Final%20Projek%20APLIKOM-692.png](images/Final%20Projek%20APLIKOM-692.png)

Merupakan aktivitas yang menarik untuk mewujudkan gambar di atas
dengan perangkat lunak geometri; misalnya, saya mengetahui perangkat
lunak yang ditulis dalam Java yang memiliki instruksi "garis
kontur"...


Semua ini ditemukan oleh seorang hakim Prancis bernama Pierre de
Fermat; ia menulis surat kepada para dilettan lain seperti pendeta
Marin Mersenne dan Blaise Pascal yang bekerja di pajak penghasilan.
Jadi titik unik F sehingga FA+FB+FC minimal, disebut titik Fermat dari
segitiga tersebut. Namun tampaknya beberapa tahun sebelumnya,
Torriccelli dari Italia telah menemukan titik ini sebelum Fermat
menemukannya! Bagaimanapun tradisinya adalah mencatat titik F ini...


## Empat titik

Langkah berikutnya adalah menambahkan titik ke-4 D dan mencoba
meminimalkan MA+MB+MC+MD; katakanlah Anda adalah operator TV kabel dan
ingin mencari di bidang mana Anda harus meletakkan antena Anda
sehingga Anda dapat menyalurkan sinyal ke empat desa dan menggunakan
panjang kabel sesedikit mungkin!


\>D=[1,1];

\>function d4(x,y):=d3(x,y)+sqrt((x-D[1])^2+(y-D[2])^2)

\>plot3d("d4",xmin=-1.5,xmax=1.5,ymin=-1.5,ymax=1.5):


![images/Final%20Projek%20APLIKOM-693.png](images/Final%20Projek%20APLIKOM-693.png)

\>fcontour("d4",xmin=-1.5,xmax=1.5,ymin=-1.5,ymax=1.5,hue=1);

\>P=(A\_B\_C\_D)'; plot2d(P[1],P[2],points=1,add=1,color=12);

\>insimg;


![images/Final%20Projek%20APLIKOM-694.png](images/Final%20Projek%20APLIKOM-694.png)

Masih terdapat nilai minimum dan tidak tercapai di titik A, B, C,
maupun D:


\>function f(x):=d4(x[1],x[2])

\>neldermin("f",[0.2,0.2])


    [0.142858,  0.142857]

Tampaknya dalam kasus ini, koordinat titik optimal bersifat rasional
atau mendekati rasional...


Sekarang ABCD adalah persegi, kita mengharapkan bahwa titik optimal
akan menjadi pusat ABCD:


\>C=[-1,1];

\>plot3d("d4",xmin=-1,xmax=1,ymin=-1,ymax=1):


![images/Final%20Projek%20APLIKOM-695.png](images/Final%20Projek%20APLIKOM-695.png)

\>fcontour("d4",xmin=-1.5,xmax=1.5,ymin=-1.5,ymax=1.5,hue=1);

\>P=(A\_B\_C\_D)'; plot2d(P[1],P[2],add=1,color=12,points=1);

\>insimg;


![images/Final%20Projek%20APLIKOM-696.png](images/Final%20Projek%20APLIKOM-696.png)

# Contoh 7: Bola Dandelin dengan Povray

Anda dapat menjalankan demonstrasi ini, jika Anda telah menginstal
Povray, dan pvengine.exe di jalur program.


Pertama, kita hitung jari-jari bola.


Jika Anda melihat gambar di bawah, Anda melihat bahwa kita memerlukan
dua lingkaran yang menyentuh dua garis yang membentuk kerucut, dan
satu garis yang membentuk bidang yang memotong kerucut.


Kami menggunakan file geometry.e milik Euler untuk ini.


\>load geometry;


Pertama dua garis membentuk kerucut.


\>g1 &= lineThrough([0,0],[1,a])


    
                                 [- a, 1, 0]
    

\>g2 &= lineThrough([0,0],[-1,a])


    
                                [- a, - 1, 0]
    

Lalu baris ketiga.


\>g &= lineThrough([-1,0],[1,1])


    
                                 [- 1, 2, 1]
    

Kita merencanakan segalanya sejauh ini.


\>setPlotRange(-1,1,0,2);

\>color(black); plotLine(g(),"")

\>a:=2; color(blue); plotLine(g1(),""), plotLine(g2(),""):


![images/Final%20Projek%20APLIKOM-697.png](images/Final%20Projek%20APLIKOM-697.png)

Sekarang kita ambil titik umum pada sumbu y.


\>P &= [0,u]


    
                                    [0, u]
    

Hitunglah jarak ke g1.


\>d1 &= distance(P,projectToLine(P,g1)); $d1


$$\sqrt{\left(\frac{a^2\,u}{a^2+1}-u\right)^2+\frac{a^2\,u^2}{\left(a
 ^2+1\right)^2}}$$Hitunglah jarak ke g.


\>d &= distance(P,projectToLine(P,g)); $d


$$\sqrt{\left(\frac{u+2}{5}-u\right)^2+\frac{\left(2\,u-1\right)^2}{
 25}}$$Dan temukan pusat kedua lingkaran, yang jaraknya sama.


\>sol &= solve(d1^2=d^2,u); $sol


$$\left[ u=\frac{-\sqrt{5}\,\sqrt{a^2+1}+2\,a^2+2}{4\,a^2-1} , u=
 \frac{\sqrt{5}\,\sqrt{a^2+1}+2\,a^2+2}{4\,a^2-1} \right] $$Ada dua solusi.


Kita mengevaluasi solusi simbolik, dan menemukan kedua pusat, dan
kedua jarak.


\>u := sol()


    [0.333333,  1]

\>dd := d()


    [0.149071,  0.447214]

Gambarkan lingkaran-lingkaran tersebut ke dalam gambar.


\>color(red);

\>plotCircle(circleWithCenter([0,u[1]],dd[1]),"");

\>plotCircle(circleWithCenter([0,u[2]],dd[2]),"");

\>insimg;


![images/Final%20Projek%20APLIKOM-701.png](images/Final%20Projek%20APLIKOM-701.png)

## Plot dengan Povray

Selanjutnya kita plot semuanya dengan Povray. Perhatikan bahwa Anda
mengubah perintah apa pun dalam urutan perintah Povray berikut, dan
menjalankan kembali semua perintah dengan Shift-Return.


Pertama-tama kita memuat fungsi povray.


\>load povray;

\>defaultpovray="C:\\Program Files\\POV-Ray\\v3.7\\bin\\pvengine.exe"


    C:\Program Files\POV-Ray\v3.7\bin\pvengine.exe

Kami menyiapkan suasananya dengan tepat.


\>povstart(zoom=11,center=[0,0,0.5],height=10°,angle=140°);


Berikutnya kita menulis kedua bola itu ke dalam file Povray.


\>writeln(povsphere([0,0,u[1]],dd[1],povlook(red)));

\>writeln(povsphere([0,0,u[2]],dd[2],povlook(red)));


Dan kerucutnya, transparan.


\>writeln(povcone([0,0,0],0,[0,0,a],1,povlook(lightgray,1)));


Kita buat bidang yang dibatasi pada kerucut.


\>gp=g();

\>pc=povcone([0,0,0],0,[0,0,a],1,"");

\>vp=[gp[1],0,gp[2]]; dp=gp[3];

\>writeln(povplane(vp,dp,povlook(blue,0.5),pc));


Sekarang kita buat dua titik pada lingkaran, di mana bola menyentuh
kerucut.


\>function turnz(v) := return [-v[2],v[1],v[3]]

\>P1=projectToLine([0,u[1]],g1()); P1=turnz([P1[1],0,P1[2]]);

\>writeln(povpoint(P1,povlook(yellow)));

\>P2=projectToLine([0,u[2]],g1()); P2=turnz([P2[1],0,P2[2]]);

\>writeln(povpoint(P2,povlook(yellow)));


Kemudian kita buat dua titik tempat bola-bola tersebut menyentuh
bidang. Titik-titik ini adalah fokus elips.


\>P3=projectToLine([0,u[1]],g()); P3=[P3[1],0,P3[2]];

\>writeln(povpoint(P3,povlook(yellow)));

\>P4=projectToLine([0,u[2]],g()); P4=[P4[1],0,P4[2]];

\>writeln(povpoint(P4,povlook(yellow)));


Berikutnya kita hitung perpotongan P1P2 dengan bidang.


\>t1=scalp(vp,P1)-dp; t2=scalp(vp,P2)-dp; P5=P1+t1/(t1-t2)\*(P2-P1);

\>writeln(povpoint(P5,povlook(yellow)));


Kita menghubungkan titik-titik dengan segmen garis.


\>writeln(povsegment(P1,P2,povlook(yellow)));

\>writeln(povsegment(P5,P3,povlook(yellow)));

\>writeln(povsegment(P5,P4,povlook(yellow)));


Sekarang kita buat pita abu-abu, di mana bola-bola menyentuh kerucut.


\>pcw=povcone([0,0,0],0,[0,0,a],1.01);

\>pc1=povcylinder([0,0,P1[3]-defaultpointsize/2],[0,0,P1[3]+defaultpointsize/2],1);

\>writeln(povintersection([pcw,pc1],povlook(gray)));

\>pc2=povcylinder([0,0,P2[3]-defaultpointsize/2],[0,0,P2[3]+defaultpointsize/2],1);

\>writeln(povintersection([pcw,pc2],povlook(gray)));


Mulai program Povray.


\>povend();


![images/Final%20Projek%20APLIKOM-702.png](images/Final%20Projek%20APLIKOM-702.png)

Untuk mendapatkan Anaglyph ini, kita perlu memasukkan semuanya ke
dalam fungsi scene. Fungsi ini akan digunakan dua kali nanti.


\>function scene () ...


    global a,u,dd,g,g1,defaultpointsize;
    writeln(povsphere([0,0,u[1]],dd[1],povlook(red)));
    writeln(povsphere([0,0,u[2]],dd[2],povlook(red)));
    writeln(povcone([0,0,0],0,[0,0,a],1,povlook(lightgray,1)));
    gp=g();
    pc=povcone([0,0,0],0,[0,0,a],1,"");
    vp=[gp[1],0,gp[2]]; dp=gp[3];
    writeln(povplane(vp,dp,povlook(blue,0.5),pc));
    P1=projectToLine([0,u[1]],g1()); P1=turnz([P1[1],0,P1[2]]);
    writeln(povpoint(P1,povlook(yellow)));
    P2=projectToLine([0,u[2]],g1()); P2=turnz([P2[1],0,P2[2]]);
    writeln(povpoint(P2,povlook(yellow)));
    P3=projectToLine([0,u[1]],g()); P3=[P3[1],0,P3[2]];
    writeln(povpoint(P3,povlook(yellow)));
    P4=projectToLine([0,u[2]],g()); P4=[P4[1],0,P4[2]];
    writeln(povpoint(P4,povlook(yellow)));
    t1=scalp(vp,P1)-dp; t2=scalp(vp,P2)-dp; P5=P1+t1/(t1-t2)*(P2-P1);
    writeln(povpoint(P5,povlook(yellow)));
    writeln(povsegment(P1,P2,povlook(yellow)));
    writeln(povsegment(P5,P3,povlook(yellow)));
    writeln(povsegment(P5,P4,povlook(yellow)));
    pcw=povcone([0,0,0],0,[0,0,a],1.01);
    pc1=povcylinder([0,0,P1[3]-defaultpointsize/2],[0,0,P1[3]+defaultpointsize/2],1);
    writeln(povintersection([pcw,pc1],povlook(gray)));
    pc2=povcylinder([0,0,P2[3]-defaultpointsize/2],[0,0,P2[3]+defaultpointsize/2],1);
    writeln(povintersection([pcw,pc2],povlook(gray)));
    endfunction
</pre>
Anda memerlukan kacamata merah/cyan untuk menghargai efek berikut.


\>povanaglyph("scene",zoom=11,center=[0,0,0.5],height=10°,angle=140°);


![images/Final%20Projek%20APLIKOM-703.png](images/Final%20Projek%20APLIKOM-703.png)

# Contoh 8: Geometri Bumi

Dalam buku catatan ini, kami ingin melakukan beberapa perhitungan
sferis. Fungsi-fungsi tersebut terdapat dalam berkas "spherical.e" di
folder contoh. Kami perlu memuat berkas tersebut terlebih dahulu.


\>load "spherical.e";


Untuk memasukkan posisi geografis, kami menggunakan vektor dengan dua
koordinat dalam radian (utara dan timur, nilai negatif untuk selatan
dan barat). Berikut ini adalah koordinat untuk Kampus FMIPA UNY.


\>FMIPA=[rad(-7,-46.467),rad(110,23.05)]


    [-0.13569,  1.92657]

Anda dapat mencetak posisi ini dengan sposprint (cetak posisi bulat).


\>sposprint(FMIPA) // posisi garis lintang dan garis bujur FMIPA UNY


    S 7°46.467' E 110°23.050'

Mari kita tambahkan dua kota lagi, Solo dan Semarang.


\>Solo=[rad(-7,-34.333),rad(110,49.683)]; Semarang=[rad(-6,-59.05),rad(110,24.533)];

\>sposprint(Solo), sposprint(Semarang),


    S 7°34.333' E 110°49.683'
    S 6°59.050' E 110°24.533'

Pertama, kita hitung vektor dari satu ke yang lain pada bola ideal.
Vektor ini adalah [arah, jarak] dalam radian. Untuk menghitung jarak
di bumi, kita kalikan dengan jari-jari bumi pada garis lintang 7°.


\>br=svector(FMIPA,Solo); degprint(br[1]), br[2]\*rearth(7°)-\>km // perkiraan jarak FMIPA-Solo


    65°20'26.60''
    53.8945384608

Ini adalah perkiraan yang bagus. Rutin berikut menggunakan perkiraan
yang lebih baik lagi. Pada jarak yang pendek, hasilnya hampir sama.


\>esdist(FMIPA,Semarang)-\>" km" // perkiraan jarak FMIPA-Semarang


    Commands must be separated by semicolon or comma!
    Found:  // perkiraan jarak FMIPA-Semarang (character 32)
    You can disable this in the Options menu.
    Error in:
    esdist(FMIPA,Semarang)-&gt;" km" // perkiraan jarak FMIPA-Semaran ...
                                 ^

Ada fungsi untuk judul, yang memperhitungkan bentuk elips bumi. Sekali
lagi, kami mencetak dengan cara yang canggih.


\>sdegprint(esdir(FMIPA,Solo))


         65.34°

Sudut suatu segitiga melebihi 180° pada bola.


\>asum=sangle(Solo,FMIPA,Semarang)+sangle(FMIPA,Solo,Semarang)+sangle(FMIPA,Semarang,Solo); degprint(asum)


    180°0'10.77''

Ini dapat digunakan untuk menghitung luas segitiga. Catatan: Untuk
segitiga kecil, ini tidak akurat karena kesalahan pengurangan dalam
asum-pi.


\>(asum-pi)\*rearth(48°)^2-\>" km^2" // perkiraan luas segitiga FMIPA-Solo-Semarang


    Commands must be separated by semicolon or comma!
    Found:  // perkiraan luas segitiga FMIPA-Solo-Semarang (character 32)
    You can disable this in the Options menu.
    Error in:
    (asum-pi)*rearth(48°)^2-&gt;" km^2" // perkiraan luas segitiga FM ...
                                    ^

Ada fungsi untuk ini, yang menggunakan lintang rata-rata segitiga
untuk menghitung jari-jari bumi, dan menangani kesalahan pembulatan
untuk segitiga yang sangat kecil.


\>esarea(Solo,FMIPA,Semarang)-\>" km^2", //perkiraan yang sama dengan fungsi esarea()


    2123.64310526 km^2

Kita juga dapat menambahkan vektor ke posisi. Vektor berisi arah dan
jarak, keduanya dalam radian. Untuk mendapatkan vektor, kita
menggunakan svector. Untuk menambahkan vektor ke posisi, kita
menggunakan saddvector.


\>v=svector(FMIPA,Solo); sposprint(saddvector(FMIPA,v)), sposprint(Solo),


    S 7°34.333' E 110°49.683'
    S 7°34.333' E 110°49.683'

Fungsi-fungsi ini mengasumsikan bentuk bola yang ideal. Sama halnya di
bumi.


\>sposprint(esadd(FMIPA,esdir(FMIPA,Solo),esdist(FMIPA,Solo))), sposprint(Solo),


    S 7°34.333' E 110°49.683'
    S 7°34.333' E 110°49.683'

Mari kita lihat contoh yang lebih besar, Tugu Jogja dan Monas Jakarta
(menggunakan Google Earth untuk mencari koordinatnya).


\>Tugu=[-7.7833°,110.3661°]; Monas=[-6.175°,106.811944°];

\>sposprint(Tugu), sposprint(Monas)


    S 7°46.998' E 110°21.966'
    S 6°10.500' E 106°48.717'

Menurut Google Earth, jaraknya adalah 429,66 km. Kami memperoleh
perkiraan yang baik.


\>esdist(Tugu,Monas)-\>" km" // perkiraan jarak Tugu Jogja - Monas Jakarta


    Commands must be separated by semicolon or comma!
    Found:  // perkiraan jarak Tugu Jogja - Monas Jakarta (character 32)
    You can disable this in the Options menu.
    Error in:
    esdist(Tugu,Monas)-&gt;" km" // perkiraan jarak Tugu Jogja - Mona ...
                             ^

Judulnya sama dengan yang dihitung di Google Earth.


\>degprint(esdir(Tugu,Monas))


    294°17'2.85''

Akan tetapi, kita tidak lagi memperoleh posisi target yang tepat, jika
kita menambahkan arah dan jarak ke posisi awal. Hal ini terjadi karena
kita tidak menghitung fungsi invers secara tepat, tetapi mengambil
perkiraan radius bumi di sepanjang lintasan.


\>sposprint(esadd(Tugu,esdir(Tugu,Monas),esdist(Tugu,Monas)))


    S 6°10.500' E 106°48.717'

Namun, kesalahannya tidak besar.


\>sposprint(Monas),


    S 6°10.500' E 106°48.717'

Tentu saja, kita tidak dapat berlayar dengan arah yang sama dari satu
tujuan ke tujuan lain, jika kita ingin mengambil jalur terpendek.
Bayangkan, Anda terbang ke arah timur laut mulai dari titik mana pun
di bumi. Kemudian Anda akan berputar ke kutub utara. Lingkaran besar
tidak mengikuti arah yang konstan!


Perhitungan berikut menunjukkan bahwa kita jauh dari tujuan yang
benar, jika kita menggunakan arah yang sama selama perjalanan kita.


\>dist=esdist(Tugu,Monas); hd=esdir(Tugu,Monas);


Sekarang kita tambahkan 10 dikalikan sepersepuluh jaraknya, dengan
memakai arah ke Monas, kita sampai di Tugu.


\>p=Tugu; loop 1 to 10; p=esadd(p,hd,dist/10); end;


Hasilnya sangat jauh.


\>sposprint(p), skmprint(esdist(p,Monas))


    S 6°11.250' E 106°48.372'
         1.529km

Sebagai contoh lain, mari kita ambil dua titik di bumi pada garis
lintang yang sama.


\>P1=[30°,10°]; P2=[30°,50°];


Lintasan terpendek dari P1 ke P2 bukanlah lingkaran lintang 30°,
tetapi lintasan yang lebih pendek yang dimulai 10° lebih jauh ke utara
di P1.


\>sdegprint(esdir(P1,P2))


         79.69°

Namun, jika kita mengikuti pembacaan kompas ini, kita akan berputar ke
kutub utara! Jadi kita harus menyesuaikan arah kita di sepanjang
jalan. Untuk tujuan kasar, kita menyesuaikannya pada 1/10 dari total
jarak.


\>p=P1;  dist=esdist(P1,P2); ...  
\>     loop 1 to 10; dir=esdir(p,P2); sdegprint(dir), p=esadd(p,dir,dist/10); end;


         79.69°
         81.67°
         83.71°
         85.78°
         87.89°
         90.00°
         92.12°
         94.22°
         96.29°
         98.33°

Jaraknya tidak tepat, karena kita akan menambahkan sedikit kesalahan,
jika kita mengikuti arah yang sama terlalu lama.


\>skmprint(esdist(p,P2))


         0.203km

Kita memperoleh perkiraan yang baik, jika kita menyesuaikan arah
setelah setiap 1/100 jarak total dari Tugu ke Monas.


\>p=Tugu; dist=esdist(Tugu,Monas); ...  
\>     loop 1 to 100; p=esadd(p,esdir(p,Monas),dist/100); end;

\>skmprint(esdist(p,Monas))


         0.000km

Untuk keperluan navigasi, kita bisa mendapatkan urutan posisi GPS
sepanjang lingkaran besar menuju Monas dengan fungsi navigasi.


\>load spherical; v=navigate(Tugu,Monas,10); ...  
\>     loop 1 to rows(v); sposprint(v[#]), end;


    S 7°46.998' E 110°21.966'
    S 7°37.422' E 110°0.573'
    S 7°27.829' E 109°39.196'
    S 7°18.219' E 109°17.834'
    S 7°8.592' E 108°56.488'
    S 6°58.948' E 108°35.157'
    S 6°49.289' E 108°13.841'
    S 6°39.614' E 107°52.539'
    S 6°29.924' E 107°31.251'
    S 6°20.219' E 107°9.977'
    S 6°10.500' E 106°48.717'

Kita menulis suatu fungsi yang memplot bumi, dua posisi, dan posisi di
antaranya.


\>function testplot ...


    useglobal;
    plotearth;
    plotpos(Tugu,"Tugu Jogja"); plotpos(Monas,"Tugu Monas");
    plotposline(v);
    endfunction
</pre>
Sekarang rencanakan semuanya.


\>plot3d("testplot",angle=25, height=6,\>own,\>user,zoom=4):


![images/Final%20Projek%20APLIKOM-704.png](images/Final%20Projek%20APLIKOM-704.png)

Atau gunakan plot3d untuk mendapatkan tampilan anaglifnya. Ini tampak
sangat bagus dengan kaca mata merah/biru kehijauan.


\>plot3d("testplot",angle=25,height=6,distance=5,own=1,anaglyph=1,zoom=4):


![images/Final%20Projek%20APLIKOM-705.png](images/Final%20Projek%20APLIKOM-705.png)

# Latihan

1. Gambarlah segi-n beraturan jika diketahui titik pusat O, n, dan
jarak titik pusat ke titik-titik sudut segi-n tersebut (jari-jari
lingkaran luar segi-n), r.


Petunjuk:


* 
Besar sudut pusat yang menghadap masing-masing sisi segi-n adalah
* (360/n).

* 
Titik-titik sudut segi-n merupakan perpotongan lingkaran luar segi-n
* dan garis-garis yang melalui pusat dan saling membentuk sudut sebesar
* kelipatan (360/n).

* 
Untuk n ganjil, pilih salah satu titik sudut adalah di atas.

* 
Untuk n genap, pilih 2 titik di kanan dan kiri lurus dengan titik
* pusat.

* 
Anda dapat menggambar segi-3, 4, 5, 6, 7, dst beraturan.


\>load geometry


    Numerical and symbolic geometry.

\>setPlotRange(-3.5,3.5,-3.5,3.5);

\>A=[-2,-2]; plotPoint(A,"A");

\>B=[2,-2]; plotPoint(B,"B");

\>C=[0,3]; plotPoint(C,"C");

\>plotSegment(A,B,"c");

\>plotSegment(B,C,"a");

\>plotSegment(A,C,"b");

\>aspect(1):


![images/Final%20Projek%20APLIKOM-706.png](images/Final%20Projek%20APLIKOM-706.png)

\>c=circleThrough(A,B,C);

\>R=getCircleRadius(c);

\>O=getCircleCenter(c);

\>plotPoint(O,"O");

\>l=angleBisector(A,C,B);

\>color(2); plotLine(l); color(1);

\>plotCircle(c,"Lingkaran luar segitiga ABC"):


![images/Final%20Projek%20APLIKOM-707.png](images/Final%20Projek%20APLIKOM-707.png)

2. Gambarlah suatu parabola yang melalui 3 titik yang diketahui.


Petunjuk:


- Misalkan persamaan parabolanya y= ax^2+bx+c.


- Substitusikan koordinat titik-titik yang diketahui ke persamaan
tersebut.


- Selesaikan SPL yang terbentuk untuk mendapatkan nilai-nilai a, b, c.


\>load geometry;

\>setPlotRange(5); P=[2,0]; Q=[4,0]; R=[0,-4];

\>plotPoint(P,"P"); plotPoint(Q,"Q"); plotPoint(R,"R"):


![images/Final%20Projek%20APLIKOM-708.png](images/Final%20Projek%20APLIKOM-708.png)

\>sol &= solve([a+b=-c,16\*a+4\*b=-c,c=-4],[a,b,c])


    
                         [[a = - 1, b = 5, c = - 4]]
    

Sehingga dapat ditentukan nilai a = -1, b = 5 dan c = -4


\>function y&=4\*x^2+5\*x-12


    
                                  2
                               4 x  + 5 x - 12
    

\>plot2d("4\*x^2+5\*x-12",-13,13,-13,13):


![images/Final%20Projek%20APLIKOM-709.png](images/Final%20Projek%20APLIKOM-709.png)

3. Gambarlah suatu segi-4 yang diketahui keempat titik sudutnya,
misalnya A, B, C, D.


   - Tentukan apakah segi-4 tersebut merupakan segi-4 garis singgung
(sisinya-sisintya merupakan garis singgung lingkaran yang sama yakni
lingkaran dalam segi-4 tersebut).


   - Suatu segi-4 merupakan segi-4 garis singgung apabila keempat
garis bagi sudutnya bertemu di satu titik.


   - Jika segi-4 tersebut merupakan segi-4 garis singgung, gambar
lingkaran dalamnya.


   - Tunjukkan bahwa syarat suatu segi-4 merupakan segi-4 garis
singgung apabila hasil kali panjang sisi-sisi yang berhadapan sama.


\>load geometry


    Numerical and symbolic geometry.

\>setPlotRange(-5,5,-5,5);

\>A=[-4,-4]; plotPoint(A,"A");

\>B=[4,-4]; plotPoint(B,"B");

\>C=[4,4]; plotPoint(C,"C");

\>D=[-4,4]; plotPoint(D,"D");

\>plotSegment(A,B,"");

\>plotSegment(B,C,"");

\>plotSegment(C,D,"");

\>plotSegment(A,D,"");

\>aspect(1):


![images/Final%20Projek%20APLIKOM-710.png](images/Final%20Projek%20APLIKOM-710.png)

\>l=angleBisector(A,B,C);

\>m=angleBisector(B,C,D);

\>P=lineIntersection(l,m);

\>color(5); plotLine(l); plotLine(m); color(1);

\>plotPoint(P,"P"):


![images/Final%20Projek%20APLIKOM-711.png](images/Final%20Projek%20APLIKOM-711.png)

Dapat dilihat bahwa keempat garis bagi sudutnya bertemu di satu titik
yaitu titik P.


\>r=norm(P-projectToLine(P,lineThrough(A,B)));

\>plotCircle(circleWithCenter(P,r),"Lingkaran dalam segiempat ABCD"):


![images/Final%20Projek%20APLIKOM-712.png](images/Final%20Projek%20APLIKOM-712.png)

Dapat dilihat bahwa sisi-sisinya merupakan garis singgung lingkaran
yang sama.


Akan ditunjukkan bahwa hasil kali panjang sisi-sisi yang berhadapan
sama.


\>AB=norm(A-B)


    8

\>CD=norm(C-D)


    8

\>AD=norm(A-D)


    8

\>BC=norm(B-C)


    8

\>AB.CD


    64

\>AD.BC


    64

Terbukti bahwa hasil kali panjang sisi-sisi yang berhadapan sama yaitu
64. Jadi dapat dipastikan bahwa segiempat tersebut merupakan segiempat
garis singgung.


4. Gambarlah suatu ellips jika diketahui kedua titik fokusnya,
misalnya P dan Q. Ingat ellips dengan fokus P dan Q adalah tempat
kedudukan titik-titik yang jumlah jarak ke P dan ke Q selalu sama
(konstan).


Penyelesaian :


Diketahui kedua titik fokus P = [-2,-2] dan Q = [2,-2]


\>P=[-2,-2]; Q=[2,-2];

\>function d1(x,y):=sqrt((x-P[1])^2+(y-P[2])^2)

\>Q=[2,-2]; function d2(x,y):=sqrt((x-P[1])^2+(y-P[2])^2)+sqrt((x-Q[1])^2+(y-Q[2])^2)

\>fcontour("d2",xmin=-2,xmax=2,ymin=-3,ymax=1,hue=1):


![images/Final%20Projek%20APLIKOM-713.png](images/Final%20Projek%20APLIKOM-713.png)

\>plot3d("d2",xmin=-2,xmax=2,ymin=-3,ymax=1):


![images/Final%20Projek%20APLIKOM-714.png](images/Final%20Projek%20APLIKOM-714.png)

\>plot2d("abs(x+1)+abs(x-1)",xmin=-3,xmax=3):


![images/Final%20Projek%20APLIKOM-715.png](images/Final%20Projek%20APLIKOM-715.png)

5. Gambarlah suatu hiperbola jika diketahui kedua titik fokusnya,
misalnya P dan Q. Ingat ellips dengan fokus P dan Q adalah tempat
kedudukan titik-titik yang selisih jarak ke P dan ke Q selalu sama
(konstan).


\>P=[-2,-2]; Q=[2,-2];

\>function d1(x,y):=sqrt((x-p[1])^2+(y-p[2])^2)

\>Q=[2,-2]; function d2(x,y):=sqrt((x-P[1])^2+(y-P[2])^2)+sqrt((x+Q[1])^2+(y+Q[2])^2)

\>fcontour("d2",xmin=-2,xmax=2,ymin=-3,ymax=1,hue=1):


![images/Final%20Projek%20APLIKOM-716.png](images/Final%20Projek%20APLIKOM-716.png)

\>plot3d("d2",xmin=-2,xmax=2,ymin=-3,ymax=1):


![images/Final%20Projek%20APLIKOM-717.png](images/Final%20Projek%20APLIKOM-717.png)

\>plot2d("abs(x+1)+abs(x-1)",xmin=-3,xmax=3):


![images/Final%20Projek%20APLIKOM-718.png](images/Final%20Projek%20APLIKOM-718.png)

# EMT untuk Statistika

Dalam buku catatan ini, kami menunjukkan plot, pengujian, dan
distribusi statistik utama dalam Euler.


Mari kita mulai dengan beberapa statistik deskriptif. Ini bukan
pengantar statistik. Jadi, Anda mungkin memerlukan beberapa latar
belakang untuk memahami detailnya.


Asumsikan pengukuran berikut. Kami ingin menghitung nilai rata-rata
dan simpangan baku yang diukur.


\>M=[1000,1004,998,997,1002,1001,998,1004,998,997]; ...  
\>   median(M), mean(M), dev(M),


    999
    999.9
    2.72641400622

Kita bisa membuat suatu box-and-whiskers plot untuk suatu data.Dalam
kasus kami, tak ada outlier.


\>aspect(1.75); boxplot(M):


![images/Final%20Projek%20APLIKOM-719.png](images/Final%20Projek%20APLIKOM-719.png)

Kami menghitung probabilitas bahwa suatu nilai lebih besar dari 1005,
dengan asumsi nilai yang diukur berasal dari distribusi normal.


Semua fungsi untuk distribusi di Euler diakhiri dengan ...dis dan
menghitung distribusi probabilitas kumulatif (CPF).


$$\text{normaldis(x,m,d)}=\int_{-\infty}^x \frac{1}{d\sqrt{2\pi}}e^{-\frac{1}{2}(\frac{t-m}{d})^2}\ dt.$$Kami mencetak hasil dalam % dengan akurasi 2 digit menggunakan fungsi
cetak.


\>print((1-normaldis(1005,mean(M),dev(M)))\*100,2,unit=" %")


          3.07 %

Untuk contoh berikutnya, kami mengasumsikan jumlah pria berikut dalam
rentang ukuran tertentu.


\>r=155.5:4:187.5; v=[22,71,136,169,139,71,32,8];


Berikut adalah plot distribusinya.


\>plot2d(r,v,a=150,b=200,c=0,d=190,bar=1,style="\\/"):


![images/Final%20Projek%20APLIKOM-721.png](images/Final%20Projek%20APLIKOM-721.png)

Kita dapat memasukkan data mentah tersebut ke dalam tabel.


Tabel adalah metode untuk menyimpan data statistik. Tabel kita harus
berisi tiga kolom: Awal rentang, akhir rentang, jumlah orang dalam
rentang.


Tabel dapat dicetak dengan tajuk. Kita menggunakan vektor string untuk
mengatur judul.


\>T:=r[1:8]' | r[2:9]' | v'; writetable(T,labc=["BB","BA","Frek"])


            BB        BA      Frek
         155.5     159.5        22
         159.5     163.5        71
         163.5     167.5       136
         167.5     171.5       169
         171.5     175.5       139
         175.5     179.5        71
         179.5     183.5        32
         183.5     187.5         8

Jika kita memerlukan nilai rata-rata dan statistik ukuran lainnya,
kita perlu menghitung titik tengah rentang. Kita dapat menggunakan dua
kolom pertama tabel kita untuk ini.


Simbol "|" digunakan untuk memisahkan kolom, fungsi "writetable"
digunakan untuk menulis tabel, dengan opsi "labc" untuk menentukan
judul kolom.


\>(T[,1]+T[,2])/2 // the midpoint of each interval


            157.5 
            161.5 
            165.5 
            169.5 
            173.5 
            177.5 
            181.5 
            185.5 

Namun lebih mudah untuk melipat rentang dengan vektor [1/2,1/2].


\>M=fold(r,[0.5,0.5])


    [157.5,  161.5,  165.5,  169.5,  173.5,  177.5,  181.5,  185.5]

Sekarang kita dapat menghitung rata-rata dan deviasi sampel dengan
frekuensi yang diberikan.


\>{m,d}=meandev(M,v); m, d,


    169.901234568
    5.98912964449

Mari kita tambahkan distribusi normal nilai-nilai tersebut ke diagram
batang di atas. Rumus untuk distribusi normal dengan mean m dan
simpangan baku d adalah:


$$y=\frac{1}{d\sqrt{2\pi}}e^{\frac{-(x-m)^2}{2d^2}}.$$Karena nilainya berada antara 0 dan 1, untuk memplotnya pada bar plot
(grafik batang), nilainya harus dikalikan dengan 4 kali jumlah data
total.


\>plot2d("qnormal(x,m,d)\*sum(v)\*4", ...  
\>     xmin=min(r),xmax=max(r),thickness=3,add=1):


![images/Final%20Projek%20APLIKOM-723.png](images/Final%20Projek%20APLIKOM-723.png)

# Tabel

Di direktori buku catatan ini, Anda akan menemukan file dengan tabel.
Data tersebut merupakan hasil survei. Berikut adalah empat baris
pertama file tersebut. Data tersebut berasal dari buku daring Jerman
"Einführung in die Statistik mit R" karya A. Handl.


\>printfile("table.dat",4);


    Could not open the file
    table.dat
    for reading!
    Try "trace errors" to inspect local variables after errors.
    printfile:
        open(filename,"r");

Tabel berisi 7 kolom angka atau token (string). Kita ingin membaca
tabel dari file. Pertama, kita menggunakan terjemahan kita sendiri
untuk token.


Untuk ini, kita mendefinisikan set token. Fungsi strtokens()
mendapatkan vektor string token dari string yang diberikan.


\>mf:=["m","f"]; yn:=["y","n"]; ev:=strtokens("g vg m b vb");


Sekarang kita baca tabel dengan terjemahan ini.


Argumen tok2, tok4, dst. adalah terjemahan kolom-kolom tabel. Argumen
ini tidak ada dalam daftar parameter readtable(), jadi Anda perlu
menyediakannya dengan ":=".


\>{MT,hd}=readtable("table.dat",tok2:=mf,tok4:=yn,tok5:=ev,tok7:=yn);


    Could not open the file
    table.dat
    for reading!
    Try "trace errors" to inspect local variables after errors.
    readtable:
        if filename!=none then open(filename,"r"); endif;

\>load over statistics;


Untuk mencetak, kita perlu menentukan set token yang sama. Kita cetak
empat baris pertama saja.


\>writetable(MT[1:10],labc=hd,wc=5,tok2:=mf,tok4:=yn,tok5:=ev,tok7:=yn);


    MT is not a variable!
    Error in:
    writetable(MT[1:10],labc=hd,wc=5,tok2:=mf,tok4:=yn,tok5:=ev,to ...
                       ^

Titik "." mewakili nilai yang tidak tersedia.


Jika kita tidak ingin menentukan token untuk penerjemahan terlebih
dahulu, kita hanya perlu menentukan kolom mana yang berisi token dan
bukan angka.


\>ctok=[2,4,5,7]; {MT,hd,tok}=readtable("table.dat",ctok=ctok);


    Could not open the file
    table.dat
    for reading!
    Try "trace errors" to inspect local variables after errors.
    readtable:
        if filename!=none then open(filename,"r"); endif;

Fungsi readtable() sekarang mengembalikan set token.


\>tok


    Variable tok not found!
    Error in:
    tok ...
       ^

Tabel berisi entri dari file dengan token yang diterjemahkan ke angka.


String khusus NA="." diinterprtasikan sebagai "Not Available (Tidak
Tersedia)", dan mendapatkan NAN (not a number (bukan angka)) dalam
tabel. Terjemahan ini dapat diubah dengan parameter NA, dan NAval.


\>MT[1]


    MT is not a variable!
    Error in:
    MT[1] ...
         ^

Berikut ini adalah isi tabel dengan angka yang belum diterjemahkan.


\>writetable(MT,wc=5)


    Variable or function MT not found.
    Error in:
    writetable(MT,wc=5) ...
                 ^

Demi kenyamanan, Anda dapat memasukkan output readtable() ke dalam
daftar.


\>Table={{readtable("table.dat",ctok=ctok)}};


    Could not open the file
    table.dat
    for reading!
    Try "trace errors" to inspect local variables after errors.
    readtable:
        if filename!=none then open(filename,"r"); endif;

Dengan menggunakan kolom token yang sama dan token yang dibaca dari
file, kita dapat mencetak tabel. Kita dapat menentukan ctok, tok, dll.
atau menggunakan tabel list.


\>writetable(Table,ctok=ctok,wc=5);


    Variable or function Table not found.
    Error in:
    writetable(Table,ctok=ctok,wc=5); ...
                    ^

Fungsi tablecol()mengembalikan nilai dari kolom tabel,melewati
baris-bairs dengan NAN values("." dalam file), dan indeks kolom, yang
berisi nilai-nilai ini. 


\>{c,i}=tablecol(MT,[5,6]);


    Variable or function MT not found.
    Error in:
    {c,i}=tablecol(MT,[5,6]); ...
                     ^

Kita bisa menggunakan ini untuk mengestrak kolom dari tabel untuk
membuat tabel baru.


\>j=[1,5,6]; writetable(MT[i,j],labc=hd[j],ctok=[2],tok=tok)


    MT is not a variable!
    Error in:
    j=[1,5,6]; writetable(MT[i,j],labc=hd[j],ctok=[2],tok=tok) ...
                                 ^

Tentu, kita harus mengestrak tabel itu sendiri dari list tabel pada
kasus ini.


\>MT=Table[1];


    Table is not a variable!
    Error in:
    MT=Table[1]; ...
               ^

Tentu, kita juga bisa menggunakan ini untuk mencari nilai rata-rata
pada kolom atau nilai statistika yang lain.


\>mean(tablecol(MT,6))


    Variable or function MT not found.
    Error in:
    mean(tablecol(MT,6)) ...
                    ^

Fungsi getstatistics() mengembalikan elemen pada vektor, dan
jumlahnya. Kita bisa menggunakan ini untuk nilai "m" dan "f" pada
kolom kedua dari tabel kita tadi.


\>{xu,count}=getstatistics(tablecol(MT,2)); xu, count,


    Variable or function MT not found.
    Error in:
    {xu,count}=getstatistics(tablecol(MT,2)); xu, count, ...
                                        ^

Kita bisa mencetak hasilnya di tabel baru kita.


\>writetable(count',labr=tok[xu])


    Variable count not found!
    Error in:
    writetable(count',labr=tok[xu]) ...
                     ^

Fungsi selecttable() mengembalikan tabel baru dengan nilai-nilai dalam
satu kolom yang dipilih dari vektor indeks. Pertama-tama kita mencari
indeks dari dua nilai di tabel token.


\>v:=indexof(tok,["g","vg"])


    Variable or function tok not found.
    Error in:
    v:=indexof(tok,["g","vg"]) ...
                  ^

Sekarang kita bisa memilih baris dari tabel, yang memiliki salah satu
nilai dalam v di baris ke-5.


\>MT1:=MT[selectrows(MT,5,v)]; i:=sortedrows(MT1,5);


    Variable or function MT not found.
    Error in:
    MT1:=MT[selectrows(MT,5,v)]; i:=sortedrows(MT1,5); ...
                         ^

Sekarang kita dapat mencetak tabel, dengan nilai yang diekstraksi dan
diurutkan di kolom ke-5.


\>writetable(MT1[i],labc=hd,ctok=ctok,tok=tok,wc=7);


    MT1 is not a variable!
    Error in:
    writetable(MT1[i],labc=hd,ctok=ctok,tok=tok,wc=7); ...
                     ^

Untuk statistik berikutnya, kita ingin menghubungkan dua kolom tabel.
Jadi, kita mengekstrak kolom 2 dan 4 dan mengurutkan tabel.


\>i=sortedrows(MT,[2,4]);  ...  
\>     writetable(tablecol(MT[i],[2,4])',ctok=[1,2],tok=tok)


    Variable or function MT not found.
    Error in:
    i=sortedrows(MT,[2,4]);    writetable(tablecol(MT[i],[2,4])',c ...
                   ^

Dengan getstatistics(), kita juga dapat menghubungkan jumlah pada dua
kolom tabel satu sama lain.


\>MT24=tablecol(MT,[2,4]); ...  
\>   {xu1,xu2,count}=getstatistics(MT24[1],MT24[2]); ...  
\>   writetable(count,labr=tok[xu1],labc=tok[xu2])


    Variable or function MT not found.
    Error in:
    MT24=tablecol(MT,[2,4]); {xu1,xu2,count}=getstatistics(MT24[1] ...
                    ^

Suatu tabel dapat ditulis ke dalam suatu file.


\>filename="test.dat"; ...  
\>   writetable(count,labr=tok[xu1],labc=tok[xu2],file=filename);


    Variable or function count not found.
    Error in:
    filename="test.dat"; writetable(count,labr=tok[xu1],labc=tok[x ...
                                         ^

Lalu kita dapat membaca tabel dari file tersebut.


\>{MT2,hd,tok2,hdr}=readtable(filename,\>clabs,\>rlabs); ...  
\>   writetable(MT2,labr=hdr,labc=hd)


    Could not open the file
    test.dat
    for reading!
    Try "trace errors" to inspect local variables after errors.
    readtable:
        if filename!=none then open(filename,"r"); endif;

Dan hapus filenya.


\>fileremove(filename);


# Distribusi

Dengan plot2d, ada metode yang sangat mudah untuk memplot distribusi
data eksperimen.


\>p=normal(1,1000); //1000 random normal-distributed sample p

\>plot2d(p,distribution=20,style="\\/"); // plot the random sample p

\>plot2d("qnormal(x,0,1)",add=1): // add the standard normal distribution plot


![images/Final%20Projek%20APLIKOM-724.png](images/Final%20Projek%20APLIKOM-724.png)

Harap perhatikan perbedaan antara bar plot (sample) dan kurva normal
(distribusi riil). Masukkan kembali ketiga perintah tersebut untuk
melihat hasil sampel lainnya.


Berikut ini adalah perbandingan 10 simulasi dari 1000 nilai yang
didistribusikan secara normal menggunakan apa yang disebut diagram
kotak (box plot). Diagram ini menunjukkan median, kuartil 25% dan 75%,
nilai minimal dan maksimal, dan outlier.


\>p=normal(10,1000); boxplot(p):


![images/Final%20Projek%20APLIKOM-725.png](images/Final%20Projek%20APLIKOM-725.png)

Untuk menghasilkan bilangan bulat acak, Euler memiliki inrandom. Mari
kita simulasikan lemparan dadu dan plot distribusinya.


Kita menggunakan fungsi getmultiplicities(v,x), yang menghitung
seberapa sering elemen v muncul di x. Kemudian kita plot hasilnya
menggunakan columnsplot().


\>k=intrandom(1,6000,6);  ...  
\>   columnsplot(getmultiplicities(1:6,k));  ...  
\>   ygrid(1000,color=red):


![images/Final%20Projek%20APLIKOM-726.png](images/Final%20Projek%20APLIKOM-726.png)

Untuk menghasilkan bilangan bulat acak, Euler memiliki inrandom. Mari
kita simulasikan lemparan dadu dan plot distribusinya.


Kita menggunakan fungsi getmultiplicities(v,x), yang menghitung
seberapa sering elemen v muncul di x. Kemudian kita plot hasilnya
menggunakan kolomplot().


\>randpint(1,1000,[0.4,0.1,0.5]); getmultiplicities(1:3,%)


    [413,  104,  483]

Euler dapat menghasilkan nilai acak dari lebih banyak distribusi.
Lihat referensinya.


Misalnya, kita coba distribusi eksponensial. Variabel acak kontinu X
dikatakan memiliki distribusi eksponensial, jika PDF-nya diberikan
oleh




dengan parameter


\>plot2d(randexponential(1,1000,2),\>distribution):


![images/Final%20Projek%20APLIKOM-727.png](images/Final%20Projek%20APLIKOM-727.png)

Untuk banyak distribusi, Euler dapat menghitung fungsi distribusi dan
inversnya.


\>plot2d("normaldis",-4,4): 


![images/Final%20Projek%20APLIKOM-728.png](images/Final%20Projek%20APLIKOM-728.png)

Berikut ini adalah salah satu cara untuk memplot kuantil.


\>plot2d("qnormal(x,1,1.5)",-4,6);  ...  
\>   plot2d("qnormal(x,1,1.5)",a=2,b=5,\>add,\>filled):


![images/Final%20Projek%20APLIKOM-729.png](images/Final%20Projek%20APLIKOM-729.png)



Peluang untuk berada di area hijau adalah sebagai berikut.


\>normaldis(5,1,1.5)-normaldis(2,1,1.5)


    0.248662156979

Ini dapat dihitung secara numerik dengan integral berikut.


\>gauss("qnormal(x,1,1.5)",2,5)


    0.248662156979

Mari kita bandingkan distribusi binomial dengan distribusi normal
dengan nilai rata-rata dan deviasi yang sama. Fungsi invbindis()
menyelesaikan interpolasi linier antara nilai integer.


\>invbindis(0.95,1000,0.5), invnormaldis(0.95,500,0.5\*sqrt(1000))


    525.516721219
    526.007419394

Fungsi qdis() adalah kerapatan distribusi chi-kuadrat. Seperti biasa,
Euler memetakan vektor ke fungsi ini. Jadi, kita memperoleh plot semua
distribusi chi-kuadrat dengan derajat 5 hingga 30 dengan mudah dengan
cara berikut.


\>plot2d("qchidis(x,(5:5:50)')",0,50):


![images/Final%20Projek%20APLIKOM-730.png](images/Final%20Projek%20APLIKOM-730.png)

Euler memiliki fungsi yang akurat untuk mengevaluasi distribusi. Mari
kita periksa chidis() dengan integral.


Penamaannya mencoba agar konsisten. Misalnya,


* 
distribusi chi-kuadrat adalah chidis(),

* 
fungsi inversnya adalah invchidis(),

* 
densitasnya adalah qchidis().


Komplemen distribusi (ekor atas) adalah chicdis().


\>chidis(1.5,2), integrate("qchidis(x,2)",0,1.5)


    0.527633447259
    0.527633447259

# Distribusi Diskrit

Untuk menentukan distribusi diskrit Anda sendiri, Anda dapat
menggunakan metode berikut.


Pertama, kita tetapkan fungsi distribusi.


\>wd = 0|((1:6)+[-0.01,0.01,0,0,0,0])/6


    [0,  0.165,  0.335,  0.5,  0.666667,  0.833333,  1]

Artinya adalah bahwa dengan probabilitas wd[i+1]-wd[i] kita
menghasilkan nilai acak i.


Ini hampir merupakan distribusi seragam. Mari kita definisikan
generator angka acak untuk ini. Fungsi find(v,x) menemukan nilai x
dalam vektor v. Fungsi ini juga berfungsi untuk vektor x.


\>function wrongdice (n,m) := find(wd,random(n,m))


Kesalahannya begitu halus sehingga kita hanya melihatnya pada
pengulangan yang sangat banyak.


\>columnsplot(getmultiplicities(1:6,wrongdice(1,1000000))):


![images/Final%20Projek%20APLIKOM-731.png](images/Final%20Projek%20APLIKOM-731.png)

Berikut ini adalah fungsi sederhana untuk memeriksa distribusi seragam
dari nilai 1...K dalam v. Kita menerima hasilnya, jika untuk semua
frekuensi


\>function checkrandom (v, delta=1) ...


      K=max(v); n=cols(v);
      fr=getfrequencies(v,1:K);
      return max(fr/n-1/K)<delta/sqrt(n);
      endfunction
</pre>
Memang fungsi tersebut menolak distribusi seragam.


\>checkrandom(wrongdice(1,1000000))


    0

Dan menerima generator acak bawaan.


\>checkrandom(intrandom(1,1000000,6))


    1

Kita dapat menghitung distribusi binomial. Pertama ada binomialsum(),
yang mengembalikan probabilitas i atau kurang dari n kali percobaan.


\>bindis(410,1000,0.4)


    0.751401349654

Fungsi Beta terbalik digunakan untuk menghitung interval kepercayaan
Clopper-Pearson untuk parameter p. Level default adalah alpha.


Arti dari interval ini adalah jika p berada di luar interval, hasil
yang diamati sebesar 410 dalam 1000 adalah langka.


\>clopperpearson(410,1000)


    [0.37932,  0.441212]

Perintah berikut adalah cara langsung untuk mendapatkan hasil di atas.
Namun untuk n yang besar, penjumlahan langsung tidak akurat dan
lambat.


\>p=0.4; i=0:410; n=1000; sum(bin(n,i)\*p^i\*(1-p)^(n-i))


    0.751401349655

Btw, invbinsum() menghitung kebalikan dari binomialsum().


\>invbindis(0.75,1000,0.4)


    409.932733047

Dalam Bridge, kita mengasumsikan 5 kartu yang beredar (dari 52) dalam
dua tangan (26 kartu). Mari kita hitung probabilitas distribusi yang
lebih buruk dari 3:2 (misalnya 0:5, 1:4, 4:1 atau 5:0).


\>2\*hypergeomsum(1,5,13,26)


    0.321739130435

Ada juga simulasi distribusi multinomial.


\>randmultinomial(10,1000,[0.4,0.1,0.5])


              407           101           492 
              365           109           526 
              396           111           493 
              387           105           508 
              402           104           494 
              419           103           478 
              385           107           508 
              409            98           493 
              405           100           495 
              416           118           466 

# Plotting Data

Untuk memplot data, kami mencoba hasil pemilu Jerman sejak 1990, yang
diukur dalam jumlah kursi.


\>BW := [ ...  
\>   1990,662,319,239,79,8,17; ...  
\>   1994,672,294,252,47,49,30; ...  
\>   1998,669,245,298,43,47,36; ...  
\>   2002,603,248,251,47,55,2; ...  
\>   2005,614,226,222,61,51,54; ...  
\>   2009,622,239,146,93,68,76; ...  
\>   2013,631,311,193,0,63,64];


Untuk para pihak, kami menggunakan serangkaian nama.


\>P:=["CDU/CSU","SPD","FDP","Gr","Li"];


Mari kita cetak persentasenya dengan baik.


Pertama-tama kita ekstrak kolom-kolom yang diperlukan. Kolom 3 hingga
7 adalah kursi masing-masing partai, dan kolom 2 adalah jumlah total
kursi. Kolom 3 adalah tahun pemilihan.


\>BT:=BW[,3:7]; BT:=BT/sum(BT); YT:=BW[,1]';


Kemudian kami mencetak statistik dalam bentuk tabel. Kami menggunakan
nama sebagai tajuk kolom, dan tahun sebagai tajuk untuk baris. Lebar
default untuk kolom adalah wc=10, tetapi kami lebih suka keluaran yang
lebih padat. Kolom akan diperluas untuk label kolom, jika perlu.


\>writetable(BT\*100,wc=6,dc=0,\>fixed,labc=P,labr=YT)


           CDU/CSU   SPD   FDP    Gr    Li
      1990      48    36    12     1     3
      1994      44    38     7     7     4
      1998      37    45     6     7     5
      2002      41    42     8     9     0
      2005      37    36    10     8     9
      2009      38    23    15    11    12
      2013      49    31     0    10    10

Perkalian matriks berikut ini mengekstrak jumlah persentase dari dua
partai besar yang menunjukkan bahwa partai-partai kecil telah
memperoleh dukungan di parlemen hingga tahun 2009.


\>BT1:=(BT.[1;1;0;0;0])'\*100


    [84.29,  81.25,  81.1659,  82.7529,  72.9642,  61.8971,  79.8732]

Ada juga plot statistik sederhana. Kita menggunakannya untuk
menampilkan garis dan titik secara bersamaan. Alternatifnya adalah
memanggil plot2d dua kali dengan &gt;add.


\>statplot(YT,BT1,"b"):


![images/Final%20Projek%20APLIKOM-732.png](images/Final%20Projek%20APLIKOM-732.png)

Tentukan beberapa warna untuk setiap pihak.


\>CP:=[rgb(0.5,0.5,0.5),red,yellow,green,rgb(0.8,0,0)];


Sekarang kita dapat memetakan hasil pemilu 2009 dan perubahannya ke
dalam satu plot menggunakan gambar. Kita dapat menambahkan vektor
kolom ke setiap plot.


\>figure(2,1);  ...  
\>   figure(1); columnsplot(BW[6,3:7],P,color=CP); ...  
\>   figure(2); columnsplot(BW[6,3:7]-BW[5,3:7],P,color=CP);  ...  
\>   figure(0):


![images/Final%20Projek%20APLIKOM-733.png](images/Final%20Projek%20APLIKOM-733.png)

Plot data menggabungkan baris-baris data statistik dalam satu plot.


\>J:=BW[,1]'; DP:=BW[,3:7]'; ...  
\>   dataplot(YT,BT',color=CP);  ...  
\>   labelbox(P,colors=CP,styles="[]",\>points,w=0.2,x=0.3,y=0.4):


![images/Final%20Projek%20APLIKOM-734.png](images/Final%20Projek%20APLIKOM-734.png)

Plot kolom 3D menunjukkan baris data statistik dalam bentuk kolom.
Kami memberikan label untuk baris dan kolom. Angle adalah sudut
pandang.


\>columnsplot3d(BT,scols=P,srows=YT, ...  
\>     angle=30°,ccols=CP):


![images/Final%20Projek%20APLIKOM-735.png](images/Final%20Projek%20APLIKOM-735.png)

Representasi lainnya adalah plot mosaik. Perhatikan bahwa kolom-kolom
plot mewakili kolom-kolom matriks di sini. Karena panjang label
CDU/CSU, kami mengambil jendela yang lebih kecil dari biasanya.


\>shrinkwindow(\>smaller);  ...  
\>   mosaicplot(BT',srows=YT,scols=P,color=CP,style="#"); ...  
\>   shrinkwindow():


![images/Final%20Projek%20APLIKOM-736.png](images/Final%20Projek%20APLIKOM-736.png)

Kita juga bisa membuat diagram lingkaran. Karena hitam dan kuning
membentuk koalisi, kita susun ulang unsur-unsurnya.


\>i=[1,3,5,4,2]; piechart(BW[6,3:7][i],color=CP[i],lab=P[i]):


![images/Final%20Projek%20APLIKOM-737.png](images/Final%20Projek%20APLIKOM-737.png)

Berikut adalah jenis plot yang lain.


\>starplot(normal(1,10)+4,lab=1:10,\>rays):


![images/Final%20Projek%20APLIKOM-738.png](images/Final%20Projek%20APLIKOM-738.png)

Beberapa plot dalam plot2d bagus untuk statika. Berikut adalah plot
impuls data acak, yang didistribusikan secara seragam dalam [0,1].


\>plot2d(makeimpulse(1:10,random(1,10)),\>bar):


![images/Final%20Projek%20APLIKOM-739.png](images/Final%20Projek%20APLIKOM-739.png)

Namun untuk data yang terdistribusi secara eksponensial, kita mungkin
memerlukan plot logaritmik.


\>logimpulseplot(1:10,-log(random(1,10))\*10):


![images/Final%20Projek%20APLIKOM-740.png](images/Final%20Projek%20APLIKOM-740.png)

Fungsi columnsplot() lebih mudah digunakan, karena hanya memerlukan
vektor nilai. Selain itu, fungsi ini dapat mengatur labelnya sesuai
keinginan kita, kami telah menunjukkannya dalam tutorial ini.


Berikut adalah aplikasi lain, tempat kita menghitung karakter dalam
kalimat dan memplot statistik.


\>v=strtochar("the quick brown fox jumps over the lazy dog"); ...  
\>   w=ascii("a"):ascii("z"); x=getmultiplicities(w,v); ...  
\>   cw=[]; for k=w; cw=cw|char(k); end; ...  
\>   columnsplot(x,lab=cw,width=0.05):


![images/Final%20Projek%20APLIKOM-741.png](images/Final%20Projek%20APLIKOM-741.png)

Anda juga dapat mengatur sumbu secara manual.


\>n=10; p=0.4; i=0:n; x=bin(n,i)\*p^i\*(1-p)^(n-i); ...  
\>   columnsplot(x,lab=i,width=0.05,<frame,<grid); ...  
\>   yaxis(0,0:0.1:1,style="-\>",\>left); xaxis(0,style="."); ...  
\>   label("p",0,0.25), label("i",11,0); ...  
\>   textbox(["Binomial distribution","with p=0.4"]):


![images/Final%20Projek%20APLIKOM-742.png](images/Final%20Projek%20APLIKOM-742.png)

Berikut ini adalah cara untuk memetakan frekuensi angka dalam sebuah
vektor.


Kita buat sebuah vektor bilangan acak integer 1 hingga 6.


\>v:=intrandom(1,10,10)


    [7,  8,  8,  10,  8,  3,  4,  4,  5,  2]

Lalu ekstrak angka-angka unik dalam v.


\>vu:=unique(v)


    [2,  3,  4,  5,  7,  8,  10]

Dan plot frekuensi pada kolom plot.


\>columnsplot(getmultiplicities(vu,v),lab=vu,style="/"):


![images/Final%20Projek%20APLIKOM-743.png](images/Final%20Projek%20APLIKOM-743.png)

Kami ingin menunjukkan fungsi untuk distribusi nilai empiris.


\>x=normal(1,20);


Fungsi empdist(x,vs) memerlukan array nilai yang diurutkan. Jadi, kita
harus mengurutkan x sebelum dapat menggunakannya.


\>xs=sort(x);


Kemudian kami memetakan distribusi empiris dan beberapa batang
kepadatan ke dalam satu petak. Alih-alih menggunakan petak batang
untuk distribusi, kali ini kami menggunakan petak gigi gergaji.


\>figure(2,1); ...  
\>   figure(1); plot2d("empdist",-4,4;xs); ...  
\>   figure(2); plot2d(histo(x,v=-4:0.2:4,<bar));  ...  
\>   figure(0):


![images/Final%20Projek%20APLIKOM-744.png](images/Final%20Projek%20APLIKOM-744.png)

Plot sebaran mudah dibuat di Euler dengan plot titik biasa. Grafik
berikut menunjukkan bahwa X dan X+Y jelas berkorelasi positif.


\>x=normal(1,100); plot2d(x,x+rotright(x),\>points,style=".."):


![images/Final%20Projek%20APLIKOM-745.png](images/Final%20Projek%20APLIKOM-745.png)

Sering kali, kita ingin membandingkan dua sampel dengan distribusi
yang berbeda. Hal ini dapat dilakukan dengan plot kuantil-kuantil.


Untuk pengujian, kita mencoba distribusi t-student dan distribusi
eksponensial.


\>x=randt(1,1000,5); y=randnormal(1,1000,mean(x),dev(x)); ...  
\>   plot2d("x",r=6,style="--",yl="normal",xl="student-t",\>vertical); ...  
\>   plot2d(sort(x),sort(y),\>points,color=red,style="x",\>add):


![images/Final%20Projek%20APLIKOM-746.png](images/Final%20Projek%20APLIKOM-746.png)

Plot tersebut dengan jelas menunjukkan bahwa nilai-nilai yang
terdistribusi normal cenderung lebih kecil di ujung-ujung ekstrem.


Jika kita memiliki dua distribusi dengan ukuran yang berbeda, kita
dapat memperluas yang lebih kecil atau mengecilkan yang lebih besar.
Fungsi berikut ini bagus untuk keduanya. Fungsi ini mengambil nilai
median dengan persentase antara 0 dan 1.


\>function medianexpand (x,n) := median(x,p=linspace(0,1,n-1));


Mari kita bandingkan dua distribusi yang sama.


\>x=random(1000); y=random(400); ...  
\>   plot2d("x",0,1,style="--"); ...  
\>   plot2d(sort(medianexpand(x,400)),sort(y),\>points,color=red,style="x",\>add):


![images/Final%20Projek%20APLIKOM-747.png](images/Final%20Projek%20APLIKOM-747.png)

# Regresi dan Korelasi

Regresi linier dapat dilakukan dengan fungsi polyfit() atau berbagai
fungsi fit.


Sebagai permulaan, kita mencari garis regresi untuk data univariat
dengan polyfit(x,y,1).


\>x=1:10; y=[2,3,1,5,6,3,7,8,9,8]; writetable(x'|y',labc=["x","y"])


             x         y
             1         2
             2         3
             3         1
             4         5
             5         6
             6         3
             7         7
             8         8
             9         9
            10         8

Kami ingin membandingkan kecocokan yang tidak tertimbang dan
tertimbang. Pertama, koefisien kecocokan linier.


\>p=polyfit(x,y,1)


    [0.733333,  0.812121]

Sekarang koefisien dengan bobot yang menekankan nilai terakhir.


\>w &= "exp(-(x-10)^2/10)"; pw=polyfit(x,y,1,w=w(x))


    [4.71566,  0.38319]

Kami memasukkan semuanya ke dalam satu plot untuk titik dan garis
regresi, dan untuk bobot yang digunakan.


\>figure(2,1);  ...  
\>   figure(1); statplot(x,y,"b",xl="Regression"); ...  
\>     plot2d("evalpoly(x,p)",\>add,color=blue,style="--"); ...  
\>     plot2d("evalpoly(x,pw)",5,10,\>add,color=red,style="--"); ...  
\>   figure(2); plot2d(w,1,10,\>filled,style="/",fillcolor=red,xl=w); ...  
\>   figure(0):


![images/Final%20Projek%20APLIKOM-748.png](images/Final%20Projek%20APLIKOM-748.png)

Untuk contoh lain, kami membaca survei siswa, usia mereka, usia orang
tua mereka, dan jumlah saudara kandung dari sebuah berkas.


Tabel ini berisi "m" dan "f" di kolom kedua. Kami menggunakan variabel
tok2 untuk mengatur terjemahan yang tepat alih-alih membiarkan
readtable() mengumpulkan terjemahan.


\>{MS,hd}:=readtable("table1.dat",tok2:=["m","f"]);  ...  
\>   writetable(MS,labc=hd,tok2:=["m","f"]);


    Could not open the file
    table1.dat
    for reading!
    Try "trace errors" to inspect local variables after errors.
    readtable:
        if filename!=none then open(filename,"r"); endif;

Bagaimana usia saling bergantung? Kesan pertama datang dari diagram
sebaran berpasangan.


\>scatterplots(tablecol(MS,3:5),hd[3:5]):


    Variable or function MS not found.
    Error in:
    scatterplots(tablecol(MS,3:5),hd[3:5]): ...
                            ^

Jelas bahwa usia ayah dan ibu saling bergantung. Mari kita tentukan
dan gambarkan garis regresinya.


\>cs:=MS[,4:5]'; ps:=polyfit(cs[1],cs[2],1)


    MS is not a variable!
    Error in:
    cs:=MS[,4:5]'; ps:=polyfit(cs[1],cs[2],1) ...
                ^

Ini jelas model yang salah. Garis regresi adalah s=17+0,74t, di mana t
adalah usia ibu dan s adalah usia ayah. Perbedaan usia mungkin sedikit
bergantung pada usia, tetapi tidak terlalu banyak.


Sebaliknya, kami menduga fungsi seperti s=a+t. Maka a adalah rata-rata
s-t. Itu adalah perbedaan usia rata-rata antara ayah dan ibu.


\>da:=mean(cs[2]-cs[1])


    cs is not a variable!
    Error in:
    da:=mean(cs[2]-cs[1]) ...
                  ^

Mari kita gambarkan ini menjadi satu diagram sebar.


\>plot2d(cs[1],cs[2],\>points);  ...  
\>   plot2d("evalpoly(x,ps)",color=red,style=".",\>add);  ...  
\>   plot2d("x+da",color=blue,\>add):


    cs is not a variable!
    Error in:
    plot2d(cs[1],cs[2],&gt;points);  plot2d("evalpoly(x,ps)",color=re ...
                ^

Berikut ini adalah diagram kotak dari dua zaman tersebut. Ini hanya
menunjukkan bahwa zamannya berbeda.


\>boxplot(cs,["mothers","fathers"]):


    Variable or function cs not found.
    Error in:
    boxplot(cs,["mothers","fathers"]): ...
              ^

Menariknya bahwa perbedaan median tidak sebesar perbedaan mean.


\>median(cs[2])-median(cs[1])


    cs is not a variable!
    Error in:
    median(cs[2])-median(cs[1]) ...
                ^

Koefisien korelasi menunjukkan korelasi positif.


\>correl(cs[1],cs[2])


    cs is not a variable!
    Error in:
    correl(cs[1],cs[2]) ...
                ^

Korelasi peringkat adalah ukuran untuk urutan yang sama di kedua
vektor. Korelasi ini juga cukup positif.


\>rankcorrel(cs[1],cs[2])


    cs is not a variable!
    Error in:
    rankcorrel(cs[1],cs[2]) ...
                    ^

# Membuat Fungsi Baru

Tentu saja, bahasa EMT dapat digunakan untuk memprogram fungsi baru.
Misalnya, kita mendefinisikan fungsi skewness.


di mana m adalah rata-rata x.


\>function skew (x:vector) ...


    m=mean(x);
    return sqrt(cols(x))*sum((x-m)^3)/(sum((x-m)^2))^(3/2);
    endfunction
</pre>
Seperti yang Anda lihat, kita dapat dengan mudah menggunakan bahasa
matriks untuk mendapatkan implementasi yang sangat singkat dan
efisien. Mari kita coba fungsi ini.


\>data=normal(20); skew(normal(10))


    1.92013005365

Berikut adalah fungsi lainnya, yang disebut koefisien kemiringan
Pearson.


\>function skew1 (x) := 3\*(mean(x)-median(x))/dev(x)

\>skew1(data)


    0.113966137064

# Simulasi Monte Carlo

Euler dapat digunakan untuk mensimulasikan kejadian acak. Kita telah
melihat contoh sederhana di atas. Berikut ini contoh lain, yang
mensimulasikan 1000 kali lemparan 3 dadu, dan menanyakan distribusi
jumlahnya.


\>ds:=sum(intrandom(1000,3,6))';  fs=getmultiplicities(3:18,ds)


    [1,  16,  26,  44,  63,  102,  123,  103,  126,  119,  106,  87,  38,
    22,  18,  6]

We can plot this now.


\>columnsplot(fs,lab=3:18):


![images/Final%20Projek%20APLIKOM-749.png](images/Final%20Projek%20APLIKOM-749.png)

Menentukan distribusi yang diharapkan tidaklah mudah. ??Kami
menggunakan rekursi tingkat lanjut untuk ini.


Fungsi berikut menghitung jumlah cara bilangan k dapat
direpresentasikan sebagai jumlah n bilangan dalam rentang 1 hingga m.
Fungsi ini bekerja secara rekursif dengan cara yang jelas.


\>function map countways (k; n, m) ...


      if n==1 then return k>=1 && k<=m
      else
        sum=0; 
        loop 1 to m; sum=sum+countways(k-#,n-1,m); end;
        return sum;
      end;
    endfunction
</pre>
Berikut ini hasil dari tiga kali lemparan dadu.


\>countways(5:25,5,5)


    [1,  5,  15,  35,  70,  121,  185,  255,  320,  365,  381,  365,  320,
    255,  185,  121,  70,  35,  15,  5,  1]

\>cw=countways(3:18,3,6)


    [1,  3,  6,  10,  15,  21,  25,  27,  27,  25,  21,  15,  10,  6,  3,
    1]

Kami menambahkan nilai yang diharapkan ke plot.


\>plot2d(cw/6^3\*1000,\>add); plot2d(cw/6^3\*1000,\>points,\>add):


![images/Final%20Projek%20APLIKOM-750.png](images/Final%20Projek%20APLIKOM-750.png)

Untuk simulasi lain, deviasi nilai rata-rata dari n variabel acak
berdistribusi normal 0-1 adalah 1/akar(n).


\>longformat; 1/sqrt(10)


    0.316227766017

Mari kita periksa ini dengan simulasi. Kita hasilkan 10000 kali 10
vektor acak.


\>M=normal(10000,10); dev(mean(M)')


    0.316261483596

\>plot2d(mean(M)',\>distribution):


![images/Final%20Projek%20APLIKOM-751.png](images/Final%20Projek%20APLIKOM-751.png)

Median dari 10 bilangan acak berdistribusi normal 0-1 memiliki deviasi
yang lebih besar.


\>dev(median(M)')


    0.370232920635

Karena kita dapat dengan mudah menghasilkan lintasan acak, kita dapat
mensimulasikan proses Wiener. Kita mengambil 1000 langkah dari 1000
proses. Kemudian kita memetakan deviasi standar dan rata-rata langkah
ke-n dari proses ini bersama dengan nilai yang diharapkan dalam warna
merah.


\>n=1000; m=1000; M=cumsum(normal(n,m)/sqrt(m)); ...  
\>   t=(1:n)/n; figure(2,1); ...  
\>   figure(1); plot2d(t,mean(M')'); plot2d(t,0,color=red,\>add); ...  
\>   figure(2); plot2d(t,dev(M')'); plot2d(t,sqrt(t),color=red,\>add); ...  
\>   figure(0):


![images/Final%20Projek%20APLIKOM-752.png](images/Final%20Projek%20APLIKOM-752.png)

# Pengujian

Pengujian merupakan alat penting dalam statistik. Dalam Euler, banyak
pengujian yang diterapkan. Semua pengujian ini menghasilkan galat yang
kita terima jika kita menolak hipotesis nol.


Sebagai contoh, kita menguji lemparan dadu untuk distribusi seragam.
Pada 600 lemparan, kita memperoleh nilai berikut, yang kita masukkan
ke dalam uji chi-kuadrat.


\>chitest([90,103,114,101,103,89],dup(100,6)')


    0.498830517952

Uji chi-square juga memiliki modus, yang menggunakan simulasi Monte
Carlo untuk menguji statistik. Hasilnya harus hampir sama. Parameter
&gt;p menginterpretasikan vektor y sebagai vektor probabilitas.


\>chitest([90,103,114,101,103,89],dup(1/6,6)',\>p,\>montecarlo)


    0.482

Kesalahan ini terlalu besar. Jadi kita tidak dapat menolak distribusi
seragam. Ini tidak membuktikan bahwa dadu kita adil. Namun, kita tidak
dapat menolak hipotesis kita.


Selanjutnya, kita menghasilkan 1000 lemparan dadu menggunakan
generator angka acak, dan melakukan pengujian yang sama.


\>n=1000; t=random([1,n\*6]); chitest(count(t\*6,6),dup(n,6)')


    0.820257984345

Mari kita uji nilai rata-rata 100 dengan uji-t.


\>s=200+normal([1,100])\*10; ...  
\>   ttest(mean(s),dev(s),100,200)


    0.370593239652

Fungsi ttest() memerlukan nilai rata-rata, deviasi, jumlah data, dan
nilai rata-rata yang akan diuji.


Sekarang mari kita periksa dua pengukuran untuk nilai rata-rata yang
sama. Kita tolak hipotesis bahwa keduanya memiliki nilai rata-rata
yang sama, jika hasilnya &lt;0,05.


\>tcomparedata(normal(1,10),normal(1,10))


    0.202523792233

Jika kita menambahkan bias pada satu distribusi, kita akan mendapatkan
lebih banyak penolakan. Ulangi simulasi ini beberapa kali untuk
melihat efeknya.


\>tcomparedata(normal(1,10),normal(1,10)+2)


    5.91931730187e-06

Pada contoh berikutnya, kita buat 20 lemparan dadu acak sebanyak 100
kali dan hitung angka-angka yang ada di dalamnya. Rata-rata harus ada
20/6=3,3 angka.


\>R=random(100,20); R=sum(R\*6<=1)'; mean(R)


    3.39

Sekarang kita bandingkan jumlah angka satu dengan distribusi binomial.
Pertama kita gambarkan distribusi angka satu.


\>plot2d(R,distribution=max(R)+1,even=1,style="\\/"):


![images/Final%20Projek%20APLIKOM-753.png](images/Final%20Projek%20APLIKOM-753.png)

\>t=count(R,21);


Kemudian kita menghitung nilai yang diharapkan.


\>n=0:20; b=bin(20,n)\*(1/6)^n\*(5/6)^(20-n)\*100;


Kita harus mengumpulkan beberapa angka untuk mendapatkan kategori yang
cukup besar.


\>t1=sum(t[1:2])|t[3:7]|sum(t[8:21]); ...  
\>   b1=sum(b[1:2])|b[3:7]|sum(b[8:21]);


Uji chi-kuadrat menolak hipotesis bahwa distribusi kami adalah
distribusi binomial, jika hasilnya &lt; 0,05.


\>chitest(t1,b1)


    0.292756569915

Contoh berikut berisi hasil dua kelompok orang (misalnya laki-laki dan
perempuan) yang memilih 1 dari 6 partai. 


\>A=[23,37,43,52,64,74;27,39,41,49,63,76];  ...  
\>     writetable(A,wc=6,labr=["m","f"],labc=1:6)


               1     2     3     4     5     6
         m    23    37    43    52    64    74
         f    27    39    41    49    63    76

Kami ingin menguji independensi suara dari jenis kelamin. Uji tabel
chi^2 melakukan hal ini. Hasilnya terlalu besar untuk menolak
independensi. Jadi, kami tidak dapat mengatakan, apakah pemungutan
suara bergantung pada jenis kelamin dari data ini.


\>tabletest(A)


    0.990701632326

Berikut ini adalah tabel yang diharapkan, jika kita mengasumsikan
frekuensi pemungutan suara yang diamati.


\>writetable(expectedtable(A),wc=6,dc=1,labr=["m","f"],labc=1:6)


               1     2     3     4     5     6
         m  24.9  37.9  41.9  50.3  63.3  74.7
         f  25.1  38.1  42.1  50.7  63.7  75.3

Kita dapat menghitung koefisien kontingensi yang dikoreksi. Karena
sangat mendekati 0, kita simpulkan bahwa pemungutan suara tidak
bergantung pada jenis kelamin.


\>contingency(A)


    0.0427225484717

# Beberapa Pengujian Lainnya

Selanjutnya, kami menggunakan analisis varians (uji F) untuk menguji
tiga sampel data berdistribusi normal untuk nilai rata-rata yang sama.
Metode ini disebut ANOVA (analisis varians). Dalam Euler, fungsi
varanalysis() digunakan.


\>x1=[109,111,98,119,91,118,109,99,115,109,94]; mean(x1),


    106.545454545

\>x2=[120,124,115,139,114,110,113,120,117]; mean(x2),


    119.111111111

\>x3=[120,112,115,110,105,134,105,130,121,111]; mean(x3)


    116.3

\>varanalysis(x1,x2,x3)


    0.0138048221371

Artinya, kita menolak hipotesis nilai rata-rata yang sama. Kita
melakukan ini dengan probabilitas kesalahan sebesar 1,3%.


Ada juga uji median, yang menolak sampel data dengan distribusi
rata-rata yang berbeda dengan menguji median sampel gabungan.


\>a=[56,66,68,49,61,53,45,58,54];

\>b=[72,81,51,73,69,78,59,67,65,71,68,71];

\>mediantest(a,b)


    0.0241724220052

Uji kesetaraan lainnya adalah uji peringkat. Uji peringkat jauh lebih
tajam daripada uji median.


\>ranktest(a,b)


    0.00199969612469

Dalam contoh berikut, kedua distribusi memiliki rata-rata yang sama.


\>ranktest(random(1,100),random(1,50)\*3-1)


    0.0403890544389

Sekarang, mari kita coba simulasikan dua perawatan a dan b yang
diterapkan pada orang yang berbeda.


\>a=[8.0,7.4,5.9,9.4,8.6,8.2,7.6,8.1,6.2,8.9];

\>b=[6.8,7.1,6.8,8.3,7.9,7.2,7.4,6.8,6.8,8.1];


Uji signum memutuskan, apakah a lebih baik dari b.


\>signtest(a,b)


    0.0546875

Ini adalah kesalahan yang sangat besar. Kita tidak dapat menolak bahwa
a sama baiknya dengan b.


Uji Wilcoxon lebih tajam daripada uji ini, tetapi bergantung pada
nilai kuantitatif perbedaannya.


\>wilcoxon(a,b)


    0.0296680599405

Mari kita coba dua pengujian lagi menggunakan seri yang dihasilkan.


\>wilcoxon(normal(1,20),normal(1,20)-1)


    0.00499819423799

\>wilcoxon(normal(1,20),normal(1,20))


    0.275145971064

# Angka Acak

Berikut ini adalah pengujian untuk generator angka acak. Euler
menggunakan generator yang sangat bagus, jadi kita tidak perlu
mengharapkan masalah apa pun.


Pertama-tama kita menghasilkan sepuluh juta angka acak dalam [0,1].


\>n:=10000000; r:=random(1,n);


Next we count the distances between two numbers less than 0.05.


\>a:=0.05; d:=differences(nonzeros(r<a));


Terakhir, kami memplot berapa kali setiap jarak terjadi, dan
membandingkannya dengan nilai yang diharapkan.


\>m=getmultiplicities(1:100,d); plot2d(m); ...  
\>     plot2d("n\*(1-a)^(x-1)\*a^2",color=red,\>add):


![images/Final%20Projek%20APLIKOM-754.png](images/Final%20Projek%20APLIKOM-754.png)

Bersihkan datanya


\>remvalue n;


# Pendahuluan bagi Pengguna Proyek R

Jelas, EMT tidak bersaing dengan R sebagai paket statistik. Akan
tetapi, ada banyak prosedur dan fungsi statistik yang tersedia di EMT
juga. Jadi, EMT dapat memenuhi kebutuhan dasar. Lagi pula, EMT
dilengkapi dengan paket numerik dan sistem aljabar komputer.


Buku catatan ini ditujukan bagi Anda yang sudah familier dengan R,
tetapi perlu mengetahui perbedaan sintaksis EMT dan R. Kami mencoba
memberikan gambaran umum tentang hal-hal yang jelas dan kurang jelas
yang perlu Anda ketahui.


Selain itu, kami melihat cara untuk bertukar data antara kedua sistem.


Harap dicatat bahwa ini adalah pekerjaan yang masih dalam tahap
pengerjaan.


# Sintaksis Dasar

Hal pertama yang Anda pelajari di R adalah membuat vektor. Dalam EMT,
perbedaan utamanya adalah operator : dapat mengambil ukuran langkah.
Selain itu, operator ini memiliki daya pengikatan yang rendah.


\>n=10; 0:n/20:n-1


    [0,  0.5,  1,  1.5,  2,  2.5,  3,  3.5,  4,  4.5,  5,  5.5,  6,  6.5,
    7,  7.5,  8,  8.5,  9]

Fungsi c() tidak ada. Dimungkinkan untuk menggunakan vektor guna
menggabungkan berbagai hal.


Contoh berikut ini, seperti banyak contoh lainnya, berasal dari
"Interoduction to R" yang disertakan dalam proyek R. Jika Anda membaca
PDF ini, Anda akan menemukan bahwa saya mengikuti alurnya dalam
tutorial ini.


\>x=[10.4, 5.6, 3.1, 6.4, 21.7]; [x,0,x]


    [10.4,  5.6,  3.1,  6.4,  21.7,  0,  10.4,  5.6,  3.1,  6.4,  21.7]

Operator titik dua dengan ukuran langkah EMT digantikan oleh fungsi
seq() di R. Kita dapat menulis fungsi ini dalam EMT.


\>function seq(a,b,c) := a:b:c; ...  
\>   seq(0,-0.1,-1)


    [0,  -0.1,  -0.2,  -0.3,  -0.4,  -0.5,  -0.6,  -0.7,  -0.8,  -0.9,  -1]

Fungsi rep() dari R tidak ada dalam EMT. Untuk input vektor, dapat
ditulis sebagai berikut.


\>function rep(x:vector,n:index) := flatten(dup(x,n)); ...  
\>   rep(x,2)


    [10.4,  5.6,  3.1,  6.4,  21.7,  10.4,  5.6,  3.1,  6.4,  21.7]

Perhatikan bahwa "=" atau ":=" digunakan untuk penugasan. Operator
"-&gt;" digunakan untuk unit dalam EMT.


\>125km -\> " miles"


    77.6713990297 miles

Operator "&lt;-" untuk penugasan menyesatkan dan bukan ide yang baik
untuk R. Berikut ini akan membandingkan a dan -4 dalam EMT.


\>a=2; a<-4


    0

Dalam R, "a&lt;-4&lt;3" berfungsi, tetapi "a&lt;-4&lt;-3" tidak. Saya juga
mengalami ambiguitas serupa dalam EMT, tetapi mencoba menghilangkannya
sedikit demi sedikit.


EMT dan R memiliki vektor bertipe boolean. Namun dalam EMT, angka 0
dan 1 digunakan untuk mewakili false dan true. Dalam R, nilai true dan
false tetap dapat digunakan dalam aritmatika biasa seperti dalam EMT.


\>x<5, %\*x


    [0,  0,  1,  0,  0]
    [0,  0,  3.1,  0,  0]

EMT memunculkan kesalahan atau menghasilkan NAN, tergantung pada tanda
"kesalahan".


\>errors off; 0/0, isNAN(sqrt(-1)), errors on;


    NAN
    1

String sama di R dan EMT. Keduanya berada di lokal saat ini, bukan di
Unicode.


Di R ada paket untuk Unicode. Di EMT, string dapat berupa string
Unicode. String unicode dapat diterjemahkan ke pengodean lokal dan
sebaliknya. Selain itu, u"..." dapat berisi entitas HTML.


\>u"&#169; Ren&eacut; Grothmann"


    © René Grothmann

Berikut ini mungkin atau mungkin tidak ditampilkan dengan benar pada
sistem Anda sebagai A dengan titik dan garis di atasnya. Hal ini
bergantung pada font yang Anda gunakan.


\>chartoutf([480])


    Ǡ

Penggabungan string dilakukan dengan "+" atau "|". String dapat
menyertakan angka, yang akan dicetak dalam format saat ini.


\>"pi = "+pi


    pi = 3.14159265359

# Pengindeksan

Sebagian besar waktu, ini akan bekerja seperti pada R.


Tetapi EMT akan menginterpretasikan indeks negatif dari bagian
belakang vektor, sementara R menginterpretasikan x[n] sebagai x tanpa
elemen ke-n.


\>x, x[1:3], x[-2]


    [10.4,  5.6,  3.1,  6.4,  21.7]
    [10.4,  5.6,  3.1]
    6.4

Perilaku R dapat dicapai dalam EMT dengan drop().


\>drop(x,2)


    [10.4,  3.1,  6.4,  21.7]

Vektor logika tidak diperlakukan secara berbeda dengan indeks di EMT,
berbeda dengan R. Anda harus mengekstrak elemen-elemen yang bukan nol
terlebih dahulu di EMT.


\>x, x\>5, x[nonzeros(x\>5)]


    [10.4,  5.6,  3.1,  6.4,  21.7]
    [1,  1,  0,  1,  1]
    [10.4,  5.6,  6.4,  21.7]

Sama seperti di R, vektor indeks dapat berisi pengulangan.


\>x[[1,2,2,1]]


    [10.4,  5.6,  5.6,  10.4]

Namun pemberian nama untuk indeks tidak dimungkinkan dalam EMT. Untuk
paket statistik, hal ini mungkin sering diperlukan untuk memudahkan
akses ke elemen-elemen vektor.


Untuk meniru perilaku ini, kita dapat mendefinisikan sebuah fungsi
sebagai berikut.


\>function sel (v,i,s) := v[indexof(s,i)]; ...  
\>   s=["first","second","third","fourth"]; sel(x,["first","third"],s)


    
    Trying to overwrite protected function sel!
    Error in:
    function sel (v,i,s) := v[indexof(s,i)]; ... ...
                 ^
    
    Trying to overwrite protected function sel!
    Error in:
    function sel (v,i,s) := v[indexof(s,i)]; ... ...
                 ^
    
    Trying to overwrite protected function sel!
    Error in:
    function sel (v,i,s) := v[indexof(s,i)]; ... ...
                 ^
    
    Trying to overwrite protected function sel!
    Error in:
    function sel (v,i,s) := v[indexof(s,i)]; ... ...
                 ^
    
    Trying to overwrite protected function sel!
    Error in:
    function sel (v,i,s) := v[indexof(s,i)]; ... ...
                 ^
    [10.4,  3.1]

# Tipe Data

EMT memiliki lebih banyak tipe data tetap daripada R. Jelas, di R
terdapat vektor yang terus bertambah. Anda dapat menetapkan vektor
numerik kosong v dan menetapkan nilai ke elemen v[17]. Hal ini tidak
mungkin dilakukan di EMT.


Berikut ini agak tidak efisien.


\>v=[]; for i=1 to 10000; v=v|i; end;


EMT sekarang akan membuat vektor dengan v dan i yang ditambahkan pada
tumpukan dan menyalin vektor itu kembali ke variabel global v.


Yang lebih efisien mendefinisikan vektor terlebih dahulu.


\>v=zeros(10000); for i=1 to 10000; v[i]=i; end;


Untuk mengubah jenis tanggal di EMT, Anda dapat menggunakan fungsi
seperti complex().


\>complex(1:4)


    [ 1+0i ,  2+0i ,  3+0i ,  4+0i  ]

Konversi ke string hanya dimungkinkan untuk tipe data dasar. Format
saat ini digunakan untuk penggabungan string sederhana. Namun, ada
fungsi seperti print() atau frac().


Untuk vektor, Anda dapat dengan mudah menulis fungsi Anda sendiri.


\>function tostr (v) ...


    s="[";
    loop 1 to length(v);
       s=s+print(v[#],2,0);
       if #<length(v) then s=s+","; endif;
    end;
    return s+"]";
    endfunction
</pre>
\>tostr(linspace(0,1,10))


    [0.00,0.10,0.20,0.30,0.40,0.50,0.60,0.70,0.80,0.90,1.00]

Untuk komunikasi dengan Maxima, terdapat fungsi convertmxm(), yang
juga dapat digunakan untuk memformat vektor untuk keluaran.


\>convertmxm(1:10)


    [1,2,3,4,5,6,7,8,9,10]

Untuk Latex perintah tex dapat digunakan untuk mendapatkan perintah
Latex.


\>tex(&[1,2,3])


    \left[ 1 , 2 , 3 \right] 

# Faktor dan Tabel

Dalam pengantar R terdapat contoh dengan apa yang disebut faktor.


Berikut ini adalah daftar wilayah dari 30 negara bagian.


\>austates = ["tas", "sa", "qld", "nsw", "nsw", "nt", "wa", "wa", ...  
\>   "qld", "vic", "nsw", "vic", "qld", "qld", "sa", "tas", ...  
\>   "sa", "nt", "wa", "vic", "qld", "nsw", "nsw", "wa", ...  
\>   "sa", "act", "nsw", "vic", "vic", "act"];


Asumsikan, kita memiliki pendapatan yang sesuai di setiap negara
bagian.


\>incomes = [60, 49, 40, 61, 64, 60, 59, 54, 62, 69, 70, 42, 56, ...  
\>   61, 61, 61, 58, 51, 48, 65, 49, 49, 41, 48, 52, 46, ...  
\>   59, 46, 58, 43];


Sekarang, kita ingin menghitung rata-rata pendapatan di wilayah
tersebut. Sebagai program statistik, R memiliki factor() dan tappy()
untuk ini.


EMT dapat melakukan ini dengan menemukan indeks wilayah dalam daftar
wilayah yang unik.


\>auterr=sort(unique(austates)); f=indexofsorted(auterr,austates)


    [6,  5,  4,  2,  2,  3,  8,  8,  4,  7,  2,  7,  4,  4,  5,  6,  5,  3,
    8,  7,  4,  2,  2,  8,  5,  1,  2,  7,  7,  1]

Pada titik tersebut, kita dapat menulis fungsi loop kita sendiri untuk
melakukan sesuatu hanya untuk satu faktor.


Atau kita dapat meniru fungsi tapply() dengan cara berikut.


\>function map tappl (i; f$:call, cat, x) ...


    u=sort(unique(cat));
    f=indexof(u,cat);
    return f$(x[nonzeros(f==indexof(u,i))]);
    endfunction
</pre>
Agak tidak efisien, karena menghitung wilayah unik untuk setiap i,
tetapi berhasil.


\>tappl(auterr,"mean",austates,incomes)


    [44.5,  57.3333333333,  55.5,  53.6,  55,  60.5,  56,  52.25]

Perhatikan bahwa ini berfungsi untuk setiap vektor wilayah.


\>tappl(["act","nsw"],"mean",austates,incomes)


    [44.5,  57.3333333333]

Sekarang, paket statistik EMT mendefinisikan tabel seperti di R.
Fungsi readtable() dan writetable() dapat digunakan untuk input dan
output.


Jadi kita dapat mencetak pendapatan negara rata-rata di wilayah dengan
cara yang mudah.


\>writetable(tappl(auterr,"mean",austates,incomes),labc=auterr,wc=7)


        act    nsw     nt    qld     sa    tas    vic     wa
       44.5  57.33   55.5   53.6     55   60.5     56  52.25

Kita juga dapat mencoba meniru perilaku R sepenuhnya.


Faktor-faktor tersebut harus disimpan dalam suatu koleksi dengan jenis
dan kategori (negara bagian dan teritori dalam contoh kita). Untuk
EMT, kita tambahkan indeks yang telah dihitung sebelumnya.


\>function makef (t) ...


    ## Factor data
    ## Returns a collection with data t, unique data, indices.
    ## See: tapply
    u=sort(unique(t));
    return {{t,u,indexofsorted(u,t)}};
    endfunction
</pre>
\>statef=makef(austates);


Now the third element of the collection will contain the indices.


\>statef[3]


    [6,  5,  4,  2,  2,  3,  8,  8,  4,  7,  2,  7,  4,  4,  5,  6,  5,  3,
    8,  7,  4,  2,  2,  8,  5,  1,  2,  7,  7,  1]

Sekarang kita dapat meniru tapply() dengan cara berikut. Fungsi ini
akan mengembalikan tabel sebagai kumpulan data tabel dan judul kolom.


\>function tapply (t:vector,tf,f$:call) ...


    ## Makes a table of data and factors
    ## tf : output of makef()
    ## See: makef
    uf=tf[2]; f=tf[3]; x=zeros(length(uf));
    for i=1 to length(uf);
       ind=nonzeros(f==i);
       if length(ind)==0 then x[i]=NAN;
       else x[i]=f$(t[ind]);
       endif;
    end;
    return {{x,uf}};
    endfunction
</pre>
Kami tidak menambahkan banyak pemeriksaan tipe di sini. Satu-satunya
tindakan pencegahan menyangkut kategori (faktor) tanpa data. Namun,
seseorang harus memeriksa panjang t yang benar dan kebenaran koleksi
tf.


Tabel ini dapat dicetak sebagai tabel dengan writetable().


\>writetable(tapply(incomes,statef,"mean"),wc=7)


        act    nsw     nt    qld     sa    tas    vic     wa
       44.5  57.33   55.5   53.6     55   60.5     56  52.25

# Array

EMT hanya memiliki dua dimensi untuk array. Tipe data ini disebut
matriks. Akan mudah untuk menulis fungsi untuk dimensi yang lebih
tinggi atau pustaka C untuk ini.


R memiliki lebih dari dua dimensi. Dalam R, array adalah vektor dengan
bidang dimensi.


Dalam EMT, vektor adalah matriks dengan satu baris. Vektor dapat
dibuat menjadi matriks dengan redim().


\>shortformat; X=redim(1:20,4,5)


            1         2         3         4         5 
            6         7         8         9        10 
           11        12        13        14        15 
           16        17        18        19        20 

Ekstraksi baris dan kolom, atau sub-matriks, sangat mirip di R.


\>X[,2:3]


            2         3 
            7         8 
           12        13 
           17        18 

Namun, dalam R dimungkinkan untuk menetapkan daftar indeks vektor
tertentu ke suatu nilai. Hal yang sama dimungkinkan dalam EMT hanya
dengan loop.


\>function setmatrixvalue (M, i, j, v) ...


    loop 1 to max(length(i),length(j),length(v))
       M[i{#},j{#}] = v{#};
    end;
    endfunction
</pre>
Kami mendemonstrasikan ini untuk menunjukkan bahwa matriks dilewatkan
dengan referensi dalam EMT. Jika Anda tidak ingin mengubah matriks
asli M, Anda perlu menyalinnya dalam fungsi tersebut.


\>setmatrixvalue(X,1:3,3:-1:1,0); X,


            1         2         0         4         5 
            6         0         8         9        10 
            0        12        13        14        15 
           16        17        18        19        20 

Produk luar dalam EMT hanya dapat dilakukan antara vektor. Hal ini
dilakukan secara otomatis karena bahasa matriks. Satu vektor harus
berupa vektor kolom dan yang lainnya berupa vektor baris.


\>(1:5)\*(1:5)'


            1         2         3         4         5 
            2         4         6         8        10 
            3         6         9        12        15 
            4         8        12        16        20 
            5        10        15        20        25 

Dalam pengantar PDF untuk R terdapat sebuah contoh, yang menghitung
distribusi ab-cd untuk a,b,c,d yang dipilih secara acak dari 0 hingga
n. Solusi dalam R adalah membentuk matriks 4 dimensi dan menjalankan
table() di atasnya.


Tentu saja, ini dapat dicapai dengan loop. Namun, loop tidak efektif
dalam EMT atau R. Dalam EMT, kita dapat menulis loop dalam C dan itu
akan menjadi solusi tercepat.


Namun, kita ingin meniru perilaku R. Untuk ini, kita perlu meratakan
perkalian ab dan membuat matriks ab-cd.


\>a=0:6; b=a'; p=flatten(a\*b); q=flatten(p-p'); ...  
\>   u=sort(unique(q)); f=getmultiplicities(u,q); ...  
\>   statplot(u,f,"h"):


![images/Final%20Projek%20APLIKOM-755.png](images/Final%20Projek%20APLIKOM-755.png)

Selain multiplisitas yang tepat, EMT dapat menghitung frekuensi dalam
vektor.


\>getfrequencies(q,-50:10:50)


    [0,  23,  132,  316,  602,  801,  333,  141,  53,  0]

Cara termudah untuk memplot ini sebagai distribusi adalah sebagai
berikut.


\>plot2d(q,distribution=11):


![images/Final%20Projek%20APLIKOM-756.png](images/Final%20Projek%20APLIKOM-756.png)

Namun, Anda juga dapat menghitung terlebih dahulu jumlah dalam
interval yang dipilih. Tentu saja, berikut ini menggunakan
getfrequencies() secara internal.


Karena fungsi histo() mengembalikan frekuensi, kita perlu
menskalakannya sehingga integral di bawah grafik batang adalah 1.


\>{x,y}=histo(q,v=-55:10:55); y=y/sum(y)/differences(x); ...  
\>   plot2d(x,y,\>bar,style="/"):


![images/Final%20Projek%20APLIKOM-757.png](images/Final%20Projek%20APLIKOM-757.png)

# Daftar

EMT memiliki dua jenis daftar. Satu adalah daftar global yang dapat
diubah, dan yang lainnya adalah jenis daftar yang tidak dapat diubah.
Kami tidak peduli dengan daftar global di sini.


Jenis daftar yang tidak dapat diubah disebut koleksi dalam EMT. Ia
berperilaku seperti struktur dalam C, tetapi elemennya hanya diberi
nomor dan tidak diberi nama.


\>L={{"Fred","Flintstone",40,[1990,1992]}}


    Fred
    Flintstone
    40
    [1990,  1992]

Saat ini unsur-unsur tersebut tidak memiliki nama, meskipun nama dapat
ditetapkan untuk tujuan khusus. Unsur-unsur tersebut diakses dengan
angka.


\>(L[4])[2]


    1992

# Input dan Output File (Membaca dan Menulis Data)

Anda sering kali ingin mengimpor matriks data dari sumber lain ke EMT.
Tutorial ini memberi tahu Anda tentang berbagai cara untuk
mencapainya. Fungsi sederhana adalah writematrix() dan readmatrix().


Mari kita tunjukkan cara membaca dan menulis vektor bilangan real ke
dalam file.


\>a=random(1,100); mean(a), dev(a),


    0.52438
    0.294

Untuk menulis data ke dalam berkas, kami menggunakan fungsi
writematrix().


Karena pengantar ini kemungkinan besar berada di dalam direktori,
tempat pengguna tidak memiliki akses tulis, kami menulis data ke
direktori beranda pengguna. Untuk buku catatan sendiri, ini tidak
diperlukan, karena berkas data akan ditulis ke dalam direktori yang
sama.


\>filename="test.dat";


Sekarang kita tulis vektor kolom a' ke dalam berkas. Ini menghasilkan
satu angka di setiap baris berkas.


\>writematrix(a',filename);


Untuk membaca data, kita menggunakan readmatrix().


\>a=readmatrix(filename)';


Dan hapus berkasnya.


\>fileremove(filename);

\>mean(a), dev(a),


    0.52438
    0.294

Fungsi writematrix() atau writetable() dapat dikonfigurasi untuk
bahasa lain.


Misalnya, jika Anda memiliki sistem bahasa Indonesia (titik desimal
dengan koma), Excel Anda memerlukan nilai dengan koma desimal yang
dipisahkan oleh titik koma dalam file csv (nilai default dipisahkan
dengan koma). File berikut "test.csv" akan muncul di folder Anda saat
ini.


\>filename="test.csv"; ...  
\>   writematrix(random(5,3),file=filename,separator=",");


Anda sekarang dapat membuka berkas ini langsung dengan Excel
Indonesia.


\>fileremove(filename);


Terkadang kita memiliki string dengan token seperti berikut.


\>s1:="f m m f m m m f f f m m f";  ...  
\>   s2:="f f f m m f f";


Untuk menokenisasi ini, kami mendefinisikan vektor token.


\>tok:=["f","m"]


    f
    m

Lalu kita dapat menghitung berapa kali setiap token muncul dalam
string, dan memasukkan hasilnya ke dalam tabel.


\>M:=getmultiplicities(tok,strtokens(s1))\_ ...  
\>     getmultiplicities(tok,strtokens(s2));


Tulis tabel dengan tajuk token.


\>writetable(M,labc=tok,labr=1:2,wc=8)


                   f       m
           1       6       7
           2       5       2

Untuk statika, EMT dapat membaca dan menulis tabel.


\>file="test.dat"; open(file,"w"); ...  
\>   writeln("A,B,C"); writematrix(random(3,3)); ...  
\>   close();


Berkasnya tampak seperti ini.


\>printfile(file)


    A,B,C
    0.7404999942251013,0.584865092166482,0.3793594964060733
    0.6731183688226442,0.535007020680046,0.7951663097316103
    0.7118359131301066,0.2093402910017989,0.8909297435213943
    

Fungsi readtable() dalam bentuk yang paling sederhana dapat membacanya
dan mengembalikan kumpulan nilai dan baris judul.


\>L=readtable(file,\>list);


Koleksi ini dapat dicetak dengan writetable() ke buku catatan, atau ke
berkas.


\>writetable(L,wc=10,dc=5)


             A         B         C
        0.7405   0.58487   0.37936
       0.67312   0.53501   0.79517
       0.71184   0.20934   0.89093

Matriks nilai adalah elemen pertama dari L. Perhatikan bahwa mean()
dalam EMT menghitung nilai rata-rata dari baris-baris matriks.


\>mean(L[1])


      0.56824 
      0.66776 
      0.60404 

# File CSV

Pertama, mari kita tulis sebuah matriks ke dalam sebuah file. Untuk
keluarannya, kami membuat file di direktori kerja saat ini.


\>file="test.csv";  ...  
\>   M=random(3,3); writematrix(M,file);


Berikut ini adalah isi file ini.


\>printfile(file)


    0.659260833187574,0.1794141480932956,0.7518861996523696
    0.3262164405213657,0.05388767532094028,0.04699178226026776
    0.6281208388462063,0.3095795215639562,0.1824435296038631
    

CVS ini dapat dibuka di sistem bahasa Inggris ke Excel dengan klik dua
kali. Jika Anda mendapatkan file seperti itu pada sistem Jerman, Anda
perlu mengimpor data ke Excel dengan memperhatikan titik desimal.


Namun, titik desimal juga merupakan format default untuk EMT. Anda
dapat membaca sebuah matriks dari sebuah file dengan readmatrix().


\>readmatrix(file)


      0.65926   0.17941   0.75189 
      0.32622  0.053888  0.046992 
      0.62812   0.30958   0.18244 

Dimungkinkan untuk menulis beberapa matriks ke dalam satu file.
Perintah open() dapat membuka file untuk menulis dengan parameter “w”.
Standarnya adalah “r” untuk membaca.


\>open(file,"w"); writematrix(M); writematrix(M'); close();


Matriks-matriks tersebut dipisahkan oleh sebuah baris kosong. Untuk
membaca matriks, buka file dan panggil readmatrix() beberapa kali.


\>open(file); A=readmatrix(); B=readmatrix(); A==B, close();


            1         0         0 
            0         1         0 
            0         0         1 

Di Excel atau spreadsheet serupa, Anda dapat mengekspor matriks
sebagai CSV (nilai yang dipisahkan dengan koma). Pada Excel 2007,
gunakan “save as” dan “format lain”, lalu pilih “CSV”. Pastikan, tabel
saat ini hanya berisi data yang ingin Anda ekspor.


Berikut ini adalah contohnya.


\>printfile("excel-data.csv")


    Could not open the file
    excel-data.csv
    for reading!
    Try "trace errors" to inspect local variables after errors.
    printfile:
        open(filename,"r");

Seperti yang Anda lihat, sistem Jerman saya menggunakan titik koma
sebagai pemisah dan koma desimal. Anda dapat mengubahnya di pengaturan
sistem atau di Excel, tetapi tidak perlu untuk membaca matriks ke
dalam EMT.


Cara termudah untuk membaca ini ke dalam Euler adalah readmatrix().
Semua koma digantikan oleh titik dengan parameter &gt;comma. Untuk CSV
bahasa Inggris, hilangkan saja parameter ini.


\>M=readmatrix("excel-data.csv",\>comma)


    Could not open the file
    excel-data.csv
    for reading!
    Try "trace errors" to inspect local variables after errors.
    readmatrix:
        if filename&lt;&gt;"" then open(filename,"r"); endif;

Mari kita plotkan.


\>plot2d(M'[1],M'[2:3],\>points,color=[red,green]'):


![images/Final%20Projek%20APLIKOM-758.png](images/Final%20Projek%20APLIKOM-758.png)

Ada beberapa cara yang lebih mendasar untuk membaca data dari file.
Anda dapat membuka file dan membaca angka baris demi baris. Fungsi
getvectorline() akan membaca angka dari sebuah baris data. Secara
default, fungsi ini mengharapkan sebuah titik desimal. Tetapi fungsi
ini juga dapat menggunakan koma desimal, jika Anda memanggil
setdecimaldot(“,”) sebelum menggunakan fungsi ini.


Fungsi berikut ini adalah contohnya. Fungsi ini akan berhenti pada
akhir file atau baris kosong.


\>function myload (file) ...


    open(file);
    M=[];
    repeat
       until eof();
       v=getvectorline(3);
       if length(v)>0 then M=M_v; else break; endif;
    end;
    return M;
    close(file);
    endfunction
</pre>
\>myload(file)


      0.65926         0   0.17941         0   0.75189 
      0.32622         0  0.053888         0  0.046992 
      0.62812         0   0.30958         0   0.18244 

Anda juga dapat membaca semua angka dalam file tersebut dengan
getvector().


\>open(file); v=getvector(10000); close(); redim(v[1:9],3,3)


      0.65926         0   0.17941 
            0   0.75189   0.32622 
            0  0.053888         0 

Dengan demikian, sangat mudah untuk menyimpan vektor nilai, satu nilai
di setiap baris dan membaca kembali vektor ini.


\>v=random(1000); mean(v)


    0.49903

\>writematrix(v',file); mean(readmatrix(file)')


    0.49903

# Menggunakan Tabel

Tabel dapat digunakan untuk membaca atau menulis data numerik. Sebagai
contoh, kita menulis tabel dengan judul baris dan kolom ke file.


\>file="test.tab"; M=random(3,3);  ...  
\>   open(file,"w");  ...  
\>   writetable(M,separator=",",labc=["one","two","three"]);  ...  
\>   close(); ...  
\>   printfile(file)


    one,two,three
          0.23,      0.45,       0.5
          0.79,      0.59,      0.22
          0.31,      0.38,      0.86

File ini dapat diimpor ke Excel.


Untuk membaca file di EMT, kita menggunakan readtable().


\>{M,headings}=readtable(file,\>clabs); ...  
\>   writetable(M,labc=headings)


           one       two     three
          0.23      0.45       0.5
          0.79      0.59      0.22
          0.31      0.38      0.86

# Menganalisis Garis

Anda bahkan dapat mengevaluasi setiap baris dengan tangan. Misalkan,
kita memiliki baris dengan format berikut.


\>line="2020-11-03,Tue,1'114.05"


    2020-11-03,Tue,1'114.05

Pertama-tama kita bisa membuat token pada garis.


\>vt=strtokens(line)


    2020-11-03
    Tue
    1'114.05

Kemudian, kita dapat mengevaluasi setiap elemen garis dengan
menggunakan evaluasi yang sesuai.


\>day(vt[1]),  ...  
\>   indexof(["mon","tue","wed","thu","fri","sat","sun"],tolower(vt[2])),  ...  
\>   strrepl(vt[3],"'","")()


    7.3816e+05
    2
    1114

Dengan menggunakan ekspresi reguler, dimungkinkan untuk mengekstrak
hampir semua informasi dari sebaris data.


Asumsikan kita memiliki baris berikut sebagai dokumen HTML.


\>line="<tr\><td\>1145.45</td\><td\>5.6</td\><td\>-4.5</td\><tr\>"


    &lt;tr&gt;&lt;td&gt;1145.45&lt;/td&gt;&lt;td&gt;5.6&lt;/td&gt;&lt;td&gt;-4.5&lt;/td&gt;&lt;tr&gt;

Untuk mengekstraknya, kami menggunakan ekspresi reguler, yang mencari


* 
tanda kurung tutup &gt;,

* 
string apa pun yang tidak mengandung tanda kurung dengan
* sub-kecocokan "(...)",

* 
tanda kurung buka dan tutup menggunakan solusi terpendek,

* 
lagi-lagi string apa pun yang tidak mengandung tanda kurung,

* 
dan tanda kurung buka &lt;.


Ekspresi reguler agak sulit dipelajari tetapi sangat ampuh.


\>{pos,s,vt}=strxfind(line,"\>([^<\>]+)<.+?\>([^<\>]+)<");


Hasilnya adalah posisi kecocokan, string yang cocok, dan vektor string
untuk sub-kecocokan.


\>for k=1:length(vt); vt[k](), end;


    1145.5
    5.6

Berikut adalah fungsi yang membaca semua item numerik antara &lt;td&gt; dan
&lt;/td&gt;.


\>function readtd (line) ...


    v=[]; cp=0;
    repeat
       {pos,s,vt}=strxfind(line,"<td.*?>(.+?)</td>",cp);
       until pos==0;
       if length(vt)>0 then v=v|vt[1]; endif;
       cp=pos+strlen(s);
    end;
    return v;
    endfunction
</pre>
\>readtd(line+"<td\>non-numerical</td\>")


    1145.45
    5.6
    -4.5
    non-numerical

# Membaca dari Web

Situs web atau berkas dengan URL dapat dibuka di EMT dan dapat dibaca
baris demi baris.


Dalam contoh ini, kami membaca versi terkini dari situs EMT. Kami
menggunakan ekspresi reguler untuk memindai "Versi ..." dalam judul.


\>function readversion () ...


    urlopen("http://www.euler-math-toolbox.de/Programs/Changes.html");
    repeat
      until urleof();
      s=urlgetline();
      k=strfind(s,"Version ",1);
      if k>0 then substring(s,k,strfind(s,"<",k)-1), break; endif;
    end;
    urlclose();
    endfunction
</pre>
\>readversion


    Version 2024-01-12

# Input dan Output Variabel

Anda dapat menulis variabel dalam bentuk definisi Euler ke dalam file
atau ke baris perintah.


\>writevar(pi,"mypi");


    mypi = 3.141592653589793;

Untuk pengujian, kami membuat file Euler di direktori kerja EMT.


\>file="test.e"; ...  
\>   writevar(random(2,2),"M",file); ...  
\>   printfile(file,3)


    M = [ ..
    0.4132433618072819, 0.8689094301579993;
    0.5472658716689791, 0.7762000691038584];

Sekarang kita dapat memuat file tersebut. Berkas tersebut akan
mendefinisikan matriks M.


\>load(file); show M,


    M = 
      0.41324   0.86891 
      0.54727    0.7762 

Jika writevar() digunakan pada suatu variabel, ia akan mencetak
definisi variabel dengan nama variabel ini.


\>writevar(M); writevar(inch$)


    M = [ ..
    0.4132433618072819, 0.8689094301579993;
    0.5472658716689791, 0.7762000691038584];
    inch$ = 0.0254;

Kita juga dapat membuka berkas baru atau menambahkannya ke berkas yang
sudah ada. Dalam contoh ini, kita menambahkannya ke berkas yang dibuat
sebelumnya.


\>open(file,"a"); ...  
\>   writevar(random(2,2),"M1"); ...  
\>   writevar(random(3,1),"M2"); ...  
\>   close();

\>load(file); show M1; show M2;


    M1 = 
       0.8448   0.30699 
      0.81725   0.55952 
    M2 = 
      0.93476 
      0.41779 
      0.48677 

Untuk menghapus file apa pun gunakan fileremove().


\>fileremove(file);


Vektor baris dalam sebuah berkas tidak memerlukan koma, jika setiap
angka berada di baris baru. Mari kita buat berkas seperti itu, tulis
setiap baris satu per satu dengan writeln().


\>open(file,"w"); writeln("M = ["); ...  
\>   for i=1 to 5; writeln(""+random()); end; ...  
\>   writeln("];"); close(); ...  
\>   printfile(file)


    M = [
    0.365095139497
    0.718027309064
    0.451787105949
    0.517348066892
    0.158148874269
    ];

\>load(file); M


    [0.3651,  0.71803,  0.45179,  0.51735,  0.15815]

## Latihan Soal



1. Analisis data statistika deskriptif


\>mean([1250,2170,1276,2175,1277,2168,1245,2130,1215,2171,1269,2184,1215,2188,1290])


    1681.5

\>data=[4185, 9360, 490, 1900, 721, 8240];

\>urutan=sort(data)


    [490,  721,  1900,  4185,  8240,  9360]

\>median([urutan])


    3042.5

\>data=[543, 879, 654, 910, 765, 128, 99,49,26,27];

\>urutqn=sort(data)


    [26,  27,  49,  99,  128,  543,  654,  765,  879,  910]

\>xbar=mean(urutan)


    4149.3

\>dev= urutan-xbar 


    [-3659.3,  -3428.3,  -2249.3,  35.667,  4090.7,  5210.7]

\>varians=mean(dev^2)


    1.2348e+07

\>data=[705,660,900,980,280,270,275,255,350,390];

\>urut=sort(data)


    [255,  270,  275,  280,  350,  390,  660,  705,  900,  980]

\>x=mean(urut)


    506.5

\>dev=urut-x


    [-251.5,  -236.5,  -231.5,  -226.5,  -156.5,  -116.5,  153.5,  198.5,
    393.5,  473.5]

\>varians=mean(dev^2)


    70415

\>simpanganbaku= sqrt(varians)


    265.36

\>x=[255,  270,  275,  280,  350,  390,  630,60,78,90,96,74,55,79,90]; max(x)- min(x)


    575

\>data=[280,  350,  390,  630,60,78,90,96,74,557,669];

\>urut=sort(data)


    [60,  74,  78,  90,  96,  280,  350,  390,  557,  630,  669]

\>quartiles(urut)


    [60,  78,  280,  557,  669]

2. Carilah rata-rata dan standar deviasi beserta plot dari data
berikut


X = 2300,2540,2850,3050,4500,5080


\>X=[2300,2540,2850,3050,4500,5080]; ...  
\>   mean(X), dev(X),


    3386.7
    1131.9

\>aspect(1.5); boxplot(X):


![images/Final%20Projek%20APLIKOM-759.png](images/Final%20Projek%20APLIKOM-759.png)

3. Menggambar Grafik Statistika!


Diketahui data ukuran sepatu siswa di suatu sekolahan


\>A=[40,42,45,45,41,38,39,40,42,44,35,36,38,39,40,41,39,38,37,36,40,43,42,41]


    [40,  42,  45,  45,  41,  38,  39,  40,  42,  44,  35,  36,  38,  39,
    40,  41,  39,  38,  37,  36,  40,  43,  42,  41]

Penjelasan diagram kotak tersebut adalah. Dapat diketahui nilai
minimum sebesar 35, Q1=38, Median (Q2) = 40, Q3=42. Dan nilai
maksimumnya adalah 45. Sebaran data tersebut juga diketahui simetris,
karena si kuartil 1 dan 2 jaraknya sama dengan kuartil 2 dan 3.


Contoh lain perbandingan 15 simulasi 500 nilai terdistribusi normal
menggunakan box plot dan ditemukan pencilan sbb


\>boxplot(A):


![images/Final%20Projek%20APLIKOM-760.png](images/Final%20Projek%20APLIKOM-760.png)

\>p=normal(15,500); boxplot(p):


![images/Final%20Projek%20APLIKOM-761.png](images/Final%20Projek%20APLIKOM-761.png)

3. Kita akan membuat diagram batang secara random


\>columnsplot(cumsum(random(6)),style="/",color=red):


![images/Final%20Projek%20APLIKOM-762.png](images/Final%20Projek%20APLIKOM-762.png)

\>columnsplot(cumsum(random(15)),style="-",color=black):


![images/Final%20Projek%20APLIKOM-763.png](images/Final%20Projek%20APLIKOM-763.png)

\>columnsplot(cumsum(random(3)),style="|",color=orange):


![images/Final%20Projek%20APLIKOM-764.png](images/Final%20Projek%20APLIKOM-764.png)

\>ay=["Senin","Selasa","Rabu","Kamis","Jumat","Sabtu","Minggu"];

\>values=[30,40,20,10,50,60,70];

\>columnsplot(values,lab=day,color=yellow);


    Function day needs at least one argument!
    Use: day (y {, m: integer scalar, d: integer scalar, h: integer scalar, min: number, ...}) 
    Error in:
    columnsplot(values,lab=day,color=yellow); ...
                              ^

\>title("Data Penjualan Perhari di Toko Watashi")


\>CP:=[rgb(0.5,0.5,0.5),red,yellow,green,rgb(0.9,0,0)]


    [5.8753e+07,  2,  15,  3,  6.5405e+07]

\>insimg


![images/Final%20Projek%20APLIKOM-765.png](images/Final%20Projek%20APLIKOM-765.png)

\>CP:=[rgb(0.5,0.5,0.5),red,yellow,green,rgb(0.9,0,0)]


    [5.8753e+07,  2,  15,  3,  6.5405e+07]

\>i=[1,2,3,4,5]; piechart(values[i],color=CP[i],lab=day[i]):


    day is not a variable!
    Error in:
    ... 3,4,5]; piechart(values[i],color=CP[i],lab=day[i]): ...
                                                         ^

\>starplot(normal(1,15)+16,lab=1:15,\>rays):


![images/Final%20Projek%20APLIKOM-766.png](images/Final%20Projek%20APLIKOM-766.png)

\>starplot(values,lab=day,\>rays):


    Function day needs at least one argument!
    Use: day (y {, m: integer scalar, d: integer scalar, h: integer scalar, min: number, ...}) 
    Error in:
    starplot(values,lab=day,&gt;rays): ...
                           ^

\>plot2d(makeimpulse(1:20,random(1,20)),\>bar):


![images/Final%20Projek%20APLIKOM-767.png](images/Final%20Projek%20APLIKOM-767.png)

\>logimpulseplot(1:20,-log(random(1,20))\*10):


![images/Final%20Projek%20APLIKOM-768.png](images/Final%20Projek%20APLIKOM-768.png)

\>aspect(1); plot2d(random(100),\>histogram):


![images/Final%20Projek%20APLIKOM-769.png](images/Final%20Projek%20APLIKOM-769.png)

\>r=150:5:185; v=[22,71,136,150,139,71,32];

\>plot2d(r,v,a=150,b=185,c=0,d=150,bar=1,style="/"):


![images/Final%20Projek%20APLIKOM-770.png](images/Final%20Projek%20APLIKOM-770.png)

\>plot2d("qnormal(x,0,1)",-5,5); ...  
\>   plot2d("qnormal(x,0,1)",a=1,b=4,\>add,\>filled):


![images/Final%20Projek%20APLIKOM-771.png](images/Final%20Projek%20APLIKOM-771.png)

Baris tersebut akan menghasilkan suatu nilai acak dari distribusi
normal dengan me
Contoh kurva fungsi distribusi kumulatif kontinu terdiri atas tiga
bagian yaitu


1. Bernilai 0 untuk x dibawah minimal dari daerah rentang


2. Merupakan fungsi monoton naik pada daerah rentang


3. Mempunyai nilai konstan 1 diatas batas maksimum daerah rentangnya


\>x=normal(1,6);

\>xs=sort(x);

\>plot2d("empdist",-3,5;xs):


![images/Final%20Projek%20APLIKOM-772.png](images/Final%20Projek%20APLIKOM-772.png)

Grafik fungsi distribusi kumulatif peubah acak diskrit merupakan
fungsi tangga dengan terendah 0 dan tertinggi 1


# Rujukan Lengkap Fungsi plot2d()

  function plot2d (xv, yv, btest, a, b, c, d, xmin, xmax, r, n,  ..  
  logplot, grid, frame, framecolor, square, color, thickness, style, ..  
  auto, add, user, delta, points, addpoints, pointstyle, bar, histogram,  ..  
  distribution, even, steps, own, adaptive, hue, level, contour,  ..  
  nc, filled, fillcolor, outline, title, xl, yl, maps, contourcolor, ..  
  contourwidth, ticks, margin, clipping, cx, cy, insimg, spectral,  ..  
  cgrid, vertical, smaller, dl, niveau, levels)  

Multipurpose plot function for plots in the plane (2D plots). This function can do
plots of functions of one variables, data plots, curves in the plane, bar plots, grids
of complex numbers, and implicit plots of functions of two variables.


Parameters




x,y       : equations, functions or data vectors


a,b,c,d   : Plot area (default a=-2,b=2)


r         : if r is set, then a=cx-r, b=cx+r, c=cy-r, d=cy+r


            r can be a vector [rx,ry] or a vector [rx1,rx2,ry1,ry2].


xmin,xmax : range of the parameter for curves


auto      : Determine y-range automatically (default)


square    : if true, try to keep square x-y-ranges


n         : number of intervals (default is adaptive)


grid      : 0 = no grid and labels,


            1 = axis only,


            2 = normal grid (see below for the number of grid lines)


            3 = inside axis


            4 = no grid


            5 = full grid including margin


            6 = ticks at the frame


            7 = axis only


            8 = axis only, sub-ticks


frame     : 0 = no frame


framecolor: color of the frame and the grid


margin    : number between 0 and 0.4 for the margin around the plot


color     : Color of curves. If this is a vector of colors,


            it will be used for each row of a matrix of plots. In the case of


            point plots, it should be a column vector. If a row vector or a


            full matrix of colors is used for point plots, it will be used for


            each data point.


thickness : line thickness for curves


            This value can be smaller than 1 for very thin lines.


style     : Plot style for lines, markers, and fills.


            For points use


            "[]", "&lt;&gt;", ".", "..", "...",


            "*", "+", "|", "-", "o"


            "[]#", "&lt;&gt;#", "o#" (filled shapes)


            "[]w", "&lt;&gt;w", "ow" (non-transparent)


            For lines use


            "-", "--", "-.", ".", ".-.", "-.-", "-&gt;"


            For filled polygons or bar plots use


            "#", "#O", "O", "/", "\", "\/",


            "+", "|", "-", "t"


points    : plot single points instead of line segments


addpoints : if true, plots line segments and points


add       : add the plot to the existing plot


user      : enable user interaction for functions


delta     : step size for user interaction


bar       : bar plot (x are the interval bounds, y the interval values)


histogram : plots the frequencies of x in n subintervals


distribution=n : plots the distribution of x with n subintervals


even      : use inter values for automatic histograms.


steps     : plots the function as a step function (steps=1,2)


adaptive  : use adaptive plots (n is the minimal number of steps)


level     : plot level lines of an implicit function of two variables


outline   : draws boundary of level ranges.




If the level value is a 2xn matrix, ranges of levels will be drawn


in the color using the given fill style. If outline is true, it


will be drawn in the contour color. Using this feature, regions of


f(x,y) between limits can be marked.




hue       : add hue color to the level plot to indicate the function


            value


contour   : Use level plot with automatic levels


nc        : number of automatic level lines


title     : plot title (default "")


xl, yl    : labels for the x- and y-axis


smaller   : if &gt;0, there will be more space to the left for labels.


vertical  :


  Turns vertical labels on or off. This changes the global variable


  verticallabels locally for one plot. The value 1 sets only vertical


  text, the value 2 uses vertical numerical labels on the y axis.


filled    : fill the plot of a curve


fillcolor : fill color for bar and filled curves


outline   : boundary for filled polygons


logplot   : set logarithmic plots


            1 = logplot in y,


            2 = logplot in xy,


            3 = logplot in x


own       :


  A string, which points to an own plot routine. With &gt;user, you get


  the same user interaction as in plot2d. The range will be set


  before each call to your function.


maps      : map expressions (0 is faster), functions are always mapped.


contourcolor : color of contour lines


contourwidth : width of contour lines


clipping  : toggles the clipping (default is true)


title     :


  This can be used to describe the plot. The title will appear above


  the plot. Moreover, a label for the x and y axis can be added with


  xl="string" or yl="string". Other labels can be added with the


  functions label() or labelbox(). The title can be a unicode


  string or an image of a Latex formula.


cgrid     :


  Determines the number of grid lines for plots of complex grids.


  Should be a divisor of the the matrix size minus 1 (number of


  subintervals). cgrid can be a vector [cx,cy].


Overview


The function can plot


* 
expressions, call collections or functions of one variable,

* 
parametric curves,

* 
x data against y data,

* 
implicit functions,

* 
bar plots,

* 
complex grids,

* 
polygons.


If a function or expression for xv is given, plot2d() will compute


values in the given range using the function or expression. The


expression must be an expression in the variable x. The range must


be defined in the parameters a and b unless the default range


[-2,2] should be used. The y-range will be computed automatically,


unless c and d are specified, or a radius r, which yields the range


[-r,r] for x and y. For plots of functions, plot2d will use an


adaptive evaluation of the function by default. To speed up the


plot for complicated functions, switch this off with &lt;adaptive, and


optionally decrease the number of intervals n. Moreover, plot2d()


will by default use mapping. I.e., it will compute the plot element


for element. If your expression or your functions can handle a


vector x, you can switch that off with &lt;maps for faster evaluation.


Note that adaptive plots are always computed element for element. 


If functions or expressions for both xv and for yv are specified,


plot2d() will compute a curve with the xv values as x-coordinates


and the yv values as y-coordinates. In this case, a range should be


defined for the parameter using xmin, xmax. Expressions contained

