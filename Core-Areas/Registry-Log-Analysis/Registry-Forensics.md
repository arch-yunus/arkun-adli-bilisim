# Windows Kayıt Defteri (Registry) ve Log Analizi

Kayıt defteri, sistem ve kullanıcı aktivitelerinin dijital "karakutusu"dur.

## 1. Kritik Kayıt Defteri Dosyaları (Hives)
- **SYSTEM:** Donanım bilgileri, sürücüler ve Timezone ayarları.
- **SOFTWARE:** Yüklü programlar ve versiyonları.
- **SAM:** Kullanıcı hesapları ve giriş bilgileri.
- **NTUSER.DAT:** Her kullanıcıya özel; son açılan dosyalar (RecentDocs), arama geçmişi ve UserAssist (çalıştırılan programlar).

## 2. Önemli Registry Anahtarları
- **UserAssist:** Kullanıcının hangi uygulamayı kaç kez ve en son ne zaman çalıştırdığını gösterir.
- **USBStor:** Sisteme takılan USB cihazların seri numaralarını ve takılma tarihlerini tutur.
- **ShellBags:** Kullanıcının hangi klasörlere eriştiğini ve pencere ayarlarını saklar.
- **Run / RunOnce:** Başlangıçta çalışan programlar (Kalıcılık/Persistence analizi için kritik).

## 3. Windows Event Logs (.evtx)
- **Security.evtx:** Başarılı/Başarısız giriş denemeleri (Event ID 4624/4625).
- **System.evtx:** Sistem açılış/kapanış, servislerin durumu.
- **Application.evtx:** Uygulama hataları ve aktiviteleri.

## 4. Timeline Analizi
Registry kayıtları ve log dosyaları birleştirilerek, olay anının saniye saniye rekonstrüksiyonu yapılır.
