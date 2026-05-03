# Arkun Metodolojisi (Arkun Workflow)

Adli bilişim süreçlerinde standart ve tekrarlanabilir bir yaklaşım, elde edilen delillerin hukuki geçerliliği için kritiktir. Arkun iş akışı dört ana aşamadan oluşur:

## 1. Tanımlama (Identification)
- Olay yerindeki tüm dijital veri depolama birimlerinin tespit edilmesi.
- Bilgisayarlar, harici diskler, USB bellekler, bulut hesapları ve mobil cihazların listelenmesi.
- Cihazların durumunun (açık/kapalı) ve ağ bağlantılarının belirlenmesi.

## 2. Koruma ve Elde Etme (Preservation & Acquisition)
- **Hash Değeri:** Her türlü veri kopyalama işleminden önce ve sonra SHA-256 veya MD5 hash değerleri alınmalıdır.
- **İmaj Alma:** Orijinal delil üzerinde çalışılmamalı, yazma korumalı (write-blocker) cihazlar eşliğinde bit-tabanlı imajlar (E01, RAW) alınmalıdır.
- **Zincirleme Kanıt:** Delilin her el değiştirmesi kayıt altına alınmalıdır.

## 3. Analiz (Analysis)
- İmaj dosyaları üzerinde adli analiz araçları (Autopsy, Magnet AXIOM vb.) ile inceleme yapılması.
- Silinmiş verilerin kurtarılması, kayıt defteri incelemeleri ve zaman tüneli analizi.
- İncelenen vaka ile ilgili anahtar kelime aramaları.

## 4. Sunum ve Raporlama (Presentation & Reporting)
- Bulguların teknik detaylardan arındırılmış, hakim ve savcıların anlayabileceği bir dille raporlanması.
- Kullanılan araçların sürüm bilgileri ve analiz yöntemlerinin şeffaf bir şekilde sunulması.
