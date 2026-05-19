# Simulation & Analysis Template

Bu klasör, Hyperloop LIM projesi için temel termal ve manyetik analizlere dair şablon ve örnek belgeleri içerir.

## Analiz Planı

### 1. Manyetik Analiz (FEA)
- Amaç: Simülasyon ile manyetik alan dağılımı, akı yoğunluğu ve çekirdek/sarım doygunluğu tespiti
- Kullanılan yazılım (örn. ANSYS Maxwell, COMSOL Multiphysics, Infolytica vb.)
- Temel girişler: Disk geometrisi, kutup adımı, hava aralığı, besleme akımı/frekansı
- Beklenen çıktı: Manyetik akı haritaları, maksimum/minimum B (Tesla), kuvvet-doğrulaması grafikleri
- Yorum: Doygunluk sınırı aşımı/güvenli sınır içinde çalışma vurgulanmalı

---

### 2. Termal Analiz
- Amaç: Kısa (2 dk) tam yükteki sargı, çekirdek ve ray sıcaklık artışı (ΔT) değerlendirmesi
- Kullanılan analiz aracı (örn. ANSYS, Solidworks Simulation, manuel enerji dengesi hesapları)
- Temel girişler: Sarım direnç kaybı (I²R), çekirdek kaybı, başlangıç ortam sıcaklığı, blower/fan debisi, ısı transfer katsayıları
- Beklenen çıktı: Sargı, gövde ve ray ΔT profili, zaman-ΔT eğrileri, maksimum sıcaklık grafikleri
- Yorum: ΔT<30°C limitinin sağlanıp sağlanmadığı analiz edilmeli

---

### 3. Kısa Yorum ve Sonuç
- Kritik noktaların tespiti (ör. hangi şartlarda limit aşılıyor, hangi soğutma rejimi işe yarıyor)
- Tasarımda gerekirse düzeltilecek veya optimize edilecek parametreler

---

Her analiz çıktısı .jpg/.png grafik veya uygun tablo ile bu klasörde paylaşılabilir.

## Görselleştirme ve Basit Simülasyon
- Test standı geometrisi ve parametre tabanlı 120 saniyelik basit hızlanma simülasyonu için:
  - [simulation/test-stand-visualization.html](test-stand-visualization.html)
