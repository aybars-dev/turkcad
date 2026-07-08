<p align="right">
  <a href="README.md">English</a> |
  <strong>Türkçe</strong>
</p>

# TurkCAD Web CAD Studio

<p align="center">
  <img src="assets/logo.svg" alt="TurkCAD logosu" width="96">
</p>

<p align="center">
  <strong>Teknik çizim, DXF iş akışları, ölçülendirme ve hafif taslak çalışmaları için tarayıcı tabanlı 2B CAD çalışma alanı.</strong>
</p>

<p align="center">
  <a href="https://turkcad.online">
    <img src="https://img.shields.io/badge/TurkCAD'i%20Aç-turkcad.online-9f1d35?style=for-the-badge&labelColor=202225" alt="TurkCAD'i Aç">
  </a>
  <img src="https://img.shields.io/badge/Sürüm-v0.1.8%20Alpha-9f1d35?style=for-the-badge&labelColor=202225" alt="v0.1.8 Alpha sürümü">
  <img src="https://img.shields.io/badge/Lisans-AGPL--3.0-9f1d35?style=for-the-badge&labelColor=202225" alt="AGPL-3.0 Lisansı">
</p>

---

## Hakkında

***TurkCAD***; teknik çizim, hafif taslak çalışmaları, DXF dosyalarını inceleme, ölçülendirme ve yaygın düzenleme işlemleri için geliştirilmiş tarayıcı tabanlı bir 2B CAD uygulamasıdır.

Proje aktif olarak geliştirilmektedir ve şu anda alpha aşamasındadır.

Kaynak kodu yakında herkese açık olarak yayımlanacaktır.
Bu depo şimdilik proje bilgilerini ve lisans ayrıntılarını içermektedir.

---

## Özellikler

* Tarayıcı tabanlı 2B CAD çalışma alanı
* Çizgi, Çoklu Çizgi, Dikdörtgen, Çember, Yay, Elips, Spline, Metin, Tarama ve Eksen Çizgisi araçları
* Taşıma, Kopyalama, Döndürme, Ölçeklendirme, Aynalama, Ofset, Kırpma, Uzatma, Birleştirme, Patlatma, Köşe Yuvarlama ve Silme komutları
* Hizalı, Doğrusal, Çap, Yarıçap ve Açısal ölçülendirme araçları
* Görünürlük, kilitleme, renk, çizgi tipi, çizgi kalınlığı ve çizgi tipi ölçeği kontrollerine sahip katman yönetimi
* Nesne Yakalama, Izgara Yakalama, Ortho, Akıllı Hizalama ve Polar İzleme desteği
* Uç noktalar, orta noktalar, merkezler ve yarıçap noktaları için tutamaç düzenleme sistemi
* DXF içe ve dışa aktarma desteği
* TurkCAD proje dosyalarını kaydetme ve yükleme
* PNG ve PDF olarak dışa aktarma
* Türkçe ve İngilizce arayüz
* Zorunlu bir sunucu altyapısına ihtiyaç duymayan statik web uygulaması mimarisi

---

## Ekran Görüntüleri

![TurkCAD teknik çizim örneği 1](assets/images/screenshot.jpeg)

![TurkCAD teknik çizim örneği 2](assets/images/screenshot2.jpg)

![TurkCAD teknik çizim örneği 3](assets/images/screenshot3.jpeg)

---

## Komut Referansı

TurkCAD, CAD programlarında kullanılan komut satırı sistemini ve kısa komutları destekler. Komut çubuğuna bir komut yazıp **Enter** tuşuna basarak çalıştırabilirsiniz. Yazım sırasında uygun komut önerileri otomatik olarak gösterilir.

<details>
<summary><strong>Çizim Komutları</strong></summary>

<br>

| Komut | Kısayol | Açıklama |
|---|---|---|
| `SELECT` | `S` | Nesne ve pencere ile seçim modunu etkinleştirir. |
| `LINE` | `L` | Nokta, uzunluk veya koordinat kullanarak hassas çizgi parçaları oluşturur. |
| `PLINE` | `PL` | Birbirine bağlı çoklu çizgi parçaları oluşturur. Bitirmek için Enter, kapatmak için `C` kullanılır. |
| `SPLINE` | `SPL` | Birden fazla kontrol noktasından geçen yumuşak bir eğri oluşturur. |
| `POINT` | `PO` | Teknik referans veya kontrol noktası yerleştirir. |
| `CENTERLINE` | `CL` | İki nokta arasında kesik merkez veya eksen çizgisi oluşturur. |
| `RECTANGLE` | `R`, `REC` | Köşe noktaları veya ölçüler kullanarak dikdörtgen çizer. |
| `CIRCLE` | `C` | Merkez ve yarıçap ya da çap kullanarak çember oluşturur. |
| `CIRCLE2P` | `C2P`, `2P` | İki çap uç noktasını kullanarak çember oluşturur. |
| `CIRCLE3P` | `C3P`, `3P` | Seçilen üç noktadan geçen bir çember oluşturur. |
| `CIRCLETTR` | `TTR` | İki nesneye teğet ve belirli yarıçapa sahip çember oluşturur. |
| `ARC` | `A` | Merkez tabanlı dairesel yay çizer. |
| `ARC2` | `A2` | Başlangıç noktası, bitiş noktası ve yarıçap veya çap kullanarak yay çizer. |
| `POLYGON` | `POL` | 3 ile 64 kenar arasında düzgün çokgen oluşturur. |
| `ELLIPSE` | `EL` | Merkez ve yarıçap değerlerini kullanarak elips çizer. |
| `ELLIPSEARC` | `EARC` | Eliptik yay oluşturur. |
| `HATCH` | `H` | Kapalı bir sınırın içine tarama deseni uygular. |
| `IMAGE` | `IMG` | Üzerinden çizim yapmak için yarı saydam referans görseli ekler. |
| `TEXT` | `T` | Seçilen taban çizgisi boyunca metin oluşturur. |

</details>

<details>
<summary><strong>Düzenleme Komutları</strong></summary>

<br>

| Komut | Kısayol | Açıklama |
|---|---|---|
| `MOVE` | `M` | Seçilen nesneleri bir taban noktası ve hedef noktası kullanarak taşır. |
| `COPY` | `CO` | Seçilen nesnelerin kopyalarını oluşturur. |
| `ROTATE` | `RO` | Seçilen nesneleri bir taban noktası etrafında döndürür. |
| `SCALE` | `SC` | Seçilen nesneleri bir taban noktasına göre ölçeklendirir. |
| `MIRROR` | `MI` | Seçilen nesneleri iki noktayla belirlenen eksene göre aynalar. |
| `OFFSET` | `O` | Desteklenen geometrilerin paralel veya eş merkezli kopyalarını oluşturur. |
| `ARRAY` | `AR` | Dikdörtgensel veya kutupsal çoğaltma iş akışını açar. |
| `RECTARRAY` | — | Satır, sütun ve aralık değerleriyle dikdörtgensel çoğaltma oluşturur. |
| `POLARARRAY` | — | Bir merkez noktası etrafında kutupsal çoğaltma oluşturur. |
| `TRIM` | `TR` | Geometrileri kesişen sınırlar üzerinden kırpar. |
| `EXTEND` | `EX` | Geometrileri seçilen sınıra kadar uzatır. |
| `FILLET` | `F` | Desteklenen nesneler arasında yuvarlatılmış veya teğet geçiş oluşturur. |
| `JOIN` | `J` | Uyumlu nesneleri birbirine bağlı geometri hâline getirir. |
| `EXPLODE` | `X` | Blokları ve desteklenen bileşik nesneleri düzenlenebilir parçalara ayırır. |
| `BLOCK` | `B` | Seçilen nesneleri yeniden kullanılabilir bir blok hâline getirir. |
| `ERASE` | `E`, `DEL` | Seçilen veya işaretlenen nesneleri siler. |

</details>

<details>
<summary><strong>Ölçülendirme ve Ölçüm Komutları</strong></summary>

<br>

| Komut | Kısayol | Açıklama |
|---|---|---|
| `DIM` | `D` | Varsayılan hizalı ölçülendirme modunu etkinleştirir. |
| `DIMALIGNED` | `DIMALI` | İki nokta arasında hizalı ölçü oluşturur. |
| `DIMLINEAR` | `DIMLIN`, `DLI` | Yatay veya dikey doğrusal ölçü oluşturur. |
| `DIMDIAMETER` | `DIMDIA`, `DDI` | Çember, yay veya elips için çap ölçüsü oluşturur. |
| `DIMRADIUS` | `DIMRAD`, `DRA` | Çember, yay veya elips için yarıçap ölçüsü oluşturur. |
| `DIMANGULAR` | `DIMANG`, `DAN` | İki çizgi veya çizgi parçası arasındaki açıyı ölçer. |
| `MEASURE` | `MEA`, `DIST` | İki nokta arasındaki mesafeyi ve açıyı ölçer. |

</details>

<details>
<summary><strong>Görünüm, Yakalama ve Yardımcı Komutlar</strong></summary>

<br>

| Komut | Kısayol | Açıklama |
|---|---|---|
| `FIT` | `ZE` | Görünür tüm çizim nesnelerini çalışma alanına sığdırır. |
| `PAN` | — | Geometrileri değiştirmeden çizim görünümünü hareket ettirir. |
| `GRID` | — | Çizim ızgarasını gösterir veya gizler. |
| `SNAP` | — | Izgaraya yakalama özelliğini açar veya kapatır. |
| `ORTHO` | — | Çizim hareketini yatay ve dikey doğrultularla sınırlar. |
| `OSNAP` | — | Nesne yakalama özelliğini açar veya kapatır. |
| `TANGENT` | `TAN` | Teğet nesne yakalama özelliğini açar veya kapatır. |
| `ALL` | `SELECTALL` | Görünür ve kilitli olmayan bütün nesneleri seçer. |
| `UNDO` | `U` | Son gerçekleştirilen çizim işlemini geri alır. |
| `REDO` | — | Son geri alınan işlemi yeniden uygular. |
| `HELP` | `?` | TurkCAD Yardım Merkezini açar. |

</details>

<details>
<summary><strong>Komut Girdileri ve Klavye Kısayolları</strong></summary>

<br>

| Girdi | İşlev |
|---|---|
| `X,Y` | Mutlak koordinat veya ölçü çifti girer. |
| `@X,Y` | Mevcut başlangıç noktasına göre göreceli koordinat girer. |
| `R25` | 25 birimlik yarıçap değeri girer. |
| `D50` | 50 birimlik çap değeri girer. |
| `LEN 250` | Seçilen çizginin uzunluğunu 250 birim olarak ayarlar. |
| `Enter` | Girilen değeri onaylar veya aktif komutu tamamlar. |
| `Esc` | Aktif adımı, komutu veya seçimi iptal eder. |
| `Delete` / `Backspace` | Seçilen nesneleri siler. |
| `Ctrl + A` | Görünür ve kilitli olmayan bütün nesneleri seçer. |
| `Ctrl + Z` | Son işlemi geri alır. |
| `Ctrl + Y` | Son geri alınan işlemi yeniden uygular. |
| `Tab` | Vurgulanan komut önerisini seçer. |

</details>

---

## Canlı Demo

TurkCAD’in herkese açık demo sürümüne aşağıdaki adresten erişebilirsiniz:

**https://turkcad.online**

---

## Geliştirme Durumu

TurkCAD aktif olarak geliştirilmektedir ve henüz tamamlanmamış özellikler, hatalar veya eksik iş akışları içerebilir.

Proje şu anda aşağıdaki kullanım alanları için uygundur:

* Hafif 2B CAD iş akışlarını test etmek
* DXF çizimlerini incelemek ve düzenlemek
* Basit teknik çizimler oluşturmak
* Tarayıcı tabanlı CAD teknolojilerini deneyimlemek
* Açık kaynaklı bir CAD projesine katkıda bulunmak

---

## Lisans

Bu proje **GNU Affero General Public License v3.0** lisansı altında yayımlanacaktır.

Ayrıntılı bilgi için [LICENSE.md](LICENSE.md) dosyasını inceleyebilirsiniz.

---

## Geliştirici

**Aybars Can** tarafından geliştirilmiştir.
