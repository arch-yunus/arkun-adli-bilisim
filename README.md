# ARKUN-ADLI-BILISIM

![Arkun Banner](arkun_banner.png)

**Arkun (Eski Türkçe):** Birinin arkasından giden, iz süren, takip eden.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Field](https://img.shields.io/badge/field-Digital%20Forensics-red.svg)
![Focus](https://img.shields.io/badge/focus-Türkiye%20Özel-white.svg)
![Status](https://img.shields.io/badge/status-Comprehensive-success.svg)

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
| [📂 Legislation](Legislation/) | CMK 134, delil hukuku ve iştisat notları. |
| [📂 Core-Areas](Core-Areas/) | Disk, Mobil, Bellek (RAM) ve Registry analizi teknikleri. |
| [📂 Tools](Tools/) | Sektörde kullanılan temel araçların rehberleri. |
| [📂 Templates](Templates/) | Adli rapor şablonları ve delil zinciri formları. |

---

## 🧠 Zihinsel Çerçeve (Arkun Mental Model)

Adli bilişim sadece teknik bir süreç değil, aynı zamanda disiplinler arası bir mantık yürütme sanatıdır. Arkun, inceleme sırasında **OODA Döngüsü**'nü benimser:

1.  **Gözlemle (Observe):** Olay yerini, uçuçu verileri ve fiziksel kanıtları tespit et.
2.  **Yönlen (Orient):** Eldeki verileri Türkiye mevzuatı (CMK 134) ve teknik imkanlar ışığında değerlendir.
3.  **Karar Ver (Decide):** İnceleme stratejini belirle (Hangi imaj formatı? Hangi analiz araçları?).
4.  **Harekete Geç (Act):** İmajı al, analizi yap ve bilimsel temellere dayalı raporla.

---

## ⚖️ Türk Mevzuat Uyumluluğu

Türkiye'de dijital delillerin toplanması ve değerlendirilmesi belirli kanunlara tabidir. Bu bölüm, teknik süreçlerin hukuki geçerliliğini korumak için gerekli referansları içerir:

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

### 3. Mobil Adli Bilişim (Mobile Forensics)
*   Android ve iOS cihazlardan veri çekme yöntemleri (Logical vs Physical).
*   Uygulama analizi (WhatsApp, Telegram vb. veritabanı incelemeleri).

### 4. Bellek (RAM) Analizi
*   Volatility ve MemProcFS kullanımı.
*   Zararlı yazılım izleri ve enjekte edilmiş kodların tespiti.

---

## 🛠️ Teknik Cephanelik (Technical Arsenal)

| Araç | Odak Alanı | Açıklama |
| :--- | :--- | :--- |
| **Autopsy** | Disk Analizi | Açık kaynaklı grafik arayüzlü inceleme platformu. |
| **FTK Imager** | Veri Toplama | İmaj alma, önizleme ve RAM dökümü. |
| **Volatility 3** | RAM Analizi | Gelişmiş bellek analiz framework'ü. |
| **Wireshark** | Network | Ağ trafiği ve paket analizi. |
| **Magnet RAM Capture** | Canlı Sistem | Hızlı ve güvenli bellek kopyalama. |

---

## 📅 Yapılacaklar (To-Do)

- [ ] Bulut Adli Bilişim (Cloud Forensics) bölümü ekle (AWS, Azure, Google Drive).
- [ ] IoT Cihazlar (Akıllı ev sistemleri, Drone) için analiz rehberi hazırla.
- [ ] Yapay Zeka destekli adli analiz araçlarını incele ve repoya ekle.
- [ ] Türkiye özelindeki güncel Yargıtay iştisatlarını "Legislation" altına ekle.
- [ ] Linux Adli Bilişim (Artifacts) rehberi oluştur.

---

## 🎯 Kullanım Senaryoları (Usage Scenarios)

Arkun, aşağıdaki senaryolarda bir yol haritası ve teknik referans olarak kullanılabilir:

*   **Adli Soruşturmalar:** Kolluk kuvvetleri için CMK 134 uyumlu veri toplama ve analiz süreçleri.
*   **Kurumsal Olay Müdahalesi (DFIR):** Şirket içi veri sızdırma, yetkisiz erişim veya zararlı yazılım saldırılarının analizi.
*   **Hukuki Bilirkişilik:** Hukukçular ve bilirkişiler için teknik bulguların hukuki zemine oturtulması.
*   **Akademik Araştırma:** Adli bilişim öğrencileri için metodolojik kaynak ve araç kullanım rehberleri.

---

## 🔄 Detaylı Arkun İş Akışı (Detailed Workflow)

| Aşama | Teknik Aksiyonlar | Hukuki/İdari Gereksinim |
| :--- | :--- | :--- |
| **Hazırlık** | Kitlerin sterilizasyonu, write-blocker kontrolü. | Görevlendirme yazısı / Arama kararı incelemesi. |
| **Müdahale** | RAM Capture, uçucu ağ verilerinin kaydı. | Olay yeri fotoğraflama ve çevre güvenliği. |
| **Elde Etme** | Bit-tabanlı imaj alma (E01), Hash hesaplama. | İmaj alma tutanağı ve şüpheliye kopya teslimi. |
| **İnceleme** | Dosya kurtarma, Registry ve Log analizi. | Analiz adımlarının "Audit Log" şeklinde kaydı. |
| **Raporlama** | Bulguların görselleştirilmesi ve teknik rapor. | Bilimsel mütalaa standartlarına uygunluk. |

---

## 📊 Adli Bilişim Eserleri (Artifacts) Hızlı Referans

Sıkça incelenen Windows eserleri ve konumları:

| Eser (Artifact) | Konum / Kaynak | Sağladığı Bilgi |
| :--- | :--- | :--- |
| **LNK Files** | `C:\Users\[User]\AppData\Roaming\Microsoft\Windows\Recent` | En son açılan dosya ve klasörlerin izleri. |
| **Prefetch** | `C:\Windows\Prefetch` | Uygulamaların çalışma zamanı ve sıklığı. |
| **Jump Lists** | `C:\Users\[User]\AppData\Roaming\Microsoft\Windows\Recent\AutomaticDestinations` | Görev çubuğuna sabitlenen veya sık kullanılan öğeler. |
| **ShimCache** | `SYSTEM\CurrentControlSet\Control\Session Manager\AppCompatCache` | Çalıştırılan executable dosyaların geçmişi. |
| **Browser History** | `AppData\Local\Google\Chrome\User Data\Default\History` | Web gezinti geçmişi ve indirmeler. |

---

## ⚖️ Etik İlkeler ve Profesyonel Standartlar

Adli bilişim uzmanı, inceleme sırasında aşağıdaki ilkelere sadık kalmalıdır:

1.  **Tarafsızlık:** Veriler sadece olduğu gibi raporlanmalı, yorumlar somut delillere dayanmalıdır.
2.  **Gizlilik:** İncelenen verilerdeki kişisel gizliliğe saygı duyulmalı, sadece vaka ile ilgili kısımlar raporlanmalıdır.
3.  **Bütünlük:** Orijinal kanıt asla değiştirilmemeli, tüm işlemler kopya üzerinden yapılmalıdır.
4.  **Yetkinlik:** Sadece uzmanlık alanına giren konularda görüş bildirilmeli, güncel teknolojiler takip edilmelidir.

---

## 🤝 Katkıda Bulunma

Arkun projesine katkıda bulunmak için:
1. Repoyu fork'layın.
2. Yeni bir özellik veya doküman dalı (branch) açın.
3. Değişikliklerinizi commit edin.
4. Pull Request gönderin.

*Not: Türkiye özelindeki güncel içtihatlar ve teknik raporlar özellikle beklenmektedir.*

---

## 📜 Lisans

Bu proje **MIT Lisansı** altında sunulmaktadır. İçerikler eğitim ve araştırma amaçlıdır; kötüye kullanım durumunda sorumluluk kullanıcıya aittir.

---

> *"İz silinmez, sadece doğru bakmayı bilmek gerekir."*