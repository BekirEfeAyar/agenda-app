# Agenda App 📒

Koyu temalı, smooth animasyonlu günlük ajanda uygulaması. Web (tek dosya) + Android (Capacitor) olarak çalışır.

## Özellikler

- 📅 Haftalık takvim şeridi (hafta gezinme, gün seçimi)
- 🗓️ Daily Schedule — etkinlik ekle / sil
- ✅ Today's Tasks — animasyonlu checkbox, renkli etiketler
- 📝 Notes — ekle / düzenle / sil + Quick Notes
- ⏱️ Focus Timer (25 dk)
- 👤 Profile + istatistikler
- 💾 Veriler `localStorage`'da saklanır
- 📱 APK olarak telefona kurulabilir

## Web olarak çalıştır

`index.html` dosyasını tarayıcıda açman yeterli (internetsiz çalışır).

## Android APK derleme

Gerekenler: Node.js, JDK 17, Android SDK.

```bash
npm install
npx cap sync android
cd android
./gradlew assembleDebug   # Windows: gradlew.bat assembleDebug
```

APK çıktısı: `android/app/build/outputs/apk/debug/app-debug.apk`

Hazır APK'yı **Releases** sayfasından indirebilirsin.

## Proje yapısı

```
agenda-app/
├── index.html          # uygulamanın tamamı (web)
├── www/                # Capacitor web klasörü
├── capacitor.config.json
├── package.json
└── android/            # Capacitor Android projesi
```
