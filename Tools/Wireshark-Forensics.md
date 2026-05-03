# Wireshark ile Ağ Adli Bilişimi (Network Forensics)

Ağ trafiği, saldırganların sistemler üzerindeki hareketlerini ve veri sızdırma girişimlerini tespit etmek için kritik bir kaynaktır.

## 1. Paket Yakalama (Packet Capture)
- **.pcap / .pcapng:** Wireshark tarafından kullanılan standart dosya formatları.
- **Promiscuous Mode:** Ağ kartının, kendisine ait olmayan paketleri de yakalamasını sağlar.

## 2. Temel Filtreler
- `ip.addr == 192.168.1.1`: Belirli bir IP adresiyle ilgili tüm paketleri gösterir.
- `tcp.port == 80 || tcp.port == 443`: Sadece HTTP ve HTTPS trafiğini filtreler.
- `http.request.method == "POST"`: Form gönderimlerini (parola, veri girişi) yakalar.
- `dns.flags.response == 0`: DNS sorgularını gösterir.

## 3. Adli Analiz İpuçları
- **Follow TCP Stream:** Parçalı paketleri birleştirerek tüm iletişimi okunabilir hale getirir.
- **Export Objects:** HTTP trafiği üzerinden indirilen dosyaları (EXE, JPG vb.) dışa aktarır.
- **Statistics -> Endpoints:** Hangi IP'nin en çok veri trafiği oluşturduğunu tespit eder (C2 sunucusu tespiti için).

## 4. Şifreli Trafik Analizi
TLS/SSL ile şifrelenmiş trafik, anahtar dosyaları (SSL Key Log) olmadan okunamaz. Ancak paket boyutları ve zamanlamaları üzerinden "Traffic Pattern Analysis" yapılabilir.
