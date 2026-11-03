# Yol Arkadaşı — koridor verileri

Bu depo uygulama için imzalı, herkese açık koridor veri paketlerini içerir. Kullanıcı yolculukları veya konum kayıtları içermez.

## Kapsam

İlk paket: Bursa–Ankara, iki yönde toplam 12 koridor. Paket sıra numarası 2; yayın hazırlığı 3 Kasım 2026. Koordinat kayıt tarihi 19 Ekim 2026'dır. Paket yayını, kaynak bilgilerinin yeni tarihte güncellendiği anlamına gelmez.

Ad, mesafe ve hız sınırları 2 Kasım 2026 sorgusunda radarnoktalari.com.tr listesiyle karşılaştırılmıştır. Kamera koordinatlarının sahada doğrulanması bekleniyor. Yol çizgileri OpenStreetMap / OSRM üzerinden hazırlanmış aday çizgilerdir. Veriler resmî hız izni veya doğruluk garantisi değildir; güncel trafik levhaları esas alınmalıdır.

Kaynaklar:
- https://radarnoktalari.com.tr/
- https://www.trafik.gov.tr/iller-arasi-radar-ve-kontrol-noktasi-uygulama-sayilari
- https://www.openstreetmap.org/copyright

## Paket

`catalog.signed.json` içinde tam veri metni ve Ed25519 imzası birlikte bulunur. Uygulama kendisine önceden tanımlanmış açık anahtarla doğrular. Özel imza anahtarı bu depoya konmaz. İmza, paketin yayıncısını ve değiştirilmediğini doğrular; yol verisinin gerçek dünyada doğru olduğunu kanıtlamaz.
