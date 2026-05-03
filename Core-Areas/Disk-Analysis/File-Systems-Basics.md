# Disk ve Dosya Sistemi Analizi Temelleri

Dijital delillerin en büyük kaynağı olan depolama birimlerinin incelenmesi, dosya sistemlerinin derinlemesine anlaşılmasını gerektirir.

## 1. İmaj Formatları
- **RAW (dd):** Verilerin bit-bit kopyasıdır. Sıkıştırma ve metadata içermez.
- **E01 (EnCase Evidence):** Adli bilişim standartıdır. Sıkıştırma, metadata (vaka no, notlar) ve bütünlük kontrolü (MD5/SHA1) içerir.
- **AFF (Advanced Forensic Format):** Açık kaynaklı ve esnek bir formattır.

## 2. Dosya Sistemleri
- **NTFS (Windows):** MFT (Master File Table), Journaling ve ADS (Alternate Data Streams) özellikleri önemlidir.
- **FAT32/exFAT:** MFT yoktur, FAT tablosu kullanılır. Silinen dosyaların kurtarılması daha kolaydır.
- **EXT4 (Linux):** Inode yapısı ve journaling analizi gerektirir.

## 3. Veri Kurtarma (File Carving)
Dosya sistemi tabloları bozulmuş veya dosyalar silinmiş olsa bile, dosyaların "header" (başlık) ve "footer" (altbilgi) imzalarına bakarak verilerin kurtarılması işlemidir.
- **Örnek İmzalar:**
  - JPEG: `FF D8 FF` ... `FF D9`
  - PDF: `%PDF-` (`25 50 44 46`)
  - ZIP/Office: `PK` (`50 4B 03 04`)

## 4. Slack Space Analizi
Dosya sisteminin küme (cluster) yapısı nedeniyle oluşan boşluklarda (File Slack) gizlenmiş verilerin aranması sürecidir.
