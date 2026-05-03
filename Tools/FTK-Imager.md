# FTK Imager Kullanım Rehberi

FTK Imager, verilerin bütünlüğünü bozmadan imaj alma ve hızlı önizleme yapma konusunda endüstri standardı bir araçtır.

## Temel Fonksiyonlar
1. **Physical Drive Acquisition:** Diskin tamamının bit-bit kopyalanması.
2. **Logical Drive Acquisition:** Sadece bölümlerin (partitions) kopyalanması.
3. **Image Mounting:** Alınan bir imajın sisteme sürücü olarak bağlanması.
4. **Memory Capture:** Canlı sistemden RAM dökümü alma.

## İmaj Alma Adımları
1. `File -> Create Disk Image` yolunu izleyin.
2. Kaynak türünü (Physical/Logical) seçin.
3. `Add` butonuna basarak imaj formatını (E01 önerilir) seçin.
4. Vaka bilgilerini (Case Number, Evidence Number) doldurun.
5. `Verify images after creating` seçeneğini mutlaka işaretleyin (Bütünlük kontrolü için).

## Önemli Notlar
- FTK Imager Lite versiyonu, kurulum gerektirmeden USB bellekten çalıştırılabilir; bu da olay yerinde sistemde minimum iz bırakılmasını sağlar.
- İmaj alma işlemi bittiğinde oluşturulan `.txt` raporu, hash değerlerinin uyuşup uyuşmadığını kontrol etmek için saklanmalıdır.
