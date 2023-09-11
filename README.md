# Selamat Datang di Tutorial Golang

Sudah saatnya beralih ke Golang...

**Katanya Golang itu cepat**, performanya hampir mendekati C dan C++. 

Wah, mantap!

Belakangan ini, **Golang semakin banyak digunakan di backend**. Mungkin karena bahasa yang dikompilasi lebih aman digunakan di sisi server.

Jika seorang hacker berhasil meretas masuk ke server kita, dia hanya akan mendapatkan file binary, bukan file script terbuka seperti PHP atau JavaScript.

Sehingga jika dia ingin memahami lebih dalam tentang aplikasi kita, dia harus melakukan reverse engineering.

Ini adalah salah satu keunggulan yang ditawarkan oleh Golang.

Selain itu, masih banyak hal lain yang dapat kita lakukan dengan Golang.

Maka dari itu, mari kita mulai dengan mempelajari dasar-dasar pemrograman Golang agar kita dapat membuat aplikasi keren nantinya.

## Apa itu Golang?

Go, atau sering disebut Golang, adalah bahasa pemrograman yang dikembangkan oleh Google.

Golang adalah bahasa pemrograman yang **statically typed** (tipe datanya ditentukan secara statis), **compiled programming language** (bahasa pemrograman yang harus di-compile sebelum dijalankan), dan **sintaksisnya mirip dengan bahasa C**.

Apa artinya **statically typed** dan **compiled programming language**?

- **Statically typed** berarti kita harus mendefinisikan tipe data secara eksplisit. Hal ini membuat kode lebih aman karena pengecekan tipe data dilakukan selama proses kompilasi.
- **Compiled programming language** berarti kita perlu mengkompilasi kode menjadi binary sebelum menjalankannya.

Selain itu, Golang juga memiliki manajemen memori yang baik, termasuk **garbage collection** untuk membersihkan objek atau variabel yang tidak digunakan, sehingga membuat program lebih aman dari bug dan kerentanan seperti buffer overflow.

## Sejarah Singkat Golang

Pengembangan Golang dimotivasi oleh:

**"Ketidakpuasan terhadap bahasa pemrograman C++."**

Walaupun banyak kode di Google ditulis dengan C++, para pengembang merasa kurang produktif dengan bahasa tersebut. Inilah yang mendorong pengembangan bahasa pemrograman baru untuk menggantikan C++.

Ada tiga tokoh penting yang terlibat dalam pengembangan Golang:

- Robert Griesemer
- Rob Pike
- Ken Thompson

Golang dirancang pada tahun 2007 dan diumumkan ke publik pada tahun 2009. Versi pertama Golang, yaitu v1.0, dirilis pada tahun 2012. Hingga saat ini, Golang telah mencapai versi v1.19.

## Persiapan Alat untuk Belajar Golang

Ada dua alat yang perlu kita siapkan untuk memulai pemrograman Golang:

1. **Teks Editor untuk Coding Golang**: Anda dapat menggunakan teks editor apa saja, tetapi Visual Studio Code (VS Code) sangat direkomendasikan karena memiliki ekstensi yang memudahkan coding Golang.

2. **Golang Compiler**: Compiler ini digunakan untuk meng-compile program Golang menjadi binary dan menjalankannya. Instalasi Golang akan berbeda tergantung pada sistem operasi Anda.

### 1. Teks Editor untuk Coding Golang

Anda bebas menggunakan teks editor mana saja, tetapi saya merekomendasikan Visual Studio Code (VS Code). Anda dapat menginstal ekstensi Golang untuk mempermudah coding Golang di VS Code.

### 2. Install Golang Compiler

Proses instalasi Golang akan berbeda tergantung pada sistem operasi yang Anda gunakan. Di bawah ini adalah instruksi instalasi untuk Windows, Ubuntu, dan Fedora:

#### Install Golang di Windows

1. Unduh installer Golang dari [situs web resmi Golang](https://go.dev/dl/). Pilih file `.msi` untuk Windows.

2. Buka installer yang telah diunduh dan ikuti langkah-langkahnya. Pastikan Anda menyetujui EULA (End User License Agreement) selama proses instalasi.

3. Setelah instalasi selesai, buka command prompt (CMD) atau PowerShell, dan jalankan perintah berikut untuk memeriksa versi Golang yang terinstal:

   <code> go version </code>
#### Install Golang di Ubuntu
Anda dapat menginstal Golang di Ubuntu dengan menggunakan apt:

 <code> sudo apt install golang-go -y </code>

Setelah instalasi selesai, cek versi Golang dengan perintah go version.

#### Install Golang di Fedora
Di Fedora, Anda dapat menginstal Golang dengan perintah dnf:

<code> sudo dnf install golang </code>
Setelah instalasi selesai, cek versi Golang dengan perintah go version.

### 3. Setting Environment Variables
Setelah menginstal Golang, Anda perlu menyiapkan beberapa variabel lingkungan. Di Ubuntu dan Fedora, Anda perlu menambahkan GOPATH ke environment variables.

Jalankan perintah berikut di terminal:

<code>mkdir -p $HOME/go
echo 'export GOPATH=$HOME/go' >> $HOME/.profile
source $HOME/.profile </code> <br />
Pastikan variabel GOPATH telah diatur dengan benar dengan menjalankan <code> echo $GOPATH </code> di terminal.
