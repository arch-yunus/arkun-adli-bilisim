# Canlı Sistem Müdahalesi ve RAM Capture

Olay yerine gidildiğinde sistemin açık olması durumunda "Uçucu Verilerin" (Volatile Data) toplanması önceliklidir.

## Uçucu Verilerin Öncelik Sırası (RFC 3227)
1. Kayıtlar (Registers), Önbellek (Cache).
2. Yönlendirme Tablosu (Routing Table), ARP Önbelleği, Süreç Tablosu, Kernel İstatistikleri, Bellek (RAM).
3. Geçici Dosya Sistemleri.
4. Sabit Disk.
5. Uzak Günlükler (Remote Logging).

## RAM İmajı Alma Araçları
- **Magnet RAM Capture:** Hafif ve kullanımı kolay bir araçtır.
- **DumpIt:** Hızlı bellek dökümü almak için tercih edilir.
- **FTK Imager (Lite):** Kurulum gerektirmeden USB üzerinden çalıştırılabilir.

## Dikkat Edilmesi Gerekenler
- İmaj alma aracı, hedef sistemde mümkün olan en az izi bırakmalıdır.
- RAM imajı alındıktan sonra hash değeri hesaplanmalı ve raporlanmalıdır.
