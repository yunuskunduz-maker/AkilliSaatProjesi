# Maker Akıllı Saat Projesi (Arduino Pro Mini & HC-05)

Bu proje, **Arduino Pro Mini** ve **HC-05 Bluetooth modülü** kullanılarak sıfırdan tasarlanmış, **kompakt ve taşınabilir** bir akıllı saat prototipidir. Ana odak noktası, tüm bileşenlerin minimum yer kaplaması için yeniden düzenlenmesi ve bir mobil uygulama ile iki yönlü iletişim kurabilmesidir.

## Temel Özellikler

| Özellik | Açıklama |
| :--- | :--- |
| **Mobil Uygulama İletişimi** | Özel bir mobil uygulamaya (Android/iOS) bağlanabilme yeteneği. |
| **Uygulamadan Mesaj Gönderme** | Uygulama üzerinden saate anlık mesajlar veya bildirimler gönderebilme. |
| **Bağlantı Durumu Gösterimi** | Bluetooth bağlantısının ne zaman başladığına dair anlık geri bildirim ile kullanıcıya bilgi verme. |
| **Kompakt ve Giyilebilir Tasarım** | Lehimleme ile bileşenlerin boyutları minimize edilerek giyilebilir hale getirilmiş tasarım. |

## Donanım ve Bileşen Listesi

Projede, yer kazanmak ve giyilebilirlik sağlamak amacıyla tüm bileşenlerin jumper pinleri sökülmüş ve doğrudan kablolarla lehimlenmiştir.

| Bileşen | Model/Detay | Kullanım Amacı |
| :--- | :--- | :--- |
| **Mikrodenetleyici** | **Arduino Pro Mini** (3.3V / 5V) | Projenin ana işlem birimi. |
| **Ekran** | **OLED Ekran** | Saat arayüzünü, bildirimleri ve bağlantı durumunu gösterme. |
| **Bluetooth Modülü** | **HC-05** | Mobil uygulama ile seri iletişim kurma. |
| **Güç Kaynağı** | **250mAh LiPo Pil** | Saatin güç kaynağı. |
| **Şarj Devresi** | **Type-C Pil Şarj Devre Soketi** | LiPo pilin kolayca şarj edilmesini sağlama. |
| **Programlama** | FDTI USB-TTL Dönüştürücü | (Sadece kod yükleme aşamasında kullanıldı, nihai üründe yer almaz.) |

## Montaj ve Yapı Süreci Notları

Bu proje, prototipleme aşamasından sonra kalıcı bir giyilebilir ürüne dönüştürülmüştür. Bu süreç, projenin en kritik ve yer tasarrufu sağlayan adımlarını içerir:

1.  **Prototipleme:** İlk olarak tüm bileşenler **jumper kablolar** kullanılarak bağlanmış ve kodun hatasız çalıştığından emin olunmuştur.
2.  **Yer Tasarrufu:** Çalışan kod yüklendikten sonra, tüm bileşenlerin (özellikle HC-05, Oled Ekran ve Arduino Pro Mini) üzerindeki **gereksiz jumper pinler lehim makinesi yardımıyla sökülmüştür.**
3.  **Kompakt Lehimleme:** Gerekli tüm bağlantılar, kısa kesilmiş ve uçları açılmış ince kablolar kullanılarak, **doğrudan lehimleme** yoluyla yapılmış ve böylece maksimum alan tasarrufu sağlanmıştır.
4.  **Kasa ve Giyilebilirlik:** Lehimlenen devre, özel olarak hazırlanan bir **kutuya** yerleştirilmiş ve bir **saat kordonu** eklenerek nihai giyilebilir forma ulaştırılmıştır.

## Yazılım ve Dosya Yapısı

### Kodlama Ortamı
* **Geliştirme Ortamı:** Arduino IDE
* **Programlama Dili:** C++

### Depo İçeriği
| Dosya Yolu | Açıklama |
| :--- | :--- |
| `https://maker.robotistan.com/wp-content/uploads/2025/06/akilli_saat-apk.zip` | Akıllı saat bağlantısı için uygulama. |
| `images/` | Projenin yapım aşaması ve son haline ait fotoğraflar. |

## Proje Görselleri

| Görünüm | Açıklama |
| :---: | :--- |
| ![Nihai Ürün](images/saat_final.jpg) | Saatin kordonlu ve kutulanmış son hali. |
| ![İç Devreler](images/program_gonderim.jpg) | Lehimleme ve kompakt kablolama detaylarını gösteren iç görünüm. |
| ![Bağlantı Beklemesi](images/baglanti_bekleniyor.jpg) | Bağlantı istemi görüntüsü. |
| ![Arayüz Görüntüsü](images/giris.jpg) | Saatin OLED ekranındaki arayüzün ve bağlantı durumunun bir görüntüsü. |
| ![Şematik](images/proje_semasi.jpg) | Bileşenlerin birbirine nasıl bağlandığını gösteren genel şema. |

---
