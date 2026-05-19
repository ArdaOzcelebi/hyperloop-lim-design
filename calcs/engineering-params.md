# Başlangıç Mühendislik Parametreleri ve Hesap Gerekçeleri

Bu dökümanda, Hyperloop LIM itki sistemi için gereken tüm ana mühendislik parametreleri, ilgili hesaplamalar ve tasarım seçimlerinin gerekçeleri açıklanmaktadır.

## 1. Temel Disk ve Hedef Değerler
- Disk çapı: 1600 mm
- Disk kütlesi: 43 kg
- Çevresel hız hedefi: 10 m/s
- Efektif yarıçap: 800 mm (disk dış çevresi referansı)
- Hedef açısal hız: 10 / 0.8 = 12.5 rad/s ≈ 119.4 RPM (yarışma hedefi olan 120 RPM ile uyumlu)

## 2. Kuvvet ve Tork Hesabı
- Atalet momenti: J = 0.5 * m * r² ≈ 0.5 * 43 * 0.8² ≈ 13.76 kg·m²
- Açısal ivme: α = Δω / Δt = 12.5 / 60 ≈ 0.21 rad/s²
- Gerekli tork: T = J * α ≈ 2.87 Nm
- Gerekli lineer kuvvet: F = T / r ≈ 3.6 N (güvenlik payı ile kabaca 10 N kapasite hedeflenmektedir)

## 3. Motor ve Sargı Parametreleri (Seçim Gerekçeleriyle)
| Parametre                 | Değer (Aralık)             | Gerekçe |
|--------------------------|----------------------------|---------|
| Kutup sayısı             | 6 (başlangıç; optimize edilecek) | 1600mm/6 ~ 267mm kutup adımı ile lineer hız, 50Hz ve slip limita uygundur |
| Kutup adımı              | ≈233 mm                    | Disk çevresine oranla uygun |
| Slip                     | %5                         | Yüksek verim, hareketli yükte uygun |
| Sarım sayısı             | 18/faz (örnek)             | Yeterli manyetik kuvvet ve akı için |
| Akım değeri              | 15 A RMS (74 A max tahmini) | Slot fill ve tel çapına göre |
| Akım yoğunluğu           | 6 A/mm²                    | 2dk sürekli çalışmada ΔT<30°C için |
| Tel kalınlığı/alanı      | 2.5 mm² (multi strand)     | Akım yoğunluğuna ve slota sığmaya uygun |
| Slot fill factor         | %45                        | Bobinaj ve termal için pratik üst sınır |
| Besleme tipi             | Yıldız (Y), sonra Δ opsiyon| Test ve düşük ilk akım için |
| Sargı tipi               | Çift katman/dağıtılmış     | Manyetik alan simetrisi için |
| Operasyon frekansı       | 0–50 Hz                    | Şebeke uyumlu, hız artışına paralel |
| Termal kayıp             | 2dk’da 300–400W (I²R+çekirdek) | Hızlı test, blower soğutma ile |
| Soğutma seçimi           | Blower+kanallı soğutucu    | Kompakt alan, yüksek debi, ΔT<30°C limiti için |

Seçimlerin ayrıntılı mühendislik/termal ve alan analizleri eklenecektir.
