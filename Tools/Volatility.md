# Volatility 3 Kullanım Rehberi

Volatility, bellek (RAM) imajlarını analiz etmek için kullanılan dünyanın en gelişmiş açık kaynaklı çerçevesidir.

## Temel Komut Yapısı
Volatility 3'te profil seçimine gerek kalmadan otomatik sembol yönetimi yapılır:
`python vol.py -f [imaj_yolu] [plugin_adi]`

## Sık Kullanılan Pluginler
- **windows.pslist:** Çalışan süreçleri listeler.
- **windows.pstree:** Süreçleri hiyerarşik (ebeveyn-çocuk) yapıda gösterir.
- **windows.netstat:** Aktif ağ bağlantılarını ve dinlenen portları listeler.
- **windows.registry.printkey:** Belirli bir kayıt defteri anahtarını okur.
- **windows.malfind:** Enjekte edilmiş kod izlerini arar.
- **windows.cmdline:** Süreçlerin hangi komut satırı argümanlarıyla çalıştığını gösterir.

## Analiz İpuçları
1. Önce `pslist` ve `pstree` ile olağandışı süreçleri belirleyin.
2. `netstat` ile şüpheli bir IP adresiyle bağlantı olup olmadığını kontrol edin.
3. `malfind` ile gizli kod parçalarını dump edin ve Virustotal gibi servislerde taratın.
