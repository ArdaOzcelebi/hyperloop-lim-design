# FMEA (Failure Modes and Effects Analysis) & Güvenlik Belgesi

Bu döküman, Lineer İndüksiyon Motor (LIM) itki sistemi için olası arıza modlarının analizini, güvenlik kritik noktalarını, önerilen önlemleri ve izlenecek test/güvenlik protokolünü içerir.

## 1. FMEA Tablosu (Örnek)
| Sistem/Altbileşen | Olası Arıza Modu | Muhtemel Etki | Olasılık | Ciddiyet | Saptanabilirlik | Risk Öncelik | Önerilen Önlem |
|-------------------|------------------|--------------|----------|----------|-----------------|--------------|----------------|
| LIM Sargısı       | Aşırı ısınma     | İzolasyon yanması, kısa devre | 2/5 | 4/5 | 4/5 | 32/125       | Termistör ile izleme, blower zorunlu |
| Disk              | Mekanik çatlak   | Disk kırılması | 1/5 | 5/5 | 2/5 | 10/125 | Periyodik NDT, kapalı muhafaza |
| Güvenlik tekerlekleri | Boşta dönmeme / aşırı aşınma | Rayda çizik, sistem devrilmesi | 2/5 | 5/5 | 3/5 | 30/125 | Malzeme seçimi, testten önce gözle muayene |
| Elektrik bağlantı | Gevşeme/yüksek direnç | Ark, kopma, güç kaybı | 2/5 | 3/5 | 4/5 | 24/125 | Vidala sabitleme, test öncesi kontrol |

## 2. Fail-Safe ve Güvenlik Protokolü
- Sıcaklık, akım ve hız sürekli izlenecek. Limit aşımında sistem otomatik olarak kapanmalı.
- Blower soğutma sürekli çalışacak. Akım sensörüyle blower kontrolü yapılmalı.
- Tüm dış muhafaza ve test alanı, operatör temas riskine karşı fiziksel bariyer ile çevrilmeli.
- Güvenlik tekerlekleri, açısal teması kaybetmeyecek şekilde limit switch ile izlenebilir.
- Enerji besleme, kolay erişimli, kazanımlı acil durdurma (emergency stop) içerir.

## 3. Test/İzleme
- Sıcaklık, akım ve mekanik titreşim loglanır.
- FMEA yoluyla riskli görülen her bir arıza için test öncesi kontrol listesi hazırlanır.
- Test sırasında operatör gözetiminde, üç aşamalı (min/nominal/maks) yük testleri yapılır.

Belge geliştikçe, yeni risk ve önlemlerle güncellenecektir.