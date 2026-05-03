# Magnet RAM Capture Kullanım Rehberi

Magnet RAM Capture, canlı bir sistemden bellek (RAM) dökümü almak için kullanılan, minimal iz bırakan ücretsiz bir araçtır.

## Öne Çıkan Özellikleri
- Kurulum gerektirmez (Portable).
- Kullanıcı dostu ve basit arayüz.
- Farklı Windows sürümleriyle yüksek uyumluluk.
- RAW (.raw) formatında çıktı verir (Volatility ve diger araçlarla uyumlu).

## Kullanım Adımları
1. Aracı bir USB bellekten yönetici (Administrator) olarak çalıştırın.
2. `Browse` butonuna basarak imajın kaydedileceği hedefi (tercihen harici bir disk) seçin.
3. `Start` butonuna basarak süreci başlatın.
4. İşlem bittiğinde oluşturulan `.txt` dosyasındaki hash değerini not alın.

## Adli Bilişim Notu
Canlı sistemde çalışırken RAM imajı almak, sistemdeki bazı verilerin yer değiştirmesine neden olur (Smearing Effect). Ancak uçuçu verilerin (şifreler, açık bağlantılar) korunması için bu risk kabul edilebilir düzeydedir.
