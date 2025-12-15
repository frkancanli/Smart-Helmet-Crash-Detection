# 🏍️ Akıllı Kask Kaza Algılama Sistemi (Smart Helmet Project)

Bu proje, motosiklet sürücülerinin güvenliğini artırmak amacıyla tasarlanmış bir **gömülü sistem prototipidir**.

## 🎯 Projenin Amacı
Motosiklet kazalarında "altın saat" kuralı hayatidir. Bu sistem, olası bir kaza anında sürücünün bilincini kontrol eder ve yanıt alamazsa otomatik olarak acil durum ekiplerine (112) haber verir.

## 🛠️ Nasıl Çalışır? (Algoritma)
Sistem **Input - Process - Output** mantığı üzerine kuruludur:

1.  **INPUT (Veri):** Kask üzerindeki ivmeölçer (G-Force) sensöründen veriler anlık okunur.
2.  **PROCESS (İşleme):**
    * Gelen veri 5g kuvvetinin üzerindeyse "Darbe" olarak algılanır.
    * Sistem sürücüye *"İyi misin?"* sorusunu yöneltir.
3.  **OUTPUT (Çıktı):**
    * Sürücü cevap verirse -> Sistem normale döner.
    * Cevap yoksa -> GPS konumu alınır ve 112'ye SMS atılır.

## 📊 Sistem Akış Şeması
Projenin çalışma mantığını gösteren blok diyagram:

![Akış Şeması][kaza yapıldı mı.jpg]



## 💻 Kullanılan Teknolojiler
* **Dil:** Python (Prototip aşaması)
* **Donanım Hedefi:** Raspberry Pi / Arduino + MPU6050 Sensör
* **Sensörler:** İvmeölçer, GPS Modülü

---
*Tasarım Dersi Projesi - 2025*
