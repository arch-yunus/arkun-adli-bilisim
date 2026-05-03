# Mobil Adli Bilişim (Mobile Forensics)

Mobil cihazlar, kişisel verilerin, konum bilgilerinin ve iletişim kayıtlarının en yoğun bulunduğu mecralardır.

## 1. Veri Elde Etme Yöntemleri
- **Mantıksal Elde Etme (Logical Acquisition):** Cihazın işletim sistemi üzerinden izin verilen dosyaların (rehber, mesajlar, arama kayıtları) alınmasıdır.
- **Dosya Sistemi Elde Etme (File System Acquisition):** Tüm dosya yapısının kopyalanmasıdır. Veritabanı dosyalarına erişim sağlar.
- **Fiziksel Elde Etme (Physical Acquisition):** Bellek çiplerinin bit-bit kopyalanmasıdır. Silinmiş verilerin kurtarılmasına olanak tanır.

## 2. Android Analizi
- **ADB (Android Debug Bridge):** Veri çekme ve komut çalıştırma için kullanılır.
- **SQLite Veritabanları:** WhatsApp, Telegram ve SMS kayıtları genellikle `/data/data/` altındaki SQLite dosyalarında saklanır.
- **APK Analizi:** Şüpheli uygulamaların izinleri ve kaynak kodları incelenmelidir.

## 3. iOS Analizi
- **iTunes Yedekleri:** Parolasız yedeklerden önemli miktarda veri çekilebilir.
- **Checkm8/Checkra1n:** Donanımsal açıklar kullanılarak yapılan tam imaj alma işlemleri.
- **Keychain Analizi:** Saklanan parolaların çözülmesi.

## 4. Uygulama Analizi
Mesajlaşma uygulamalarında "Write Ahead Logs" (WAL) dosyaları, henüz ana veritabanına yazılmamış güncel yazışmaları içerebilir.
