# 🚩 ARKUN-ADLI-BILISIM

![Arkun Banner](arkun_banner.png)

**Arkun (Eski Türkçe):** Birinin arkasından giden, iz süren, takip eden.

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Field](https://img.shields.io/badge/field-Digital%20Forensics-red.svg)](https://github.com/topics/forensics)
[![Focus](https://img.shields.io/badge/focus-Türkiye%20Özel-white.svg)](https://github.com/arch-yunus/arkun-adli-bilisim)
[![Status](https://img.shields.io/badge/status-Comprehensive-success.svg)](https://github.com/arch-yunus/arkun-adli-bilisim)

---

## 🛡️ Hakkında

**Arkun**, Türkiye'deki adli bilişim dünyasına (Digital Forensics) yönelik standartları, metodolojileri, araç setlerini ve hukuki süreçleri bir araya getiren kapsamlı bir açık kaynak bilgi deposudur. Türk mitolojisindeki "iz sürme" kavramından ilham alarak, dijital dünyada bırakılan kanıtların bilimsel ve hukuki çerçevede nasıl inceleneceğini rehber edinir.

Bu repo, adli bilişim uzmanları, kolluk kuvvetleri, hukukçular ve siber güvenlik araştırmacıları için Türkiye mevzuatına (CMK 134 vb.) uyumlu bir yol haritası sunar.

---

## 🏗️ Proje Yapısı

Repo, modüler ve kolay erişilebilir bir hiyerarşiyle yapılandırılmıştır:

| Dizin | Açıklama |
| :--- | :--- |
| [📂 Methodology](Methodology/) | İş akışları, ilk müdahale kontrol listeleri ve metodolojiler. |
| [📂 Legislation](Legislation/) | CMK 134, delil hukuku ve içtihat notları. |
| [📂 Core-Areas](Core-Areas/) | Disk, Mobil, Bellek (RAM) ve Registry analizi teknikleri. |
| [📂 Tools](Tools/) | Sektörde kullanılan temel araçların rehberleri. |
| [📂 Templates](Templates/) | Adli rapor şablonları ve delil zinciri formları. |

---

## 🧠 Zihinsel Çerçeve (Arkun Mental Model)

Adli bilişim sadece teknik bir süreç değil, aynı zamanda disiplinler arası bir mantık yürütme sanatıdır. Arkun, inceleme sırasında **OODA Döngüsü**'nü benimser:

1.  **Gözlemle (Observe):** Olay yerini, uçucu verileri ve fiziksel kanıtları tespit et.
2.  **Yönlen (Orient):** Eldeki verileri Türkiye mevzuatı (CMK 134) ve teknik imkanlar ışığında değerlendir.
3.  **Karar Ver (Decide):** İnceleme stratejini belirle (Hangi imaj formatı? Hangi analiz araçları?).
4.  **Harekete Geç (Act):** İmajı al, analizi yap ve bilimsel temellere dayalı raporla.

---

## ⚖️ Türk Mevzuat Uyumluluğu

Türkiye'de dijital delillerin toplanması ve değerlendirilmesi belirli kanunlara tabidir:

*   **CMK Madde 134:** Bilgisayarlarda, bilgisayar programlarında ve kütüklerinde arama, kopyalama ve elkoyma usulleri.
*   **Hukuki Geçerlilik:** İmaj alma süreçlerinde "Hash" değerinin önemi ve zaman damgası kullanımı.
*   **Zincirleme Kanıt (Chain of Custody):** Delilin ilk elde edildiği andan mahkeme salonuna kadar olan sürecin dokümantasyonu.

---

## 🔍 Temel Çalışma Alanları

### 1. Olay Yerine Müdahale (First Response)
*   Canlı sistemlerde veri toplama (RAM Capture).
*   Uçucu verilerin korunması ve sıralaması.
*   Yazma korumalı (Write-Blocker) donanımların kullanımı.

### 2. Disk ve Dosya Sistemi Analizi
*   E01, RAW, AFF imaj formatları.
*   NTFS, FAT32, exFAT ve EXT4 dosya sistemlerinde derinlemesine inceleme.
*   Silinmiş dosyaların kurtarılması (File Carving).

---

## 🛠️ Teknik Cephanelik (Technical Arsenal)

| Araç | Odak Alanı | Açıklama |
| :--- | :--- | :--- |
| **Autopsy** | Disk Analizi | Açık kaynaklı grafik arayüzlü inceleme platformu. |
| **FTK Imager** | Veri Toplama | İmaj alma, önizleme ve RAM dökümü. |
| **Volatility 3** | RAM Analizi | Gelişmiş bellek analiz framework'ü. |
| **Wireshark** | Network | Ağ trafiği ve paket analizi. |

---

## 📖 Adli Bilişim Sözlüğü (Glossary)

| Terim (TR) | Term (EN) | Açıklama |
| :--- | :--- | :--- |
| **Adli Kopya** | Forensic Image | Bir depolama ortamının bit-bit alınmış birebir kopyası. |
| **Uçucu Veri** | Volatile Data | Güç kesildiğinde kaybolan veriler (RAM, Ağ bağlantıları). |
| **Yazma Koruması** | Write Protection | Orijinal delilin değiştirilmesini engelleyen mekanizma. |
| **Dosya Kazıma** | File Carving | Dosya sistemi tabloları olmadan veri kurtarma tekniği. |
| **Zaman Damgası** | Timestamp | Bir olayın gerçekleştiği tarih ve saat bilgisinin kaydı. |

---

## 🔬 Adli Forensics Laboratuvar Kurulumu

Profesyonel bir inceleme ortamı için gereken temel bileşenler:

### Donanım Gereksinimleri
- **Forensic Workstation:** Yüksek işlemci gücü ve min. 64GB RAM.
- **Write-Blockers:** Tableau veya WiebeTech marka donanımsal koruyucular.
- **Steril Depolama:** İmajların saklanacağı yüksek kapasiteli ve güvenli diskler.

### Yazılım Gereksinimleri
- **İnceleme OS:** SIFT Workstation (SANS) veya TSK (The Sleuth Kit).
- **Veritabanı İzleyici:** DB Browser for SQLite (WhatsApp/Mobil analiz için).

---

## 🔄 Vaka Yaşam Döngüsü (Case Lifecycle)

| Aşama | Aksiyon | Çıktı |
| :--- | :--- | :--- |
| **Olay** | Şüpheli durumun tespiti. | İlk bildirim kaydı. |
| **Müdahale** | Delillerin güvene alınması. | Fiziksel delil listesi. |
| **Toplama** | Adli imajların alınması. | Hash değerleri (MD5/SHA1). |
| **Analiz** | Artefact incelemesi. | Teknik bulgular raporu. |
| **İfade** | Teknik bulguların sunumu. | Bilirkişi raporu / Mahkeme sunumu. |

---

## 📅 Yapılacaklar (To-Do)

- [x] AD (Active Directory) saldırı metodolojisi eklendi.
- [x] Heap Exploitation cheat-sheet oluşturuldu.
- [x] Temel araç konfigürasyonları `Tools/` altına taşındı.
- [ ] Bulut Adli Bilişim (Cloud Forensics) bölümü ekle (AWS, Azure).
- [ ] IoT Cihazlar (Smart Home, Drone) için analiz rehberi hazırla.
- [ ] Türkiye özelindeki güncel Yargıtay içtihatlarını ekle.

---

## 🤝 Katkıda Bulunma
Arkun projesine katkıda bulunmak için repoyu fork'layın ve Pull Request gönderin. Türkiye özelindeki güncel içtihatlar ve teknik raporlar özellikle beklenmektedir.

---

## 📜 Lisans
Bu proje **MIT Lisansı** altında sunulmaktadır.

---

> *"İz silinmez, sadece doğru bakmayı bilmek gerekir."*
