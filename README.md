# Hyperloop Lineer İndüksiyon Motor (LIM) İtki Sistem Tasarımı

Bu repo, Hyperloop yarışması için çift taraflı lineer indüksiyon motoruna (LIM) sahip bir itki sisteminin mühendislik gereksinimlerini, teknik parametrelerini ve tasarım sürecini ayrıntılı ve gerekçeli şekilde dökümante eder.

## Kapsam & Amaç
- Amaç: Hyperloop taşıma sisteminde, yarışma kurallarına ve teknik sınırlara uygun olarak güvenilir, verimli ve iki dakika tam güçte çalışabilen LIM itki sistemi tasarımı.
- Kapsam: Teknik seçimin her adımı (kutup sayısı, kutup adımı, sarım tipi, akım, bağlantı, slot fill, termal soğutma, güvenlik, performans/güç analizi vb.), her biri açık mühendislik hesabı ve yarışma kuralları referansıyla gerekçelendirilmiş olarak açıklar.

## Dosya Yapısı
- `README.md`: Proje özeti ve içerik indexi
- `/docs/`: Kurallar özeti, test düzeneği ve güvenlik
- `/calcs/`: Tüm mühendislik hesaplamaları ve seçimlerin gerekçeleri
- `/design/`: Teknik çizimler ve CAD referansları
- `/simulation/`: Termal ve manyetik analiz çıktı şablonları

## Kısa Teknik Bilgi
- Disk çapı: 1600 mm
- Hava aralığı: 2-3 mm (her iki tarafta), çift taraflı LIM
- Güç beslemesi: 220/380V AC, 50 Hz
- Sürekli çalışmada termal yükselme: ΔT < 30°C
- Montaj güvenlik alanı: Üst kenarı 600 mm, alt kenarı 1300 mm, yüksekliği 600 mm olan yamuk (yeşil alan)

## Test Düzeneği Görselleri
Güncel çizimler ve ölçüler docs/test-rig-images.md dosyasında bulunur.

---
Her klasörde, başlıklar ve dosyalar ilerledikçe eklenecek ve gerekçeler-ölçümler-analizler eklenmeye devam edecektir.
