# Eski Java Oyunları / J2ME Browser Emulator

Bu proje, eski Java ME (J2ME) mobil oyunlarını tarayıcıda oynatmak için hazırlanmış bir oyun kataloğu ve emülatör arayüzüdür. Kullanıcılar, eski telefon oyunlarını doğrudan web tarayıcısından açıp oynayabilir.

Canlı demo:
https://alpgube7.github.io/java-oyun-sitesi/

## Özellikler

- Eski Java/J2ME oyunlarının listelenmesi
- Arama ve kategori filtreleme
- Tarayıcı içinde oyun açma
- Mobil uyumlu ve duyarlı arayüz
- Klavye ve dokunmatik kontrol desteği
- PWA benzeri kurulum desteği
- Önbellekleme (service worker) ile tekrar yükleme deneyimi

## Proje Yapısı

```text
.
├── index.html              # Ana oyun kataloğu sayfası
├── run.html                # Oyun oynatma sayfası
├── launcher.html           # Alternatif başlatıcı arayüzü
├── games.json              # Oyun verileri
├── manifest.json           # PWA manifest
├── sw.js                   # Service worker
├── freej2me-web.jar        # Embedded emulator/runtime
├── favicon.svg             # Uygulama ikonu
├── favicon.png
├── apple-touch-icon.png
├── src/
│   ├── main.js             # Ana çalışma mantığı
│   ├── launcher.js         # Başlatıcı davranışları
│   ├── key.js              # Klavye işlemleri
│   ├── keyMapper.js        # Tuş eşleme mantığı
│   ├── keyMapperUI.js      # Tuş eşleme arayüzü
│   ├── screenKbd.js        # Ekran klavyesi desteği
│   ├── eventqueue.js       # Olay kuyruğu
│   └── ...
├── jar/                    # Oyun JAR dosyaları
├── libjs/                  # JavaScript runtime dosyaları
├── libmedia/               # Medya bileşenleri
├── libmidi/                # MIDI bileşenleri
├── .gitignore
├── generate-favicon.html
├── init.zip
├── init-original.zip
├── test-keymapper.html
├── README.md
└── ...