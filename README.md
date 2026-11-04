# Yol Arkadaşı — koridor verileri

Bu depo uygulama için imzalı, herkese açık koridor veri paketlerini içerir. Kullanıcı yolculukları veya konum kayıtları içermez.

## Kapsam

Paket 4: Bursa–Ankara, Kulu–Konya ve Ankara–Aksaray, iki yönde toplam 22 koridor / 6 güzergâh seçeneği. Yayın hazırlığı 4 Kasım 2026.

- Bursa–Ankara: 12 koridor, koordinat kayıt tarihi 19 Ekim 2026.
- Kulu–Konya: 6 koridor, kaynak kayıt tarihi 3 Kasım 2026. Her yönde 40 + 14 + 70 = 124 km denetim bölümü. Ankara–Kulu ve Konya şehir içi kapsam dışıdır.

Paket yayını, bütün kaynak kayıtlarının aynı tarihte yenilendiği anlamına gelmez. Kulu–Konya kayıtları Ankara/Çankaya–Konya/Selçuklu sorgusundan alınmıştır: https://radarnoktalari.com.tr/?gz_from=1231&gz_to=1839

İki kaynak aynı sorguda 19 koridor gösterdi; 13 örtüşen şehir içi koridor bu pakete alınmadı. Resmî toplam sayı karşılaştırması, koordinatların metre hassasiyetinde bağımsız doğrulaması değildir.

Bursa–Ankara ad, mesafe ve hız sınırları 2 Kasım 2026 sorgusunda radarnoktalari.com.tr listesiyle karşılaştırılmıştır. Kamera koordinatlarının sahada doğrulanması bekleniyor. Yol çizgileri OpenStreetMap / OSRM üzerinden hazırlanmış aday çizgilerdir. Veriler resmî hız izni veya doğruluk garantisi değildir; güncel trafik levhaları esas alınmalıdır.

Kaynaklar:
- https://radarnoktalari.com.tr/
- https://www.trafik.gov.tr/iller-arasi-radar-ve-kontrol-noktasi-uygulama-sayilari
- https://www.openstreetmap.org/copyright

## Paket

`catalog.signed.json` içinde tam veri metni ve Ed25519 imzası birlikte bulunur. Uygulama kendisine önceden tanımlanmış açık anahtarla doğrular. Özel imza anahtarı bu depoya konmaz. İmza, paketin yayıncısını ve değiştirilmediğini doğrular; yol verisinin gerçek dünyada doğru olduğunu kanıtlamaz.

## Ankara–Aksaray eklemesi

4 Kasım 2026 sorgusu: https://radarnoktalari.com.tr/?gz_from=1231&gz_to=1120

Her yönde iki koridor, kaynak mesafeleri 116 + 69 = 185 km. Ankara ucu Gölbaşıdır; koridorlar arasındaki boşluklar denetim bölümü sayılmaz. Resmî sorgu ve kaynak aynı 4 koridor / 3 radar / 7 kontrol toplamını gösterdi. Bu, koordinatların bağımsız doğrulaması değildir.

Gölbaşı–Şereflikoçhisar aday yol çizgileri kaynakta belirtilen 116 km’den yaklaşık %3,35–%3,57 uzundur. Kaynağın 116 km değeri korunmuştur; yol çizgileri ve kamera konumları sahada doğrulanmamıştır. 2, 5 ve 8 saniyelik sentetik örnekler geçti; seyrek örneklerde belirsizlik korumaları sürer.
