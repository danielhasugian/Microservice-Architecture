## Definition
Merupakan teknik design arsitektur yang bertujuan untuk membuat aplikasi dapat berjalan sesuai dengan bisnis meskipun bisnis complex, teknologi yang kompleks dan pengguna banyak. Tujuan utama dari microservices adalah untuk membuat aplikasi dapat ramah terhadap perubahan dan kokoh terhadap permintaan.

Berikut ini beberapa definisi Microservices
* **Wikipedia**
- Microservices is a variant of the service-oriented architecture (SOA) architectural style that structures an application as a collection of loosely coupled services. In a microservices architecture, services should be fine-grained and the protocols should be lightweight.

* **Chris Richardson**
- Microservices is an architectural style that structures an application as a collection of loosely coupled services, which implement business capabilities.

## How to work
Teknik bekerja dengan cara memecah service besar menjadi service kecil yang dapat berdiri sendiri dan tidak tergantung pada apapun, tujuan dari pemecahan tersebut agar service dapat berjalan dengan baik secara fungsinya dan tidak menggangu kinerja dari setiap service. 

## Problems
* Business complex
* Technology complex
* Too many client using application
* Too many developer 

## Discussion
### Di saat ini dalam membuat suatu product bukan hanya:
* Apakah dapat berjalan sesuai dengan fungsinya ?
* Client suka dengan product kita atau tidak ?
* Tidak ada bug atau issue ?
### Melainkan 
* Apakah arsitektur sudah sesuai ?
* Bagaimana dengan pengembangan terhadap fitur-fitur baru ?
* Bagaimana dengan request client yang padat?

Dari case diatas, dapat diambil kesimpulan bahwa perlu **perencanaan yang matang** sangatlah diperlukan sebelum membangun suatu aplikasi. Microservices merupakan arsitektur dapat menjawab issue-issue tersebut, dengan melakukan pemecahan service menjadi service kecil dapat menurunkan kinerja service dan menaikkan peformance dari sisi layanan.

Contoh ilustrasi produk microservices, ketika membangun aplikasi ecommerce yang dimana dibagi menjadi service-service kecil seperti payment, order, barang, user, dll dapat diilustrasikan sebagai berikut :
* Ketika banyak merchant yang ingin menjual barangnya maka dia akan mengimport semua data ke dalam aplikasi, dalam hal ini yang bekerja hanyalah service barang, dan service yang lainnya tidak melakukan apapun
* Ketika terjadi banyak pembelian oleh user maka service yang berjalan hanyalah payment dan service yang lainnya tidak melakukan apapun.

Dari case diatas dapat dilihat bahwa service yang bekerja adalah service yang sesuai dengan bisnisnya saja dan bagaimana bila dalam service tersebut terlalu padat ini akan menyebabkan terjadi overloaded dan blocking, untuk case tersebut service yang mempunyai bobot paling berat dapat direplika sehingga bobot yang begitu berat dapat di bagi ke service lain sehingga peformance dari layanan tetaplah maksimal.

## Conclusion
Microservice merupakan suatu teknik untuk membuat aplikasi yang dapat berjalan maksimal dan mudah mengembangkan fitur baru.

## Refrences link
* [Telegeram Microservices Indonesia](https://telegram.dog/msarchitecture)
* [Microservices](https://smartbear.com/learn/api-design/what-are-microservices/) 
* [Microservices](http://microservices.io/)
* [Microservices](https://martinfowler.com/articles/microservices.html)
